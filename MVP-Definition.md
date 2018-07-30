[warning]: https://cdn.proxer.me/f/hYVIoAVi "Team participation needed"

### If you see the following, team input is welcome: ![alt text][warning]

### Our MVP consists of the following parts:

- Landing Page
- Sign up / Login form
- Notes Page
- API
- Mobile Apps

# Sign up / Login routes (API)

- Routes for handling user authentication should be completed
- Both routes should return an authentication token which will be included in all other requests to verify users

# Landing Page (est. 17.08)

- The user should be able to log into his own notes very fast → further in login form
- Contact button on top to enable quick contact
- The user can find a description of the service and compelling arguments for using it, together with pictures
- The user should be able to find a Team part, where the dev team is listed.
- A contact part should exist

# Sign up / Login Form (est. 24.08)

- The user should be able to sign in and login with google, facebook, github and normal email/passwort combo
- We will use json webtoking but will probably still inform people that we are using those (the aknowledgement should be saved for the user)
- remember me feature (should just be enabled by standard for convinience, not necessary to ask)
- The user has to comply with terms and agreements to use the service

# Notes Page (est. 07.09)

- ### Navbar
- Contains a search bar, which search for any mention of the input text in the notes, also in the note body
- new note button, which opens a modal where you can create a new note, it contains all the stuff which a note contains (will be explained later)
- view icon, depending whether we find a good and purposful additional layout for notes
- archive icon, you can click on it to see your archived notes, can drag to the symbol to archive
- delete, drag note to the symbol to delete
- ### New note modal
- also doubles as edit note modal, is the same as the hover state of the note ui wise, just with the addition of the last edited date on it
- every time its closed the new state/note is being saved. 
- ### Note
- contains header and body
- contains ui: 
- color selection for the background of the note, is the categorization
- easy access to list making, needs some clue as how to stop making a note, generally needs some ui for lists, so that you can easily cross away the done stuff
- copy icon, makes a double of the note, maybe with -copy in the title
- archive icon to archive the note
- delete icon to delete the note
-share icon, which copies the note into users board, formatted
- Note should be selectable to delete more than one note
- a note should be pinnable to see it faster
- a note should be draggable to change their position, also on mobile

# Mobile APPs (est. 30.09)

- The user should contain all features of the browser version
