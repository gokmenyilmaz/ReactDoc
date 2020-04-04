````
# .env.developement
REACT_APP_API_ENDPOINT = "https://development-api.endpoint.com/"
````

````
{
  "name": "cra-env-cmd",
  "version": "0.1.0",
  "private": true,
  "homepage": ".",
  "dependencies": {
    "antd": "^4.1.0",
    "env-cmd": "^10.0.1",
    "react": "^16.8.6",
    "react-dom": "^16.8.6",
    "react-router-dom": "^5.1.2",
    "react-scripts": "3.0.1"
  },
  "scripts": {
    "start": "env-cmd -f .env.development react-scripts start",
    "build": "env-cmd -f .env.production react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  },
  "eslintConfig": {
    "extends": "react-app"
  },
  "browserslist": {
    "production": [
      ">0.2%",
      "not dead",
      "not op_mini all"
    ],
    "development": [
      "last 1 chrome version",
      "last 1 firefox version",
      "last 1 safari version"
    ]
  }
}
````
uygulalaması

````

import React, { Component } from 'react'

export default class Ekran extends Component {
    constructor(props)
    {
        super(props);
    }

    componentDidMount()
    {
      
    }

    render() {
        return (
            <div>
                xxxx:
              {process.env.REACT_APP_API_ENDPOINT}
            </div>
        )
    }
}
````
