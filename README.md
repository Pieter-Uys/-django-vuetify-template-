## Django Vuetify Template ✌️ 🐍

<img src="/src/assets/readme.png">

This template has been forked from  https://github.com/Alhakem/django-vuetify-template and has been updated to use the latest version of vue and vuetify with django 2.2.15 with NPM instead of yarn to be used in a Django and Vuetify application, you can start your next awesome project from here too!  

# Whats new?
```
Updated all the depenencies

"axios": "^0.19.2",
"core-js": "^3.6.5",
"js-cookie": "^2.2.1",
"register-service-worker": "^1.7.1",
"roboto-fontface": "*",
"vue": "^2.6.11",
"vue-router": "^3.2.0",
"vuetify": "^2.2.11",
"vuex": "^3.4.0"

Swapped yarn out for NPM
```

# Future plans

I am planning to make a docker container of this later on for ease of use.

## *Note I am still busy updating it and will make more changes with time (See this as an Aplha version)

## Project setup for Vue (NPM Side)
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

## Project setup for Vue (Django Side)

NB !!! python 3.6 is required!!!
```
 pipenv install --python 3.6 --dev & pipenv shell 
```
(Alternatively, you can use virtualenv)  
```
python manage.py migrate
```

## To run this instance do the following

## To start django 
Make sure you have all the python requirements installed in the requirements.txt
cd into the directory and activate the virtual env shell
```
pipenv shell
```
```
python manage.py runserver
```

## To start node server

```
npm run serve
```
The Vuejs application will be served from localhost:8080 and the Django Api and static files will be served from localhost:8000.

The dual dev server setup allows you to take advantage of webpack's development server with hot module replacement. Proxy config in vue.config.js is used to route the requests back to django's Api on port 8000.

If you would rather run a single dev server, you can run Django's development server only on :8000, but you have to build build the Vue app first and the page will not reload on changes.

## Deployement

I have not yet deployed this updated version, please refer to the forked repo's readme https://github.com/Alhakem/django-vuetify-template/blob/master/README.md

When I do, I will update this section.


Credit to https://github.com/Alhakem for making this

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
