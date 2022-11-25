# Create (React) Parcel App

Run this script to create a new light-weight starter React App with Parcel.

```sh
cpa new-react-project
```

## Installation

Install Parcel first.

```sh
npm install -g parcel
```

To run the script, give it executable permissions with `chmod`.

```sh
chmod +x cpa
```

You can call the script by adding it as an alias in your shell config file. (e.g. .bashrc or .zshrc)

```zsh
alias cpa="~/path/to/cpa"
```
## Files after first run

```
|-- index.html
|-- node_modules
|   `-- ...
|-- package.json
|-- package-lock.json
`-- src
    |-- App.js
    `-- index.js
```
