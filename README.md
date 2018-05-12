# Eslint-Airbnb-Conf
Konfiguracja eslint

// install the following packages: <br />
// npm info "eslint-config-airbnb@latest" peerDependencies <br />
// yarn add --dev prettier eslint-config-prettier eslint-plugin-prettier babel-eslint <br />
//  ( <br />
//    export PKG=eslint-config-airbnb; <br />
//    npm info "$PKG@latest" peerDependencies --json | command sed 's/[{},]//g ; s/: /@/g' | xargs npm install --save-dev "$PKG@latest" <br />
//  ) <br />
 <br />
 <br />
{ <br />
  "extends": ["airbnb", "prettier", "prettier/react"], <br />
  "plugins": ["prettier"], <br />
  "parser": "babel-eslint", <br />
  "parserOptions": { <br />
    "ecmaVersion": 2016, <br />
    "sourceType": "module" <br />
  }, <br />
  "env": { <br />
    "es6": true, <br />
    "browser": true, <br />
    "node": true <br />
  }, <br />
  "rules": { <br />
    "react/jsx-filename-extension": [1, { "extensions": [".js", ".jsx"] }], <br />
    "jsx-a11y/anchor-is-valid\": [ "error", <br />
      { <br />
    		"components": ["Link"], <br />
    		"specialLink": ["to"], <br />
    		"aspects": ["noHref", "invalidHref", "preferButton"] <br />
      } <br />
    ] <br />
  } <br />
} <br />
 <br />
