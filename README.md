
![Logo](https://i.ibb.co/4MPGGhX/tweeter-logo.png)


# Tweeter Chatting Application

A twitter-clone UDP social-networking application built with Python's socket module.

## Diagram (App Architecture)
![Architecture](https://i.ibb.co/XDc4NsM/Screenshot-2023-07-31-133509.png)

## Features
- Register: registers a user to the tweeter application. It will take a handle (username), an IP address, and 3 ports (one port for communication between the tracker and itself, and two for following other users).
- Query handles: returns a list of handles (usernames) that are currently registered in the tweeter application to the client.
- Follow: follows another user
- Drop: unfollows another user
- Tweet: sends out a tweet (message) to the followers
- End tweet: makes sure all the tweets are sent in the correct order
- Exit: exits the application 

## Demo Video
https://www.youtube.com/watch?v=VLRv4gq_WjY&ab_channel=BryanMatthew


## Usage/Examples
- Start the server
```command
python UDPServer.py
# Enter an IP address for the server
```
- Start the client (One terminal for each user)
```command
python UDPClient.py 
# Enter an IP address for the client
# Enter an IP for the server
# Enter the 3 port numbers that are going to be used
```
- Register
```command
register @handle IP Port1 Port2 Port3
```
- Query Handles
```command
query handles
```
- Follow
```command
follow @handle @handle_to_follow
```
- Unfollow
```command
drop @handle @handle_to_unfollow
```
- Tweet
```command
tweet @handle "message"
```
- End Tweet
```command
end tweet
```
- Exit
```command
exit
```

## Author(s)
- [@bryan-matthew](https://www.github.com/bryan-matthew)

