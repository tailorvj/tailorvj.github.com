---
published: false
---

## TODOIST is a good example of the new Functional React paradigm

React has gone through a major paradigm shift on February 2019, from classes to functional programming in JS. 

The TODOIST app is a good, simple, example of an app built in a functional way, using React hooks, useState and useEffect. I'm documenting this app as part of my knowledge base for the app prototyping workflow. 

### TODOIST

I wouldn't call it a full Firebase app, because it misses a major element - security rules. I might add them to the project in order to be able to actually use it online. 

I think the Firebase security rules issue is a global issue. I'm actually pondering whether I should build some kind of a general purpose security rules generator for Firebase and specifically Firestore, which is the more scalable type of Firebase database. 

TODOIST has src/firebase.js in its' .gitignore list, therefore, it has to be created manually. Create a src/firebase.js file, add the following to it and then update with your own Firebase settings:

[Gist source](https://gist.github.com/tailorvj/47e1195c294a4e5c03939b4dd7063d12)

  import firebase from 'firebase/app';
  import 'firebase/firestore';

  const firebaseConfig = firebase.initializeApp({
  //create a Firestore database in your Firebase project and 
  //replace only the internal part of this object from your Firebase web settings
      apiKey: "",
      authDomain: "your.firebaseapp.com",
      databaseURL: "https://your.firebaseio.com",
      projectId: "yourprojectid",
      storageBucket: "yourbucket.appspot.com",
      messagingSenderId: "yourmessagingid",
      appId: "yourappid",
      measurementId: "yourmeasurementidforanalytics"
    });

  export {firebaseConfig as firebase};

### Changing git project master.remote origin to my own Github repo without Forking through the Github website

Another thing to note about the TODOIST project. I cloned it from blacksonic from the terminal (originally he forked it from [Karl Hawden](https://github.com/karlhadwen/todoist)), created an empty repo on Github and changed the origin to my own Github repository like this:

  $ git remote rm origin
  $ git remote add origin git@github.com:tailorvj/todoist-firebase-react.git
  $ git config master.remote origin
  $ git config master.merge refs/heads/master

Then I pushed my changes to Github as [tailorvj/todoist-firebase-react](https://github.com/tailorvj/todoist-firebase-react). 

A working example of the app can be found on [https://todoist-74102.firebaseapp.com/](https://todoist-74102.firebaseapp.com/)

I love Firebase and React. I hope you enjoy it too thanks to this documentation. 

Cheers,
Tailor