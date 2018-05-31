## Setup for all platforms

You need to [set up the cordova development environment](https://cordova.apache.org/docs/en/latest/guide/cli/index.html) beforehand.

1. [Install the Requirements](https://cordova.apache.org/docs/en/latest/guide/platforms/android/index.html#installing-the-requirements)
2. Install cordova
```sh
$ npm install -g cordova
```
3. Check the requirements
```sh
$ cordova requirements
```
4. Install Vue CLI
```sh
$ npm install -g @vue/cli
```

Then create your project.

```sh
$ vue create my-project   # create your vue project. install @vue/cli if you haven't.
$ cd my-project
$ vue add cordova         # add vue-cli-pugin-cordova and invoke it
$ npm run cordova-build   # make sure you can build your project 
$ cordova prepare         # prepare cordova resources
```

## Browser Platform

#### Start development
```sh
$ npm run cordova-serve
# open http://localhost:8080
```

#### Production Build
```sh
$ npm run corodva-build
$ cordova build browser
# The `platforms/browser/www` directory is ready to deployed.
``` 

## iOS Platform
- Your app runs on the WKWebview. This feature is provided by [cordova-plugin-ionic-webview](https://github.com/ionic-team/cordova-plugin-ionic-webview).

#### Start development
```sh
$ npm run cordova-serve

# in another tab
$ cordova run ios
```

#### Production Build
```sh
$ npm run corodva-build
$ cordova build ios
```

## Android Platform

#### Start development
```sh
$ npm run cordova-serve

# in another tab
$ cordova run android
```

#### Production Build
```sh
$ npm run corodva-build
$ cordova build android
```
