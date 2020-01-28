#  IONIC-ANGULAR INSTALLATION AND SETTINGS
> Steps to follow to make full installation

* Create your project folder on your desktop  e.g bulb-project
* Open your project folder in VS-Code
* Open a Bash terminal in VS-Code with your project still opened in VS-Code
* Type this command in the terminal:

```Bash npm

npm install ionic

```

* You can type the below command to get infos about Ionic 

```
./node_modules/.bin/ionic

```
* Type the command below to start your project

```

./node_modules/.bin/ionic start

```
> Note: If the Ionic project doesn't start, close the terminals and open a new terminal
> Add your project name e.g bulb and select the Angular Framework. Here my project name is bulb

* Type this code below to enter into the project you just created

```
cd ./bulb

```
* Type

```npm command to show if project compiled successfully

npm start

```
* Open your project with this command

```npm command to show if project compiled successfully

npm run ng serve

```
> Note: The above command opens your project in a browser but with webpack-dev-server in the url
> You can delete the webpack-dev-server part of the url so you can be in home url

* Add Ionic as a dependency in the package.json file with this command

```
npm i ionic --save-dev
```
* click and open the package.json file and under the scripts tab, add the following:

```
"ionic": "ionic"
```
* Type this command to re-open your project in a browser

```
npm run ionic serve
```

> Note, if you prefer starting your project with npm start command then do this

* Open package.json file and under the scripts tab change the "start" contents to:

```
"start": "ionic serve"
```
* Test your configuration by using the npm command to open your project as follows:

```npm
npm start
```
* Type the code below to start building an android project

```
npm run ionic cordova prepare android
```
> Note, if the above code shows error that cordova is not recognised then install cordova as shown below

* Type this in your terminal

```
npm install cordova --save-dev
```
* After the installation of cordova, retype this code below

```
npm run ionic cordova prepare android
```

* Click and open the config.xml file and change the Id of the Widget tag to match your project
> e.g io.cindy.bulb   Here, cindy is the owner of the project and bulb is the project name.

* Type the below code to select a device for the project

```
npm run ionic cordova run android --device
```
> Note, if the above code shows a native-run error then execute this next command else skip it

```
npm i native-run --save-dev
```

* After runnung the native-run command, Run the below command

```
npm run ionic cordova run android --device
```

## After installation, clean up your project by doing these below

* Click on src -> app and then delete app-routing-module.ts
* Click on src->app and then delete the home folder
* Open app.module.ts and delete the import of app-routing-module
* in app.module.ts, under @NgModule, under imports tab, delete the appRoutingModule
* Open app.component.html and delete its content and type your own texts e.g Hello Kingsley

> Note: DO NOT TOUCH app.component.ts file




