## Django Vuetify Template ✌️ 🐍

<img src="/src/assets/readme.png">

This template has been forked to be used in a Django and Vuetify application, you can start your next awesome project from here too!  


This repo has been forked from https://github.com/Alhakem/django-vuetify-template and updated to use the latest Dependencies as from 2020-08-11 and is still busy updating it so if you find any problems please feel free to reach out. I will do my best to update it as time goes by. I've noticed a one problem with the setup that I will see to

 1 - The CRUD on the django page has an issue with the hot reload. When you add multiple messages and delete one it "Deletes" everything but if you refersh 
    ( Press F5 ) the message that you deleted is gone and the others will show.

Will figure it out and update this in the future. 

Thanks to Mohammed Al-Hakem and Gui Talarico  for creating the original 

* Mohammed Al-Hakem's Github - https://github.com/Alhakem
* Gui Talarico's Github - https://github.com/gtalarico



## What is new in this template
- Updated Dependencies versions.

OLD

```
 "axios": "^0.18.0",
    "vue": "^2.5.17",
    "vue-router": "^3.0.1",
    "vuetify": "^1.3.5",
    "register-service-worker": "^1.0.0"
```

NEW

```
  "@mdi/font": "^3.6.95",
    "axios": "^0.19.2",
    "core-js": "^3.6.5",
    "js-cookie": "^2.2.1",
    "register-service-worker": "^1.7.1",
    "roboto-fontface": "*",
    "vue": "^2.6.11",
    "vue-router": "^3.2.0",
    "vuetify": "^2.2.11",
    "vuex": "^3.4.0"
```


- Updated devDependencies versions.

OLD
```
"@vue/cli-plugin-babel": "^3.0.5",
    "@vue/cli-plugin-eslint": "^3.0.5",
    "@vue/cli-service": "^3.0.5",
    "vue-template-compiler": "^2.5.17",
    "@vue/cli-plugin-pwa": "^3.0.5",
    "stylus": "^0.54.5",
    "stylus-loader": "^3.0.1",
    "vue-cli-plugin-vuetify": "^0.4.5",
    "vuetify-loader": "^1.0.5"
```
NEW

```
    "@vue/cli-plugin-babel": "~4.5.0",
    "@vue/cli-plugin-eslint": "~4.5.0",
    "@vue/cli-plugin-pwa": "~4.5.0",
    "@vue/cli-plugin-router": "~4.5.0",
    "@vue/cli-plugin-vuex": "~4.5.0",
    "@vue/cli-service": "~4.5.0",
    "babel-eslint": "^10.1.0",
    "eslint": "^6.7.2",
    "eslint-plugin-vue": "^6.2.2",
    "sass": "^1.26.5",
    "sass-loader": "^8.0.2",
    "vue-cli-plugin-vuetify": "~2.0.7",
    "vue-template-compiler": "^2.6.11",
    "vuetify-loader": "^1.3.0"
```

- Removed Yarn and Replaced it with NPM

- Added a requirements.txt file

This template is a minimal example for an application using VueJs and Django (RestFramework).

It's setup to have a clear separation: use Vue, NPM, and Webpack to handle all frontend logic and asset bundling,
and use Django and RestFramework to manage a Data Models, Web API, and serve static files.

While it's possible to add endpoints to serve django-rendered html responses, the intention is to use Django primarily for the backend, and have view rendering and routing and handled by Vue + Vue Router as a Single Page Application (SPA).

Out of the box, Django will serve the application entry point (`index.html` + bundled assets) at `/` ,
data at `/api/`, and static files at `/static/`. Django admin panel is also available at `/admin/` and can be extended as needed.

The application templates from Vue Cli `create` and Django `createproject` are kept as close as possible to their
original state, except where a different configuration is needed for better integration of the two frameworks.


### Demo

