##

[![clasp](https://img.shields.io/badge/built%20with-clasp-4285f4.svg)](https://github.com/google/clasp)

## How to create this
use this tutorial https://www.youtube.com/watch?v=4Qlt3p6N0es&ab_channel=LearnGoogleSpreadsheets
```
npm install -g @google/clasp
```

```
 clasp login
```
```
 npm init
```

create src directory and clone your script

```
mkdir src
```
Autocomplete with vscode 
```
npm i -S @types/google-apps-script   
```


```
 clasp clone "SCRIPT-ID" --rootDir ./src
 ```

 ## How to use 

- clasp push
- clasp pull
- **Push changes on save in your directory**
    ```
    clasp push -w
    ```

## Features

- Autocomplete for classes of Google Apps Script in VSCode
![Autocomplete for classes of Google Apps Script in VSCode](autocomplete.png)