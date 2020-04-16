````
enums.js
/** @typedef {{adi: string, dosyano: number}} IsEmri */

/** @typedef {{No: number, RaporAd: string}} Rapor */


Home.js
import React, { Component } from "react";
import "./enums";

export default class Home extends Component {
  Kaydet() {
    /** @type {IsEmri}*/
    var personx = { adi: "ssdsd", dosyano: 34 };
    personx.dosyano = 434;

    /** @type {Rapor}*/
    var rapor1 = {};
    rapor1.No = 23;
    rapor1.RaporAd = "İnceleme";
  }

  render() {
    return (
      <div>
        <button onClick={() => this.Kaydet()}>Kaydet</button>
      </div>
    );
  }
}

````
