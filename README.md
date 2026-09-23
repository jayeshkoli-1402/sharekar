# CampusVault v2

A static frontend with Firebase as the shared backend.

## UI
The interface is redesigned around the supplied visual reference:
- warm cream + mint palette
- soft neumorphic/glass panels
- rounded dashboard cards
- compact student-resource dashboard
- folders, activity, library statistics
- responsive mobile layout

## No login
There is no visible login/signup screen. Firebase Anonymous Authentication is used silently only so Firebase can identify each browser session and apply security rules. Students only enter a display name.

## Setup
1. Create a Firebase project.
2. Enable Authentication → Anonymous.
3. Create Firestore and Storage.
4. Register a Web App.
5. Replace the firebaseConfig object in index.html.
6. Deploy firestore.rules and storage.rules.
7. Host index.html on any static host.

No update/delete operations are exposed by the UI, and the included rules explicitly deny them at the backend.
