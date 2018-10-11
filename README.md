# Typescript + Parcel

1. add package.json
```
yarn add --dev parcel-bundler react react-dom typescript @types/react @types/react-dom @types/node
```
2. create html file
3. add script in package.json 
``` json
"scripts": {
  "start": "parcel public/index.html"
}
``` 
4. <button disabled>Command</button> + <button disabled>Shift</button> + <button disabled>P</button> <br/>
type "project" then click `"Configure tsconfig.json"`

5. config in tsconfig.json
``` json
{
  "compilerOptions": {
    ...
    "jsx": "react",
    "esModuleInterop": true, 
    "strict": true
  },
  "include": [
    "src"
  ],
  ...
}
```
`"esModuleInterop"` if it **true**, it make you can use import React from 'react' instead import * as React from 'react'<br>
`"strict"` checking type (instead TSlint)

6. **DONE!**

###### if it not working you must <button disabled>Command</button> + <button disabled>Shift</button> + <button disabled>P</button> and type `restart TS server`