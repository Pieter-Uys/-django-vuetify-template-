# dashboard

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
