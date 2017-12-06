[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

# FireStarter - Angular + Firebase Progressive Web App

FireStarter is a basic Angular PWA powered by Firebase. It can serve as a foundation to learn this stack and roll out more complex features.

- [Live Demo](https://firestarter-96e46.firebaseapp.com/)
- [Lessons and Screencasts](https://angularfirebase.com)
- [Join the Slack Team](https://join.slack.com/t/angularfirebase/shared_invite/enQtMjU2OTU5OTMyODM3LWU4YTZiMGFhZjJhYmEwYzI1MWFmYTgyMWRmOTI5NWZjYWE3NTMwZjFmNWMwZGI1MmMzODQ3OTFlZjFkMjc5N2Y)

## Features

- Angular 5.0
- 100 PWA Lighthouse Score
- Firebase Auth with Custom Data in Firestore
- CRUD Demos (Firestore & Realtime DB)
- File Uploads to Firebase Storage Demo

## TODO => Expand

- Angular Material integration
- Expanded user profiles
- Auth guards for certain sections
- Access phone camera + storage
- CRUD for basic entity type (e.g. destination/entry/product or whatever)
- Listing for basic entities 
- Simple filters for entities (e.g. location, category or tag)
- Basic pagination or infinite scroll
- "News Feed" listing
- Google Maps Example (ability to attach to basic entity type)
- Basic search functionality


## Usage

Create an account at https://firebase.google.com/

- `git clone https://github.com/codediodeio/angular-firestarter.git firestarter`
- `cd firestarter`
- `npm install`

Create the environment files below in `src/environments/`.

#### environment.ts
```typescript
export const environment = {
    production: false,
    firebaseConfig: {
        apiKey: 'APIKEY',
        authDomain: 'DEV-APP.firebaseapp.com',
        databaseURL: 'https://DEV-APP.firebaseio.com',
        projectId: 'DEV-APP',
        storageBucket: 'DEV-APP.appspot.com',
        messagingSenderId: '123456789'
    }
};
```
#### environment.prod.ts
```typescript
export const environment = {
    production: true,
    firebaseConfig: {
        // same as above, or use a different firebase project to isolate environments
    }
};
```

And finally `ng serve`

