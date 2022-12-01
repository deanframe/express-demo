# Express Demo

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

Clone this repo to your computer - we'll be building a simple REST endpoint!

1. Run `yarn`, and then `yarn start` to start the frontend. You should see a page with two buttons
2. Install `express` with `yarn add express`
3. Install `cors` with `yarn add cors`
4. Create a folder named `server`
5. In the folder, add an `index.js` file with the following:
```
const express = require("express")
const cors = require("cors")

app.use(cors());

const app = express();
const port = 3001;

app.get('/', (req, res) => {
  res.send('Hello World!')
})

app.listen(port, () => {
  console.log(`Express server listening on port ${port}`)
})

```
6. In `package.json`, add the following to the `"scripts"` section: `"start-server": "node server/index.js"`
7. Open a new terminal window and run `yarn`, then `yarn start-server`
8. Visit `localhost:3001` in your browser!
