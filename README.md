# Unit 11 Express Homework: Note Taker

## Description

I created an application that can be used to write, save, and delete notes. This application will use an express backend and save and retrieve note data from a JSON file.

* The application frontend has already been created, I built the backend and connected the two. 

* The following HTML routes are created:

  * GET `/notes` - Should return the `notes.html` file.

  * GET `*` - Should return the `index.html` file

* The application has a `db.json` file on the backend that that is used to store and retrieve notes using the `fs` module.

* The following API routes are created:

  * GET `/api/notes` -  Reads the `db.json` file and returns all saved notes as JSON.

  * POST `/api/notes` - Receives a new note to save on the request body, add then saves to the `db.json` file, and then returns the new note to the client.

  * DELETE `/api/notes/:id` - Receives a query parameter containing the id of a note to delete. Each note is given a unique id with installing the UUID package. It then reads from 'db.json', removes the note with the given 'id' property and then rewrites the 'db.json' file.  
## Deploying the App

The app wsa successfully deployed to the local server and to Heroku.
- - -

* (GitHub Link- note-taker)[https://github.com/abouelelas/note-taker]
* (Heroku Link- note-taker)[https://peaceful-castle-23554.herokuapp.com/notes.html]

![Screenshot](https://github.com/abouelelas/note-taker/blob/master/public/assets/Notetaker-ss.png)