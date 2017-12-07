[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

# FireStarter - Angular + Firebase Progressive Web App

An Angular PWA starter powered by Firebase and Angular. 

- [Live Demo](https://firestarter-96e46.firebaseapp.com/)

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
- [ ] Firebase Cloud Functions (resize images)

*Functionality*

- [ ] Firebase Auth (login with Facebook, Google or email) 
- [ ] Expanded user profiles with custom data in Firestore
- [ ] Access camera or phone storage => Upload files to Firebase Storage
- [ ] Google Maps support and "use my location"


*Additional*

- [ ] Routing
- [ ] Auth guards for relevant sections
- [ ] CRUD for example entity types E.g. venue + event 
- [ ] Listing for example entity type
- [ ] Details view for example entity types
- [ ] Filters for example entity types
- [ ] Basic search
- [ ] Basic pagination and/or infinite scroll

*Views*

- [ ] Login/Registration
- [ ] User profile 
- [ ] Settings
- [ ] Home screen: "Social update feed" (posts with user profile details e.g. profile image, user name, date added)
- [ ] Event Listing
- [ ] Event Details
- [ ] Venue Listing
- [ ] Venue Details

*Nice to have*

- [ ] Like feature
- [ ] Follow feature
- [ ] Add to Favourite
- [ ] Social sharing

## Usage

Create an account at https://firebase.google.com/

- `git clone https://github.com/lifeonlars/angular-firestarter.git firestarter`
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

