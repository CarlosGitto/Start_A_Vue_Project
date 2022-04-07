# Starting a new Vue 3 project for linux with bootstrap

Please be sure you have install `Node.js` before continue

## VUE

### Start a CLI and run

```
npm install -g @vue/cli
vue --version
vue create hello-world
```

### Manually select features

Select the following options:

Features:

- Chose Vue version
- Babel
- Router
- Vuex
- Linter / Formatter (Optional)

Vue version:

- 3.x

History router:

- n

Lint config:

- ESLint + Prettier
- Lint on save

Save config files:

- In package.json

Save personalize config:

- y
- [name for this config]

## BOOTSTRAP

### Start a CLI and run

```
cd /your_project_path
npm install bootstrap
code .
```

### Inside the Project Files

In the route `/src/main.js` add:

```
import "bootstrap";
import "bootstrap/dist/css/bootstrap.min.css";
```

## Start the server

In a shell with the route to your vue project open run the following:

```
npm run serve
```

Then go to your browser and type 'http://localhost:8080'

## END

