# Eslint-Airbnb-Conf
Konfiguracja eslint

// install the following packages:
// npm info "eslint-config-airbnb@latest" peerDependencies
// yarn add --dev prettier eslint-config-prettier eslint-plugin-prettier babel-eslint
//  (
//    export PKG=eslint-config-airbnb;
//    npm info "$PKG@latest" peerDependencies --json | command sed 's/[{},]//g ; s/: /@/g' | xargs npm install --save-dev "$PKG@latest"
//  )


{
  "extends": ["airbnb", "prettier", "prettier/react"],
  "plugins": ["prettier"],
  "parser": "babel-eslint",
  "parserOptions": {
    "ecmaVersion": 2016,
    "sourceType": "module"
  },
  "env": {
    "es6": true,
    "browser": true,
    "node": true
  },
  "rules": {
    "react/jsx-filename-extension": [1, { "extensions": [".js", ".jsx"] }],
    "jsx-a11y/anchor-is-valid\": [ "error",
      {
    		"components": ["Link"],
    		"specialLink": ["to"],
    		"aspects": ["noHref", "invalidHref", "preferButton"]
      }
    ]
  }
}

