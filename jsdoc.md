````
#mytypes.js

/** @typedef {{adi: string, dosyano: number}} IsEmri */

export default deneme;

````

````
//@ts-check

import React, { Component } from 'react';
import { render } from 'react-dom';
import Confirm from './confirmService/Confirm'
import FormData from './FormData'


/** @typedef { import('./mytypes').IsEmri } IsEmri */


export default class App extends Component {

  constructor(props) {
    super(props)
    this.removeItem = this.removeItem.bind(this);

    this.adi="rrrrrrrr";
this.kilosu="rrr";


/** @type {IsEmri} */
  this.x={adi:"23434",dosyano:666}

 
   
  }
  ````
