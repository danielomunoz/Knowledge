# Curso de Complete React Developer in 2022 (w/ Redux, Hooks, GraphQL)

## Índice del curso:
1.- Introducción (nada importante)
2.- React Key Concepts  
3.- React Basics
4.- Capstone Project: Intro + Setup

### 2.- React Key Concepts
* Declarative vs Imperative: Tú no tocas el DOM, es React quien se encarga de ello mientras que tú le pasas el objeto de estado. Él toca el DOM cuando mejor le viene y de la mejor manera sin tú enterarte.

* Component Architecture: Explica cómo es la arquitectura basada en componentes.

* One Way Data Flow: React construye un VirtualDOM con los componentes en medio del árbol y va observando cómo cambia el estado -> para cambiar el VirtualDOM -> para cambiar el DOM real. Y sólo en esta dirección de cambio.

* UI Library: Existen librerías con componentes predefinidos para crear nuestras vistas.

### 3.- React Basics
* Aquí instalamos NVM, NodeJS y Yarn:  
`curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash`  
`source ~/.bashrc`  
`nvm install v12.22.12`  
`sudo apt install curl`  
`curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -`  
`echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list`  
`sudo apt update && sudo apt install yarn`  

* Create React App - NPX: Aprendemos a crear el scaffolding de una app completa de react usando  
`npx create-react-app [nombre]`  
`cd [nombre]`  
`npm start`  
También explica lo que es npx. Básicamente npx descarga la última versión de un paquete y lo ejecuta sin tener que instalarlo previamente en tu pc, ni local ni globalmente.
* Create React App - React-Scripts 1 ... 2: Aquí explica un poco el funcionamiento general + los scripts del paquete react-scripts (start, build, test, eject)
* Create React App - Everything Else: Explica el scaffolding de una app de React
* Monsters Rolodex - Class Components: Aquí transforma una app con hooks en una app con clases, y seguiremos así para todo este proyecto de los Monsters.
* Monsters Rolodex - Component State: Construímos un estado en el constructor de nuestro componente App y lo utilizamos para renderizar un nombre.
* Monters Rolodex - setState: Utilizar la función setState() para cambiar el estado y forzar un reRender.
* Monsters Rolodex - setState and Secondary Callback: Cuidado con setState que es una función asíncrona! Si queremos ver el estado después de ejecutarla, deberemos hacer el console log en su callback
* Monsters Rolodex - Mapping Arrays to Elements: Usamos map a modo de ngFor, muy útil!
* Monsters Rolodex - Keys for Mapping: Cada elemento del mapping debe tener una key única para React. Si hubiera más de un elemento en el map (h1 dentro de un div), la key deberá estar en el elemento padre.
* Monsters Rolodex - Lifecycle Method: componentDidMount: Introducción a los lifecycle methods. En este caso, después de que el componente se monte.
* Monsters Rolodex - Renders & Re-renders in React: Explica, con lo que tenemos ya, qué se ejecuta antes y qué después en nuestro componente. Constructor -> render -> componentDidMount. Pero después del DidMount React detecta un cambio, por lo que se vuelve a ejecutar el render().
* Monsters Rolodex - Optimizations: Mejoras sobre lo que tenemos ya. Funciones anónimas y por qué no es óptimo dejarlas anónimas.
* Monsters Rolodex - CardList Component: Comenzamos a componetizar el proyecto
* Monsters Rolodex - Component Props: Explica los props, es decir, las propiedades que pasas a otros componentes.
* Monsters Rolodex - Rendering and Re-rendering part 2: Vuelve a explicar el flujo de renderizados según el árbol de componentes de nuestra App.
* Monsters Rolodex - CSS in React: Lo más importante aquí es que los CSS que vayamos importando son globales, no están aislados sino que se "ven" en todo el proyecto
* Functional vs Class Components: A partir de aquí comienza a explicar cómo sería nuesta app si hubiésemos usado componentes funcionales en lugar de clases (los cuales son más modernos).
* Class Component Lifecycle Methods Breakdown: IMPORTANTE, muestra foto muy ilustrativa de los lifecycles más comunes en React. Por ejemplo, existe una orden para forzar a React a que reRenderice. Los componentes funcionales no siguen esos lifecycles methods específicos, pero sí siguen el mismo lifecycle.
* Monsters Rolodex - Functional Component Intro: Introducción a los componentes funcionales -> Migrando nuestro proyecto de Monsters Rolodex.
* Pure & Impure Functions: Explica la diferencia entre funciones puras e impuras, importante para comprender la diferencia entre componentes funcionales y clases, porque los componentes funcionales son funciones impuras.
* Monsters Rolodex - Hooks: useState: IMPORTANTE el uso de useState (estado para componentes funcionales).
* Monsters Rolodex - Functional Component Re-rendering: Cuándo se reRenderiza un componente funcional.
* Monsters Rolodex - Infinite Re-rendering: Problema que tenemos con el fetch de los monstruos que tenemos que hacer. Viene a enseñarnos el componentDidMount de los componentes funcionales, o cómo se hace un fetch realmente con componentes funcionales.
* Monsters Rolodex - Hooks: useEffect: IMPORTANTE: este es el componentDidMount de los componentes funcionales.
* React v18: Strict Mode Changes: Explica por qué aparecen dobles los console.logs! Es por el modo estricto de React18, no es que estemos haciendo nada mal :)
* Estos últimos vídeos son vídeos del funcionamiento profundo de React, ReactDOM, etc. Es decir, cómo React hace las cosas "por detrás". Útiles si se quiere coger un conocimiento profundo.
* React and ReactDOM: Es un vídeo interesantísimo donde construye un proyecto de React con un raw index.html from scratch.

### 4.- Capstone Project: Intro + Setup
* 