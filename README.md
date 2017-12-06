[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

# FireStarter - Angular + Firebase Progressive Web App

FireStarter is a basic Angular PWA powered by Firebase. It can serve as a foundation to learn this stack and roll out more complex features.

- [Live Demo](https://firestarter-96e46.firebaseapp.com/)
- [Lessons and Screencasts](https://angularfirebase.com)
- [Join the Slack Team](https://join.slack.com/t/angularfirebase/shared_invite/enQtMjU2OTU5OTMyODM3LWU4YTZiMGFhZjJhYmEwYzI1MWFmYTgyMWRmOTI5NWZjYWE3NTMwZjFmNWMwZGI1MmMzODQ3OTFlZjFkMjc5N2Y)

## Features (current)

- Angular 5.0
- 100 PWA Lighthouse Score
- Firebase Auth with Custom Data in Firestore
- CRUD Demos (Firestore & Realtime DB)
- File Uploads to Firebase Storage Demo

## Wishlist (TODO)

- [x] Angular 5.0
- [ ] Angular Cli
- [ ] Angular Material
- [ ] PWA Support (service worker + app manifest)
- [ ] Firebase Firestore (ideally using AngularFire)
- [ ] NgRX for state management

*Functionality*

- [ ] Firebase Auth (login with Facebook, Google or email) 
- [ ] Expanded user profiles with custom data in Firestore
- [ ] Access camera or phone storage => Upload files to Firebase Storage
- [ ] Google Maps support and "use my location"

*Additional*

- [ ] Routing examples
- [ ] Auth guards for relevant sections
- [ ] CRUD for basic entity type(s) (e.g. entry,destination,location,product,post)
- [ ] Listing for basic entity type
- [ ] Filters for basic entity type
- [ ] "Social update feed"
- [ ] Basic search
- [ ] Basic pagination 
- [ ] Infinite scroll 



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

