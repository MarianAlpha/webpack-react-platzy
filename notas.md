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
