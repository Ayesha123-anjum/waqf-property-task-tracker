# PerfAi-Assignment
Waqf Property Task Tracker

## Project Overview

A simple application to help Waqf property managers track basic tasks
related to property management.

<i>Tags - </i> #node #express #monogdb #react

## 

## Installation

Clone the repository from GitHub repo <a href="https://github.com/codewithfaizan/PerfAi-Assignment"> PerfAi-Assignment </a>. <b> Note : This Application requires a .env file containing mongodb srv string follow below </b>

```bash
git clone git@github.com:codewithfaizan/PerfAi-Assignment.git
```
Install the dependencies
```bash
// Same in client & server
npm i 
```
Create a .env file
```bash
touch .env
```
Copy paste the script inside the .env file and Add the mongoDB srv string

```bash
// .env
PORT = 3000
MONGODB_SRV=
```
<p>code for generating secret-key - </p>
## Development
### server
```bash
Start the server
```bash
nodemon app.js
```
### client
```bash
Start the server
```bash
npm run dev
```


## Features
### Authentication
- Session-based authentication is a stateful authentication technique where we use sessions to keep track of the authenticated user.
- User submits the login request for authentication.
- Server validates the credentials. If the credentials are valid, the server initiates a session and stores some information about the client
- Client saves the session id in a cookie and this cookie is sent to the server in each request made after the authentication.
- Server, upon receiving a request, checks if the session id is present in the request and uses this session id to get information about the client.

### Rate limiting
- Rate limiting and slow-down mechanisms help maintain the stability, security, and performance of web applications.
- These controls prevent overloading systems and offer a level of protection against brute force and Distributed Denial of Service (DDoS) attacks.
- express-rate-limit package is used to help handle high traffic.


## API Endpoints 
<h4>Public</h4>

<ul> 
<li>POST /api/auth/signup: create a new user account.</li>
<li>POST /api/auth/login: log in to an existing user account and receive an access token.</li>
<li>POST /auth/signup   : create a new user account.</li>
<li>POST /auth/login    : log in to an existing user account and receive an access token.</li>
<li>GET /auth/profile  : Profile. </li>
</ul>
<h4>Notes  Endpoints</h4>
<h4>Property  Endpoints</h4>
<ul>
<li>GET /api/notes: get a list of all notes for the authenticated user.</li>
<li>GET /api/notes/:id: get a note by ID for the authenticated user.</li>
<li>POST /api/notes: create a new note for the authenticated user.</li>
<li>PUT /api/notes/:id: update an existing note by ID for the authenticated user.</li>
<li>DELETE /api/notes/:id: delete a note by ID for the authenticated user.</li>
<li>POST /api/notes/:id/share: share a note with another user for the authenticated user.</li>
<li>GET /api/search?q=:query: search for notes based on keywords for the authenticated user.</li>
<li>POST /auth/property/add    : create a property for authenticated user.</li>
<li>GET /auth/property/all     : get all properties authenticated user.</li>
<li>GET /auth/property/:id     : get a property by id.</li>
<li>DELETE /auth/property/:id  : delete a property by id.</li>
  
<li>POST /auth/task/add        : Add a task for the propert object.</li>
<li>GET /auth/task/getall      : get all tasks list</li>
<li>PATCH auth/task/update/:id : Update the status.</li>
</ul>

## Npm packages used and their usage

