https://medium.com/@trukrs/type-safe-javascript-with-jsdoc-7a2a63209b76
VsCode ayarlardan checkJs:true yapılır
````
"javascript.implicitProjectConfig.checkJs": true
````

````
Enums.js

/**
 * @typedef {Object} Person
 * @prop {string} ad
 * @prop {number} kilo
 */
 

/** @type {Person} person */
export const personel = {
  ad: "summer",
  kilo: 20,
};

//intellisense devreye girer burda name ve age hatalı property//
/** @type {Person} person */
export const person = {
  name: 'Joe', 
  age: 32
}


````

````
import React, { Component } from "react";

import { personel } from "./enums";

export default class Home extends Component {
  constructor(props) {
    super(props);
    console.log("xxx");
  }

  Kaydet1() {
  
  // burda intellisense aktif hale gelir
    let x=personel.kilo;
  }

  render() {
    return (
      <div>
        <button onClick={() => this.Kaydet1()}>Kaydet</button>
      </div>
    );
  }
}


````
