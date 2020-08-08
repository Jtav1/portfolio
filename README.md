# portfolio

Just a simple home page website.

## Project setup
```
npm install
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

### Docker commands (For Justin's reference until I set up a proper CI/CD pipeline)
 docker build command:
 ```
 sudo docker build --tag justintavares-web/latest ./
 ```

 docker run command: 
 ```
 sudo docker run --publish 8080:80 --detach --name justintavares-web justintavares-web/latest
 ```