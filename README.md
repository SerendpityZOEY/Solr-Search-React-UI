# Solr Relevant Commit Search

This application uses ReactJS to connect with Solr to search data. Applied Material UI and Materializecss for front-end.

## First Time Setup
If you already have npm and node installed, you can skip this step.
For Ubuntu:
```
$sudo apt-get update
$sudo apt-get install nodejs
$node -v
$sudo apt-get install npm
$npm -v
```
For Mac:
 
1. Open the Terminal app and type `brew install node`.
2. Sit back and wait. Homebrew downloads some files and installs them. And that’s it.

## Running

- Compile:
```
$npm run-script build-app
```

- Run with:
```
$npm start
```

If the browser is not opened automatically, then view the page through this url:
```
localhost:8080
```

## Install dependencies
If you can't run the program, try the following command to install node modules locally.
```
$npm install
```

## Instructions

- The default query is `*:*` to fetch everything from Solr and display first 10 commits.
- For filters, they are set to `all` by default, which will search within `add`, `remove`, `not being modified` fields for either import statements or callsites.
    - Specify add/remove/modify/all from dropdown (optional)
    - eg: type `android.app.Fragment` in imports text field, or type `getId` in callsites field to specify the exact text.
    - Click search.
- *Note*:Methods filter is under developing.

![Screen Shot](docs/ScreenShot.png)

## Deployment
Tool is deployed at http://192.12.243.***:8080/.
