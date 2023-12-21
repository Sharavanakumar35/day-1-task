# HTTP 1.1 :fist_right::fist_left: HTTP 2 (Layman Explaination)

### Before we get into the differences, let's take a look at what HTTP really means...

## HTTP
HTTP stands for HyperText Transfer Protocol. It is the foundation of any data exchange on the Web, and it is a protocol used for transmitting hypertext (text that is linked together) over the Internet. In simpler terms, it's the set of rules that allows your web browser to request a particular web page from a server and then display it on your screen.

*Think of HTTP like a conversation between your web browser (like Chrome or Firefox) and a server (a powerful computer somewhere that stores a website). This conversation happens every time you open a webpage.*

## HTTP 1.1
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

### Essence
HTTP/1.1 is the language that allows your browser and the server to talk, but it's like a polite conversation where they take turns. It works well for many situations, but as websites became more complex, there was room for improvement, which led to the development of newer versions like HTTP/2.


## HTTP 2
HTTP/2 is an upgraded version of the communication rules between your web browser and the server when you're surfing the internet.

### 1. Talking Simultaneously:
Unlike HTTP/1.1, where requests happen one after the other, HTTP/2 allows your browser to ask for multiple things at the same time. It's like opening several lanes on a data highway so that different parts of a webpage can be requested simultaneously.
### 2. Smarter Communication:
HTTP/2 is better at compressing the information it sends between your browser and the server. Think of it as using a more efficient language that saves space and time, making the communication faster.
### 3. Single Connection Efficiency:
Instead of opening several connections to the server, HTTP/2 uses a single connection more efficiently. It's like having a streamlined conversation channel that can handle multiple topics without creating unnecessary complexity.
### 4. Prioritizing Needs:
With HTTP/2, your browser and the server can agree on what's more important to load first. This prioritization ensures that crucial parts of a webpage, like the main content, are delivered faster.
### 5. Proactive Loading:
HTTP/2 introduces a feature called server push. Imagine the server not only sending what your browser asked for but also predicting what you might need next and sending it in advance. It's like a helpful friend who hands you things before you even ask.

### Essence
HTTP/2 is an improvement that allows your browser and the server to communicate more efficiently. It's like upgrading from a single-lane road to a multi-lane highway, making your web experience faster and smoother, especially for modern, complex websites.


## Differences Overview

| Feature                    | HTTP/1.1                               | HTTP/2                                         |
|----------------------------|----------------------------------------|------------------------------------------------|
| Multiplexing               | Limited to one request per connection   | Enables multiple concurrent requests (streams) |
| Header Compression         | Not supported                          | Utilizes Huffman coding for header compression   |
| Protocol Format            | Text-based                            | Binary format                                  |
| Connection Management      | Multiple connections for parallelism   | Single, multiplexed connection for efficiency  |
| Server Push                | Not supported                          | Allows proactive pushing of resources          |
| Stream Prioritization      | Not prioritized                       | Supports prioritization for efficient loading |
| Persistent Connections     | Requires multiple connections         | Promotes connection reuse for reduced overhead |
