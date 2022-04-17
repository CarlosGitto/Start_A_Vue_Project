# Starting a new Vue 3 project for linux with Bootstrap 5 and Fontawesome

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

## FONTAWESOME
### Start a CLI and run

```
cd /your_project_path
npm i --save @fortawesome/fontawesome-svg-core
npm i --save @fortawesome/free-solid-svg-icons
npm i --save @fortawesome/free-regular-svg-icons
npm i --save @fortawesome/vue-fontawesome@prerelease
code .
```

### How to add fontawesome icons to your vue project

Inside your project go to `src/main.js` and add the following:

```
import { library } from '@fortawesome/fontawesome-svg-core'

import { faHatWizard } from '@fortawesome/free-solid-svg-icons'

import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

library.add(faHatWizard)

```
***`library.add()` can recieve an array of icons**

Where `faHatWizard` is the name of the icon you want to add, the on your `create(App)` append `.component('font-awesome-icon', FontAwesomeIcon)`

To use the icon insert into your template code:

`<font-awesome-icon icon=”hat-wizard” />`

## Sources

- https://cli.vuejs.org/guide/creating-a-project.html
- https://stackoverflow.com/questions/65547199/using-bootstrap-5-with-vue-3
- https://blog.fontawesome.com/how-to-use-vue-js-with-font-awesome/

## END

