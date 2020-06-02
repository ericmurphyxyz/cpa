#!/bin/sh

mkdir $1
cd $1

npm init -y
npm i react react-dom

# Add starter files
echo '<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>React App</title>
  </head>
  <body>
    <div id="root"></div>
    <script src="src/index.js"></script>
  </body>
</html>' >> index.html

mkdir src
echo 'import React from "react";
import ReactDOM from "react-dom";
import App from "./App";

ReactDOM.render(<App />, document.getElementById("root"));' >> src/index.js
echo 'import React from "react";

const App = () => <div>Hello world.</div>;

export default App;' >> src/App.js

# Add start script
sed -i "/scripts/ a\ \ \ \ \"start\": \"parcel index.html\"," package.json

echo "Success! Created $1 at $PWD"
echo -e "Inside that directory, run the \e[36mnpm start\e[0m command to start the development server."