[Live Demo](https://django-vue-template-demo.herokuapp.com/) 

Note** this is based on the old version and should be used as an example

### Includes

* Django
* Django Restframework
* Django Whitenoise, CDN Ready
* Vue Cli 3
* Vue Router
* Gunicorn
* Configuration for Heroku Deployment


### Template Structure


| Location             |  Content                                   |
|----------------------|--------------------------------------------|
| `/backend`           | Django Project & Backend Config            |
| `/backend/api`       | Django App (`/api`)                        |
| `/src`               | Vue App .                                  |
| `/src/main.js`       | JS Application Entry Point                 |
| `/public/index.html` | Html Application Entry Point (`/`)         |
| `/public/static`     | Static Assets                              |
| `/dist/`             | Bundled Assets Output (generated at `NPM build` |

## Prerequisites

Before getting started you should have the following installed and running:

- [X] NPM - [instructions](https://nodejs.org/en/download/)
- [X] Vue Cli 3 - [instructions](https://cli.vuejs.org/guide/installation.html)
- [X] Python 3.6
- [X] Pipenv

## Setup Template

```
$ git clone https://github.com/gtalarico/django-vue-template
$ cd django-vue
```

Setup
```
$ NPM install
```
## Pipenv installation

If you have a higher version of python 3.6 you will need to install python 3.6 or earlier it will not work on a higher version Eg. python 3.7, 3.8 and above until pipenv is updated to support these versions (not later than 3x) To specify pipenv to use python 3.6 like this.
```
pipenv --python 3.6 install --dev & pipenv shell 
```
```
$ pipenv install --dev & pipenv shell 
$ python manage.py migrate
```

Make sure you are in the same directory as the manage.py script and that your pipenv shell is active
```
$ python manage.py runserver
```

From another tab in the same directory:

```
$ npm run serve
```


 Always make sure the virtualenv is activated before running the following

```
python manage.py runserver 
python manage.py migrate  
```


To activate the pipenv make sure you are in the same directory as the manage.py script and run the following (this is not needed with the above commands but its needed when you close the command line and wish to re-activate it)

```
pipenv shell 
```



## Virtualenv installation

Alternatively you can use virtualenv to run this as well (Depending on your requirements). just make sure you have all the requirements installed in the requirements.txt and you have django version 2.2.15 installed into your virtualenv

* See Virtualenv - [PyPI](https://pypi.org/project/virtualenv/ ) for usage and installation

Cd into the directory where manage.py is then run the following in command line

```
virtualenv venv
```
The above will create a virtual env from the highest version of python installed on your computer

cd into the virtual env and into the Scripts directory under venv

```
cd venv/Scripts
```

activate the virtual env type 'activate' (This will run the activate script and activate your virtualenv)

```
activate 
```

Linux users to activate it  
```
source activate
```

cd back to the directory where manage.py is and install the python requirements from the requirements.txt file

```
pip install -r requirements.txt
```

Make migrations to your django sqllite to create the tables for the CRUD functionality

```
python manage.py migrate
```

Then you can run the django server by typing in the following 

```
python manage.py runserver
```

And the nodejs server from another command line tab

```
 npm run serve
```


The Vuejs application will be served from `localhost:8080` and the Django Api
and static files will be served from `localhost:8000`.

The dual dev server setup allows you to take advantage of
webpack's development server with hot module replacement.
Proxy config in `vue.config.js` is used to route the requests
back to django's Api on port 8000.

If you would rather run a single dev server, you can run Django's
development server only on `:8000`, but you have to build build the Vue app first
and the page will not reload on changes.

```
$ npm run build
$ python manage.py runserver
```


## Deploy

* Set `ALLOWED_HOSTS` on `backend.settings.prod.py`

### Heroku Server

```
$ heroku apps:create django-vue-template-demo
$ heroku git:remote --app django-vue-template-demo
$ heroku buildpacks:add --index 1 heroku/nodejs
$ heroku buildpacks:add --index 2 heroku/python
$ heroku addons:create heroku-postgresql:hobby-dev
$ heroku config:set DJANGO_SETTINGS_MODULE=backend.settings.prod

$ git push heroku
```

Heroku's nodejs buidlpack will handle install for all the dependencies from the `packages.json` file.
It will then trigger the `postinstall` command which calls `yarn build`.
This will create the bundled `dist` folder which will be served by whitenoise.

The python buildpack will detect the `pipfile` and install all the python dependencies.

The `Procfile` will run Django migrations and then launch Django'S app using gunicorn, as recommended by heroku.

##### Heroku One Click Deploy

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/Alhakem/django-vuetify-template)

## Static Assets

See `settings.dev` and `vue.config.js` for notes on static assets strategy.

This template implements the approach suggested by Whitenoise Django.
For more details see [WhiteNoise Documentation](http://whitenoise.evans.io/en/stable/django.html)

It uses Django Whitenoise to serve all static files and Vue bundled files at `/static/`.
While it might seem inefficient, the issue is immediately solved by adding a CDN
with Cloudfront or similar.
Use `vue.config.js` > `baseUrl` option to set point all your assets to the CDN,
and then set your CDN's origin back to your domains `/static` url.

Whitenoise will serve static files to your CDN once, but then those assets are cached
and served directly by the CDN.

This allows for an extremely simple setup without the need for a separate static server.

[Cloudfront Setup Wiki](https://github.com/gtalarico/django-vue-template/wiki/Setup-CDN-on-Cloud-Front)
