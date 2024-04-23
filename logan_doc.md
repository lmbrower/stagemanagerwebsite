### How to make changes
Go to our github respository and fork the repository.
* Click [here](https://github.com/Bmfioresi/stage-managers-book)

* In the top-right corner of the page, click Fork.

* Under "Owner," select the dropdown menu and click an owner for the forked repository.

* By default, forks are named the same as their upstream repositories, but you can name it whatever you'd like.

* Optional:
  * in the "Description" field, type a description of your fork.
  * select Copy the DEFAULT branch only.

* Click Create fork.

#### After installing Node.js and npm
Most of our files are split into two main folders: client and server. Client holds the frontend react.js files and server holds the backend node.js files. To make changes, you can simply edit any of the files as you see fit, or create entirely new ones.
To test your changes, open two terminals. Navigate to the client directory in one, and the server directory in the other.

##### Client
In the client terminal, run the command `npm start`. This will start the client on `localhost:3000` and open it in your default browser. If you have dependency issues, run `npm install` and it will automatically install all of the dependencies in `packages.json`.
##### Server
In the server terminal, run the command `npm run dev`. This will start the server on `localhost:8000` and run it in the background. If you have dependency issues, run `npm install` and it will automatically install all of the dependencies in `packages.json`.
You will need to login to MongoDB Atlas, add your computer's IP Address, and create a .env file with variables MONGODB_USERNAME and MONGODB_PASSWORD to facilitate the communication between the server and the database.

### Project backlog and bug lists

#### Backlog
Our project backlog is located [here](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm).

#### Bug list
Major bugs include:
* When you log in, the sidebar does not automatically refresh, which forces the user to refresh the page to join a hub and to view the hubs they are a member of.
* The script viewer only properly displays on Edge, and displays a downloadable file on other browsers.

#### Other potential issues
You will want to refactor to a local mongodb database rather than relying on Atlas.
Styling will need to be refactored to be responsive using Bootstrap.
HIDs and UIDs must be integers; some of our code uses 'Number()' in certain locations because we were originally using strings. May cause unexpected results.