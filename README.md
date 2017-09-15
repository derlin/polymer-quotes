# \<quotes\>

Store your quotes on firebase: [https://derlin-quotes.firebaseapp.com](https://derlin-quotes.firebaseapp.com)

This is a simple PWA (_Progressive Web App_) built with Polymer. It is integrated with firebase (using a Google authentication mecanism) and may be "installed" on the homescreen of an Android device.

# Setup

## Clone the repo

```
git clone https://github.com/derlin/polymer-quotes
cd polymer-quotes
```

## Install dependencies

The application uses `npm` and `bower`. To install everything, run:
```
npm install
bower install
```

## Link with firebase

Install firebase locally (use `-g` to install it system-wide):
```
npm install firebase-tools
```

Run the `init` command:

```
./node_modules/firebase-tools/bin/firebase init
```

It will ask you a lot of things. You need the following features (_Which Firebase CLI features do you want to setup for this folder?_): 
 * Database: Deploy Firebase Realtime Database Rules
 * Hosting: Configure and deploy Firebase Hosting sites

Then, use the default options and answer NO to all _overwrite_ prompt.

# Run and deploy

## Run locally

This project uses _gulp_. Run locally for testing using:

```
gulp serve
```

## Deploy to Firebase

To deploy to firebase, run:

```
./node_modules/firebase-tools/bin/firebase deploy
```