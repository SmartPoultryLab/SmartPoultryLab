# Smart Poultry Laboratory


## Used Technologies
Smart Poultry Laboratory uses a number of open source projects to work properly:

- [Python](https://www.python.org/) - programming language that lets you work quickly and integrate systems more effectively
- [Django](https://www.django-rest-framework.org/) - powerful and flexible toolkit for building Web APIs.
- [MySQL](https://www.mysql.com/) - fully managed database service to deploy cloud-native applications.
- [Vue](https://vuejs.org/) - Progressive JavaScript Framework for building reactive single page applications

## _Backend-Group Tasks_

### Tasks list (Mohamed Shawky)
- [x] Users api CRUD endpoints
- [x] DRF JWT Authentication
- [x] Add docker configurations
- [ ] Document folder structure
- [ ] Configure Static/media & templates
- [ ] Integrate material ui & react js on templates
  

### Tasks list (Omar Baz)
- [x] Users api CRUD endpoints
- [x] DRF JWT Authentication
- [x] Add docker configurations
- [ ] Document folder structure
- [ ] Configure Static/media & templates
- [ ] Integrate material ui & react js on templates

## _Frontend-Group Tasks_

### Tasks list (Ali Gamal)
- [x] Users api CRUD endpoints
- [x] DRF JWT Authentication
- [x] Add docker configurations
- [ ] Document folder structure
- [ ] Configure Static/media & templates
- [ ] Integrate material ui & react js on templates
  

### Tasks list (Lo'ay Mokhtar)
- [x] Users api CRUD endpoints
- [x] DRF JWT Authentication
- [x] Add docker configurations
- [ ] Document folder structure
- [ ] Configure Static/media & templates
- [ ] Integrate material ui & react js on templates

## _Database-Group Tasks_

### Tasks list (Ahmed Saify)
- [x] Users api CRUD endpoints
- [x] DRF JWT Authentication
- [x] Add docker configurations
- [ ] Document folder structure
- [ ] Configure Static/media & templates
- [ ] Integrate material ui & react js on templates
  


## Installation

### Includes

* Django
* Django REST framework
* Django Whitenoise, CDN Ready
* Vue CLI 3
* Vue Router
* Vuex

### Project Structure


| Location             |  Content                                   |
|----------------------|--------------------------------------------|
| `/backend`           | Django Project & Backend Config            |
| `/backend/api`       | Django App (`/api`)                        |
| `/src`               | Vue App .                                  |
| `/src/main.js`       | JS Application Entry Point                 |
| `/public/index.html` | Html Application Entry Point (`/`)         |
| `/public/static`     | Static Assets                              |
| `/dist/`             | Bundled Assets Output (generated at `yarn build`) |

## Prerequisites

Before getting started you should have the following installed and running:

- [x] Node.js - [instructions](https://nodejs.org/en/download/)
- [X] Yarn - [instructions](https://yarnpkg.com/en/docs/install)
- [X] Vue CLI 3 - [instructions](https://cli.vuejs.org/guide/installation.html)
- [X] Python 3 - [instructions](https://wiki.python.org/moin/BeginnersGuide)
- [X] Pipenv - [instructions](https://pipenv.readthedocs.io/en/latest/install/#installing-pipenv)

## Setup Project

```
$ git clone https://github.com/SmartPoultryLab/SmartPoultryLab.git
$ cd SmartPoultryLab
```

Setup
```
$ yarn install
$ pipenv install --dev && pipenv shell
$ python manage.py migrate
```

## Running Development Servers

```
$ python manage.py runserver
```

From another tab in the same directory:

```
$ yarn serve
```

The Vue application will be served from [`localhost:8080`](http://localhost:8080/) and the Django API
and static files will be served from [`localhost:8000`](http://localhost:8000/).

The dual dev server setup allows you to take advantage of
webpack's development server with hot module replacement.
Proxy config in [`vue.config.js`](/vue.config.js) is used to route the requests
back to django's API on port 8000.

If you would rather run a single dev server, you can run Django's
development server only on `:8000`, and you have to build the Vue app first
and the page will not reload on changes.

```
$ yarn build
$ python manage.py runserver
```