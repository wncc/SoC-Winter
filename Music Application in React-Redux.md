# Music Application in React-Redux

## Week 1: Induction Week (Getting started)
This week would be an introduction to react and redux and any other libraries that might be used in the final project.

### Day 1: Basic introduction of React
React is an open-source, front end, JavaScript library for building user interfaces or UI components. To start with, make sure to have React installed in your machines. You can follow [this](https://reactjs.org/docs/create-a-new-react-app.html#create-react-app) simple tutorial to do so. 

If you’re a complete beginner in React, you can refer to the following YouTube videos. They’re a little long but good to get you started with it. And if you know Angular already, then it’ll be much easier for you to pick this up as well.
- [React Tutorial for Beginners by Mosh](https://www.youtube.com/watch?v=Ke90Tje7VS0) 
- [React Playlist](https://www.youtube.com/watch?v=QFaFIcGhPoM&list=PLC3y8-rFHvwgg3vaYJgHGnModB54rxOk3)

You can choose to watch any of these or both as well. Just remember to code alongside else the concepts will run away from your mind.

### Day 2: More robust introduction about React + First React application
React undoubtedly has one of the best documentations and thus proves to be its best learning source. All the important concepts are explained in a coherent manner. Try coding alongside for better understanding. Follow all the blogs in the [“Main Concepts”](https://reactjs.org/docs/hello-world.html) sections to get a full grasp of the concepts.

We suggest doing [this tutorial](https://reactjs.org/tutorial/tutorial.html) to build your first react application! 

### Day 3: React Bootstrap and SCSS
React-Bootstrap replaces the Bootstrap JavaScript. Each component has been built from scratch as a true React component. It has evolved and grown alongside React, making it an excellent choice as your UI foundation. It’s [documentation](https://react-bootstrap.github.io/) is the best source to learn React-Bootstrap.

To install React-Bootstrap in your React application, run the following simple command in your terminal inside your React project. 

`npm install react-bootstrap bootstrap`

Have a look at [this introduction](https://react-bootstrap.github.io/getting-started/introduction/) to get started with its usage. The best thing about using React-Bootstrap in your application is its [Grid System](https://react-bootstrap.github.io/layout/grid/) that uses flexbox as its base.

It is also advised to use [SCSS](https://sass-lang.com/) instead of CSS along with this project. It is very similar to CSS and very quick to learn. 

### Day 4: Learning Redux and its integration with React
Redux is an open-source JavaScript library for managing application state and is used along with React for building the UI screens. You can install Redux following [this link](https://redux.js.org/introduction/getting-started#installation).
The key to understanding Redux is understanding State, Reducers and Actions. Begin with [this tutorial](https://youtu.be/poQXNp9ItL4) and try coding alongside (skip the portions you already know).

Since, Redux is also well documented, it is advised to follow either of these tutorial to learn Redux:
- [Redux Essentials, Part 1: Redux Overview and Concepts](https://redux.js.org/tutorials/essentials/part-1-overview-concepts)
- [Redux Fundamentals, Part 1: Redux Overview](https://redux.js.org/tutorials/fundamentals/part-1-overview)

### Day 5: More Redux and Api integration using axios
These are some additional resources to learn Redux, since it is not easy to grasp Redux at first go.
- [React Redux Tutorials - 1 - Introduction](https://www.youtube.com/watch?v=9boMnm5X9ak&list=PLC3y8-rFHvwheJHvseC3I0HuYI2f46oAK)
- [Redux Crash Course With React](https://www.youtube.com/watch?v=93p3LxR9xfM)  

*Axios* is a popular, promise-based HTTP client that sports an easy-to-use API and can be used in both the browser and Node. js. It is usually easy to use Axios for backend integration in React. 

Make sure to install axios on your machine, using [this link](https://www.npmjs.com/package/axios#installing). 
This is a good tutorial to learn how to use axios: [How to make HTTP requests like a pro with Axios](https://blog.logrocket.com/how-to-make-http-requests-like-a-pro-with-axios/). It is usually easy to learn, so this might suffice. If you still have some doubts, do read the [documentation](https://www.npmjs.com/package/axios) or watch this [Axios Crash Course | HTTP Library tutorial](https://youtu.be/6LyagkoRWYA). 

## Week 2: Final Project
This week would be all about implementing everything learnt to make the final application. There are a lot of video tutorials available online for designing a music application in React. However, it is recommended that initially you should try on your own and then look for the tutorials if stuck.

### Getting Started
Read these tutorials to get started with what the actual project would look like and what you would need to do. Please don't try finding the source code as that'll be very easily avaible on GitHub or elsewhere.
- [Tutorial 1](https://www.creativebloq.com/how-to/build-a-simple-music-player-with-react)
- [Tutorial 2](https://medium.com/@anuragbhattacharjee/diy-music-player-with-react-js-309d63cfbcba)

### UI Designing 
Start with designing the UI of the application. Either take inspiration from the [Spotify](https://www.spotify.com/) or try designing your own in [Figma](https://www.figma.com/). Have a look at the image below for some ideation. 

![Music Player](https://reactnativeexample.com/content/images/2019/07/React-Native-Music-App.jpg)

### API Integration
The most famous API used while designing music applications is the [Spotify API](https://developer.spotify.com/documentation/web-api/). You can axios for calling the api and integrating with the application.

### Folder Structure
Keep in mind the folder structure to follow during implementing the application. It would be very useful later on when you design larger applications, so it is good to incorporate at an earlier stage as well.
- Keep all the reusable components in one folder called components.
- Make one folder for all the views (or pages) in your application.
- For all the Redux work, keep one folder and then make sub folders like action, reducers and store. 

### Resources
These are some of the tutorials that you can follow to implement the application, all of these are complete on their own and you can follow any of these to make the project. There are a lot of other video tutorials which can easily be found online, so do search if these don't seem sufficient.
- [Build a Spotify Clone with REACT JS for Beginners](https://youtu.be/pnkuI8KXW_8)
- [Build a MUSIC app in REACT JS #1](https://youtu.be/3ourkSxbd0Y) and [Build a Music app in REACT JS #2](https://youtu.be/M4TTeSVX3HI) 
