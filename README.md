# basic_ionic_cap_ang_project

Super minimal project
Following Your First Ionic App: Angular (https://ionicframework.com/docs/angular/your-first-app), but without the added features of photos etc.

### Steps Followed

### Install Ionic Tooling
`$ npm install -g @ionic/cli native-run cordova-res`

### Create an App
```
$ ionic start photo-gallery tabs --type=angular --capacitor
$ cd photo-gallery
```

### Add OneSignal
`$ npm install onesignal-cordova-plugin`

### Modify /src/app/app.component.ts
Add `import OneSignal from 'onesignal-cordova-plugin';`

Add `OneSignal.setAppId("YOU_APP_ID_HERE");`

### Run on Android
```
$ ionic build
$ ionic cap add android
$ ionic cap copy
$ ionic cap sync

$ ionic cap open android
```

Run in Android Studio or use CLI `$ ionic cap run android`
