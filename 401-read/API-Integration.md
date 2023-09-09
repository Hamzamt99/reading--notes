# Explain the different between a query string parameter and a path parameter.

## - A query string parameter is appended to the end of a URL and starts with a "?", used to send optional data to a server, often for filtering or pagination.
## - A path parameter is a part of the URL path, typically enclosed in curly braces, and is used to specify a specific resource or identifier in the URL.

# What would our API URL with a path id parameter be given the following information:
### Domain: http://our-site.com
### v3
### model name: stuff
### id: things 
##  http://our-site.com/stuff?id=things

# We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.
### Think of the interface like a menu at a restaurant. It shows you all the options (or functions) the API can do.
### When you order from the menu, you're actually using the API to get the data or do a specific task, just like choosing a dish to eat.

# Describe how you would use middleware to implement basic and bearer auth.

### To implement basic auth with middleware, you'd decode the base64-encoded credentials from the request header and validate them.
### For bearer auth, you'd extract the token from the request header, verify its authenticity, and grant access accordingly

# Describe the handshake necessary to implement OAuth.
### The user requests access to a resource from a client app.
### The client redirects the user to the authorization server, 
### where the user grants permission, and the server issues an access token to the client to access the resource on behalf of the user.

# Describe how Role Based Access Control works to a non-technical friend.

### Think of Role-Based Access Control like different levels of access cards in a building. Each person has a card (role) that allows them to access certain rooms (permissions).
### You get the card (role) that matches your job, so you can only go where you're supposed to, keeping things secure.
