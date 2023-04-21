# Lab Report 2 #
## Part 1 ##

**StringServer Code:**

StringServer.java:
```
import java.io.IOException;
import java.net.URI;
import java.util.ArrayList;
import java.util.List;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.

    String message = "";

    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return message;
        }
        else {
            System.out.println("Path: " + url.getPath());
            if (url.getPath().contains("/add-messages")) {
                if (url.getQuery().startsWith("s=")) {
                    message += url.getQuery().substring(2) + "\n";
                    return message;
                }
                else {
                    return "404 Not Found";
                }
            }
            return "404 Not Found!";
        }
    }
}

class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```
  
**StringServer Example 1:**

**stringServer Examples 2:**
