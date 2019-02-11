# stream_react-redux

React application that allows users to create or join a live stream video.

- #### Libraries used:

  - [react](https://reactjs.org/) to build the user interface.
  - [redux](https://redux.js.org/) to manage the application state.
  - [react-redux](https://github.com/reduxjs/react-redux) to connect redux to the react app.
  - [redux-thunk](https://github.com/reduxjs/redux-thunk), redux middleware to handle async actions.
  - [redux-form](https://github.com/erikras/redux-form/) to manage the form state in Redux.
  - [react-router-dom](https://github.com/ReactTraining/react-router/tree/master/packages/react-router-dom) to handle routings in our app.
  - [flv.js](https://github.com/Bilibili/flv.js/) to display a Flash VideoPlayer.

* #### Design:

  - [semantic-ui](https://semantic-ui.com/) for the overall app design.

* #### Back-end:

  - [axios](https://github.com/axios/axios) to perform HTTP requests.
  - [server-json](https://github.com/typicode/json-server) to create a fake REST API.
  - [node-media-server](https://github.com/illuspas/Node-Media-Server) for implementation of RTMP-FLV media server.

## Application functionalities:

- **Social login** with Google.
- **Create**, **edit**, **delete** and **join** streams.

## Usage:

- Install [OBS](https://obsproject.com/) (Open Broadcaster Software).
- Clone project in a new directory.
- Install packages of the 3 folders: api, client and rtmpserver.
- In each folder run: npm start.
- In your browser, navigate to the react app and log in using google authentication.
- Create a new stream with a title and an description.
- Join the stream and copy the stream id.
- Create a new scene in OBS (Open Broadcaster Software).
- In settings navigate to the Stream tab.
- Select Custom Streaming Server with url: rtmp://localhost/live and the ID copied in the react app.
- In the main screen of OBS click on "Start Streaming".
- Voilà! The live stream should appear in the react app.
