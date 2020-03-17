# Budget-Tracker

## Project Description 

An application utilizing local storage DBs to track budgets whether online or offline, through the use of MongoDB/Mongoose and IndexedDB.

## Table of Contents 

1. [Installations & Dependencies](##Installations-And-Dependencies)

2. [Usage](##Usage) 

3. [Additional Contributors](##Additional-Contributors)

4. [Licensing](##License) 

5. [Testing](##Testing)

## Installations and Dependencies 

1. Compression - compresses images/code to increase performance
2. Express - server technology to save to the database
3. lite-server - development-only fallback server tech
4. Mongoose - ODM library for MongoDB
5. Morgan - provides additional logging metrics for debugging and performance

## Usage 

> IMPORTANT: Please ensure that all node modules have been installed in the local directory. Installation of MongoDB is required to use this program.

After proper installations and setup, begin the server through node.js (">node server.js") within the local directory. This application will allow the user to save deposits and expenses through the interface, which will be displayed as a continuous graph on the screen based on total budget (deposits minus expenses). These entries will also be saved to the database through Mongoose, and can be viewed through the MongoDB CLI. When offline, the application will still function as well as track the budget through the graph - however, new entries will be saved to the IndexedDB and not Mongoose, and can instead be viewed through the Developer Tools -> Application -> IndexedDB -> pending (be sure to refresh 'pending' upon entry). When returning online, the IndexedDB will empty and the entries will then populate MongoDB. As such, this application can be used regardless of the user's online status.

## Additional Contributors 

N/A

## License 

N/A

## Testing 

N/A
