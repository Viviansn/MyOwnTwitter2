MyOwnTwitter2 implements a message sharing application. Users login into the system to post messages, and then other users can see all the stream of messages.

There are two versions of the app, each one on a different branch:

**Firebase branch:**

Authentication, authorization, and persistence for Users and Messages is implemented with Firebase (https://firebase.google.com/). The app implements push updates whenever there is a change in the dataset.
To make this version work, you need to add your own google-services.json file to the app module. Without it, the mobile app will not connect to Firebase

**Room branch:**

Persistence for Users and Messages is implemented with Room (https://developer.android.com/topic/libraries/architecture/room.html) so there is no "message sharing" yet. However, this is still a good example of how implement data persistence with Room (and SQLite)

** Master branch:**
Currently receives patches from the firebase branch.

Known issues:

- ~~The ListView on the MessagesActivity does not properly refresh/update after the user enters a new message~~
- Serveral Error checkings are missing. Most of them are described as TODO.
 

