<div align="center"><h1>ShortLinikiFy</h1></div>

------------------------

<div align="center">
<img src="https://i.imgur.com/0iXMDac.jpg" alt="My Shortlinkify Design">
</div>

## __Overview__

This Single Paged __URL Shortener project__ is designed to provide a simple and efficient way to __shorten long URLs__ into __concise, easy-to-share links__. 
The application is built using [__Node.js__, __MongoDB__, __Express.js__ and __EJS__ for the view engine],
and it offers a user-friendly interface for __shortening URLs__ and __managing shortened links__.

__Features__
- `URL Shortening`: Easily shorten long URLs to create compact and shareable links.
- `Custom Short URLs`: Optionally customize the short URL for easy memorization.
- `Link Management`: View or delete shortened links for better control.
- `Analytics`: Track basic analytics such as click count for each shortened link.
- `Dark Mode`: Toggle between light and dark mode for a personalized viewing experience.
- `User-Friendly Interface`: A clean and intuitive user interface for easy navigation.

## Prerequisites
Before running the application, the following must be installed:
- `Node.js`
- `MongoDB`

## Installation
- Step 1: __Clone this repository__:

```
git clone https://github.com/HBIbidunni/Shortlinkify.git

```
- Step 2: __Navigate to the project directory__: 

```
cd Shortlinkify

```
- Step 3: __Install dependencies__: 

```
npm i express mongoose ejs

``` 

## Configuration
- Step 1: __Create a MongoDB database__.

- Update the __mongoose.connect__ method in __server.js__ with the __MongoDB__ connection string:

```
mongoose.connect('your-mongodb-connection-string', {
  useNewUrlParser: true,
  useUnifiedTopology: true
});

```

## Usage
- Step 1: __Start the server__:

```
npm run devStart

```

This command runs the server using nodemon for automatic reloading during development.

- Step 2: Open your browser and __go to http://localhost:3000/__ to access ShortLinkiFy.


## Application Structure

- __index.ejs__: The main HTML template file containing the structure and styling of the web application.

- __shortUrl.js__: Defines the Mongoose schema for the ShortUrl model used to interact with the MongoDB database.

- __package.json__: Specifies project details, dependencies, and scripts for running the application.

- __server.js__: The main server file that sets up the Express application, defines routes, and connects to the database.



## Detailed Explanation of the Application Structure

This breakdown provides a comprehensive understanding of the ShortLinkiFy project, 
covering its frontend structure, backend data schema, project configuration, and server setup. 
Each component contributes to the functionality and appearance of the Single Paged URL shortener application.


1) `package.json`

This file contains metadata about the project and its dependencies.

- Specifies the name and version of the project.

- Defines a development script (`devStart`) using nodemon to auto-restart the server during development.

- Lists the project's runtime dependencies, including `Express`, `EJS`, `Mongoose`, and `ShortId`.

- Lists development dependencies, including nodemon for automatic server restarts.


2) `server.js`

 This is the main server file responsible for setting up the Express application, defining routes, and connecting to the MongoDB database.

- Imports required libraries, including Express, Mongoose, and the ShortUrl model.

- Express Setup: Configures the Express app with EJS as the view engine.

- Enables parsing of URL-encoded data.

- Defines routes for handling homepage requests, URL shortening submissions, URL deletion requests, and short URL redirection.

- Connects to the MongoDB database using Mongoose.

- Specifies the port to listen on and starts the server.


3) `index.ejs`

This file is the main HTML template for the ShortLinkiFy web application. 
It uses the __EJS templating engine__ for dynamic content rendering. Its key components:

- HTML Structure:

<html>, <head>, and <body> tags define the basic HTML structure.
<meta> tags set character encoding, viewport settings, and compatibility.
External stylesheets are linked for Bootstrap and local styling.

- Styles:

The <style> block contains custom CSS for light and dark modes, a toggle button, container styles, table styles, and a navigation bar.
The @keyframes glow rule defines a simple animation for text shadow.

- Title and Navigation:

The <title> tag sets the document title.
The navigation bar contains a link to the home page (#).

- Container and Form:

A container holds the main content. The <h1> tag displays the application name with a gradient background.
A form allows users to submit a URL for shortening.

- Table:

A table displays information about each shortened URL, including the full URL, short URL, clicks, and delete button.

- Scripts:

JavaScript functions for toggling dark mode and confirming delete actions.
A button triggers the dark mode toggle function.


4) `shortUrl.js`

This file defines the Mongoose schema for the ShortUrl model, which represents a shortened URL in the MongoDB database.

- Schema: The schema includes fields for the full URL, short URL (generated using shortId), click count, and an action field.

-Exports: The module exports the Mongoose model based on the schema.


## ShortLinkiFy Demo: Light & Dark Mode

<div>
  <img src="https://i.imgur.com/4F5alEe.jpg" alt="ShortLinkiFy 1" width="400" />
  <img src="https://i.imgur.com/ZUS4z6W.jpg" alt="ShortLinkiFy 2" width="400" />
</div>

<div>  
  <img src="https://i.imgur.com/jsqNO0N.jpg" alt="ShortLinkify 3" width="400" />
  <img src="https://i.imgur.com/W4sUFzh.jpg" alt="ShortLinkiFy 4" width="400" />
</div> 
