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

## *Note I am still busy updating it and will make more changes with time (See this as a Aplha version)

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

## NB !!! python 3.6 is required!!!
```
 pipenv install --python 3.6 --dev & pipenv shell 
```
```
python manage.py migrate
```

## to run this instance do the following

## start django first 

## Make sure you have all the python requirements installed in the requirements.txt

## cd into the directory and activate the virtual env shell
```
pipenv shell
```

```
python manage.py runserver
```

## start node server second

```
npm run serve
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
