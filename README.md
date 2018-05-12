# Eslint-Airbnb-Conf
Konfiguracja eslint

// install the following packages: \n
// npm info "eslint-config-airbnb@latest" peerDependencies\n
// yarn add --dev prettier eslint-config-prettier eslint-plugin-prettier babel-eslint\n
//  (\n
//    export PKG=eslint-config-airbnb;\n
//    npm info "$PKG@latest" peerDependencies --json | command sed 's/[{},]//g ; s/: /@/g' | xargs npm install --save-dev "$PKG@latest"\n
//  )\n
\n
\n
{\n
  "extends": ["airbnb", "prettier", "prettier/react"],\n
  "plugins": ["prettier"],\n
  "parser": "babel-eslint",\n
  "parserOptions": {\n
    "ecmaVersion": 2016,\n
    "sourceType": "module"\n
  },\n
  "env": {\n
    "es6": true,\n
    "browser": true,\n
    "node": true\n
  },\n
  "rules": {\n
    "react/jsx-filename-extension": [1, { "extensions": [".js", ".jsx"] }],\n
    "jsx-a11y/anchor-is-valid\": [ "error",\n
      {\n
    		"components": ["Link"],\n
    		"specialLink": ["to"],\n
    		"aspects": ["noHref", "invalidHref", "preferButton"]\n
      }\n
    ]\n
  }\n
}\n
\n
