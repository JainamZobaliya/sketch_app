# sketch_app

1. ## Initialized React APP
    Created the react-app without using create-react-app, i.e., `npx create-react-app appName` and made the configurations manually.

    1. ### npm init
        Initialised the project by creating the pacakge.json
    2. ### Installed required package
        Install the following packages:
       1. parcel
           ```sh
           npm install -D parcel
           ```
           `-D` is for Dev Dependency
       2. react
           ```sh
           npm install react
           ```
       3. react-dom
           ```sh
           npm install react-dom
           ```
    3. ### File Setup:
       1. `index.html` - which contains an elemnet with id `root`.
       2. `index.js` - which uses react-dom method to renders HTML.

    4. ### Running the App:
       1. Start the Dev. Server using the below command:
           ```sh
           npx parcel index.html
           ```
       2.  Create the build using the below command:
           ```sh
           npx parcel build index.html
           ```
       3.  Configure the above commands in `scripts` of the `package.json` file:
           ```json
           {
               // ...
               "scripts": {
                   "start": "parcel index.html",
                   "build": "parcel build index.html",
                   // ...
               },
           }
           ```
           Alternatively, we can do like below:
           ```json
           {
               // ...
               "source": "index.html",
               "scripts": {
                   "start": "parcel",
                   "build": "parcel build",
                   // ...
               },
           }
           ```
       > The fileName `index.html`, is the relative or absolute paths or globs of the entry point.