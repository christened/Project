# Project
Sample full stack development project 

> You will be using javascript to create an application. The application requires a database, a server, and a front-end. All of this will be written in Javascript.

## Technology Stack
0. NPM - npm is a package manager for Node. It let's you use libraries for your javascript application either in the front-end or back-end.
1. React - is a javascript front-end (client-side) framework by Facebook.
2. Node and Express - Express is a server side framework that lets you write servers in javascript. It is build on top of Node.
3. MongoDB or RethinkDB - is a database (NoSQL) that stores your data

## Requirements
> You will use the technologies written in **Technology Stack**

1. As a user I would like to login using a username and password or using facebook oAuth
2. As a user I would like to post a to do list that everyone can see
3. As a user I would like to comment on any post
4. As a user I would like to edit or delete my own posts or comment.  
5. As a user I would like to find all the post or comments near my proximity.
6. A post/comment should display the name of the Poster/Commenter

## URL
> this sections talks about the url and stuff about request/response

1. GET: /
  - returns a bunch of posts

  - parameters: 
       - sortBy (optional) - it accepts the value of either "asc" or "dsc" to sort the posts by date. 
       - proximity (optional) it accepts the lat and lng to find the posts that are nearby.
       - you should be able to pass these parameter in the url or as a json payload
2. GET: /post/{id}
   - the ID is the ID of the post. it will return the post with that ID if it exists
2. GET: /comment/{id}
   - the ID is the ID of the post. it will return the comment with that ID if it exists
3. POST: /login
   - allows the person to login or register
   
   - payload takes in a JSON with the structure: { username, password }
