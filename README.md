# electron-project

## Project setup

Create the project
```
vue create project-name
```
Go into the project
```
cd project-name
```

Install electron
```
npm install electron --save-dev
```

Create a file for electron init and copy the base file from [here](https://www.electronjs.org/docs/tutorial/first-app#_kq6i7iis), or in the electron.js of this repository.
```
touch electron.js
```

Add in the package.json, anywhere
```
"main":"electron.js"
```

Add in the package.json, in the script
```
"electron":"vue-cli-service build; electron ."
```

Add a config file for Vue
```
touch vue.config.js
```

In the file, add
```
module.exports = {
    publicPath: process.env.NODE_ENV = "production" ? "./" : "/"
}
```

Now you can run with
```
npm run electron
```



### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
