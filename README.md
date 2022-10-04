# Simple User API

This is a basic CRUD app using Express.

## How It's Made:

Set up the server with Express

```
const express = require('express');
const app = express();
app.listen(3000, () => console.log('YAY server is up and runniong on 3000'));
```

Come up with some random users data

```
let users = {
    <!--  -->
}
```

Serving up static HTML page on home route

```
app.get('/', (req, res)=> {
    res.sendFile(_dirname +'/index.html')
})
```

Respond with a singler user data when users search for a name, and display the data on static page

```
app.get('/api/:name', (req, res) => {
    res.json(object)
}
```

    Listen to click event on main.js

Last, upload codes to Github and Heroku

```
heroku login -i
heroku create random-user-api
echo "web: node server.js" > Procfile
git add .
git commit -m "changes"
git push heroku main
```

## How to Install and Run the Project

clone the repository
install depedencies:

`npm install`

**Tech used:** JavaScript, Express, nodemon, Github, Heroku

## Lessons Learned:

Writing my owe API and make it work on Heroku is awesome!!

This project only provides the API data, I didn't build a front-end to render the data.

## Examples:

Take a look at these couple examples that I have in my own portfolio:

**Palettable:** https://github.com/alecortega/palettable

**Twitter Battle:** https://github.com/alecortega/twitter-battle

**Patch Panel:** https://github.com/alecortega/patch-panel
