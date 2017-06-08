### ARCHITECTURE
- command and controll instance running on a DO with redis to store the user information
- each crawler runs on a heroku instance (5 free per email).
- c&c distributes the work between crawlers
- crawlers send data back to c&c
- crawler has the server's public key, server send a request for a task to crawler through REST
### DESIRED FUNCTIONALITY
- collect all users who retweeted a tweet (this can be done through the mobile interface)
- collect all users who liked a tweet
- collect all users who follow this user
- collect all shared followers
### TIPS
- [How to override XHR in CasperJS](https://stackoverflow.com/questions/24555370/how-can-i-catch-and-process-the-data-from-the-xhr-responses-using-casperjs)
