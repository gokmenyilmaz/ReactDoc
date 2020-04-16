````
/** @enum {number} */
export const JSDocState = {
  BeginningOfLine: 0,
  SawAsterisk: 1,
  SavingComments: 2,
};

````

````
//@ts-check

import React, { Component } from "react";

import { personel, JSDocState } from "./enums";

export default class Home extends Component {
  Kaydet1() {
    // burda intellisense aktif hale gelir
    let x = personel.dosyano;

    /** @type{Array.<number>} */
    var y = [];

    y.push("sdsds");

    var x=JSDocState.SavingComments;

    
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
