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
- Step 1: `Clone this repository`:

```
git clone https://github.com/HBIbidunni/Shortlinkify.git

```
- Step 2: `Navigate to the project directory`: 

```
cd Shortlinkify

```
- Step 3: `Install dependencies`: 

```
npm i express mongoose ejs

``` 

## Configuration
- Step 1: __Create a MongoDB database__.

- Update the `mongoose.connect` method in __server.js__ with the __MongoDB__ connection string:

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
