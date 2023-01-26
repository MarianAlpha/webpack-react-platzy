# React con Webpack

- npm i react react-dom -S
- npm init
- crear la carpeta src y alli dentro se crean:
- index.js (dentro src)
- carpeta Components (dentro de src)
- App.jsx dentro de componets

En index.js se importa react con
import React from 'react';
import ReactDom from 'react-dom';
import  App from './componets/App'
ReactDom.render(
    `<App />,`
    getElementById('app')
)
Luego en la raiz se crea un carpeta llamada public
alli index.html

## Webpack

npm i @babel/core @babel/preset-env @babel/preset-react babel-loader -D
npm i webpack webpack-cli webpack-dev-server -D
npm i html-loader html-webpack-plugin -D

## Css

npm i mini-css-extract-plugin css-loader style-loader sass sass-loader -D
npm i css-minimizer-webpack-plugin terser-webpack-plugin clean-webpack-plugin -D

- Se crea el config.dev, se copia lo del config normal y se añanade el mode: development

## Para crear secciones en react

Se necesita React Router

¿Qué es router en React?
Debido a que React es de tipo SPA(single page application), no recarga la página cuando cambiamos de url. Sin embargo, router nos ayuda a crear otra página para poder navegar en nuestra aplicación. Imagina twitter web, cuando das click en un tweet, se abre otra sección donde puedes ver el tweet. Sería un problema que al momento de darle click, no cambie la url, por lo que ese tweet no tiene dirección propia, no se guardaría en tu historial y sería un problema el SEO. Para ello, usamos router, que se encargará de administrar esta situación, donde en el momento que abras el tweet, cambie la URL, pero todavía mantenga ese dinamismo y rapidez de una SPA.

¿Entonces qué es ReactRouterDOM?
npm i react-router-dom
