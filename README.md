###### Task Day: 1
# HTTP 1.1 :fist_right::fist_left: HTTP 2 (Layman Explaination)

### Before we get into the differences, let's take a look at what HTTP really means...

##HTTP
HTTP stands for HyperText Transfer Protocol. It is the foundation of any data exchange on the Web, and it is a protocol used for transmitting hypertext (text that is linked together) over the Internet. In simpler terms, it's the set of rules that allows your web browser to request a particular web page from a server and then display it on your screen.
*Think of HTTP like a conversation between your web browser (like Chrome or Firefox) and a server (a powerful computer somewhere that stores a website). This conversation happens every time you open a webpage.*

##HTTP 1.1
HTTP/1.1 is like a set of rules that helps your web browser and a server communicate when you're browsing the internet.

### 1. Making Requests
When you type a web address and hit Enter, your browser sends a request to the server, asking for the webpage.
### 2. Getting Responses
The server receives the request and sends back the webpage. It's like your browser asking for a page, and the server handing it over.
### 3. One at a time:
With HTTP/1.1, these requests and responses happen one after the other. If your browser needs multiple things to show a webpage (like images or scripts), it asks for them one by one.
### 4. Multiple Connections:
Sometimes, your browser opens multiple connections to the server to speed things up. It's like having several lanes on a highway to carry different parts of the webpage.
### 5. Header Information:
Each time your browser makes a request, it sends some extra information (headers) to the server. This includes details like the type of browser you're using.
### 6. Not always the fatest:
Because requests are handled one by one, and there's some overhead with headers, it can make things a bit slower, especially for complex webpages.

##Essence
HTTP/1.1 is the language that allows your browser and the server to talk, but it's like a polite conversation where they take turns. It works well for many situations, but as websites became more complex, there was room for improvement, which led to the development of newer versions like HTTP/2.
