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

*Stack*

- [x] Angular 5.0 + Angular Cli
- [ ] Angular Material
- [ ] PWA Support (service worker + app manifest)
- [ ] Firebase Firestore + AngularFire
- [ ] NgRX for state management
- [ ] Firebase Cloud Functions (resize images)
- [ ] Firebase Hosting (`firebase deploy`)
- [ ] AOT + PRPL pattern
- [ ] Angular Universal
- [ ] Unit Testing + BDD using Jasmine & Karma

*Functionality*

- [ ] Firebase Auth (login with Facebook, Google or email) 
- [ ] Expanded user profiles with custom data in Firestore
- [ ] Access camera or phone storage => Upload files to Firebase Storage
- [ ] Google Maps support and "use my location"
 
*Core features*

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
- [ ] Map with nearby events/venues (near me)


*Nice to have*

- Like feature
- Follow feature
- Add to Favourite
- Social sharing
- User Reviews

## Aim to cover the following core concepts

 - Ability to add and edit entities in Firestore
 - Ability to link entities in Firestore e.g. linking an event to a venue and automatically duplicate the data in both collections
 - Ensure data is kept in sync across collections when editing
 - Structure data in Firestore to take advantage of shallow queries for entity list view vs. entity details view
 - Implement best practice Material Design components via Angular Material
 - Best practice Angular form implementation whilst allowing for easy modififaction/extension
 - 

## Usage

Create an account at https://firebase.google.com/

- Enable authentication with email, Google and Facebook via console => Authentication => Sign in method
- Enable Firestore under console => Database
- Set database permissions to enable read/write access for authenticated users

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

