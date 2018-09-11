# real-time-dashboard-v1

An example of a real-time dashboard using Socket.IO and Node.

##Running
- npm install (or sudo npm install)
- npm start


##Overall architecture:

###Server Side:
- a Node app that uses Express only to host static files for the front-end (the dashboard html/css/js files)
- a FakeEmitter that emits random data to be rendered in the dashboard

###Client Side:
- an index.html which contains the html and javascript for the dashboard. 
Uses socket.io client to connect to the Node app and setups and updates some dashboard widgets rendered using D3.js

