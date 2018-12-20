# Essential JS2 for Angular with SCSS Compilation

This project we have configured with SASS compilation for Essential JS 2 for Angular application.

## Configuring Node SASS Option in `.angular-cli.json`

To avoid sass compiling issue. We need to add `stylePreprocessorOptions` option to `.angular-cli.json` file.

```js
"stylePreprocessorOptions": { 
    "includePaths": [ 
        "../node_modules/@syncfusion/ " 
    ] 
}
```

Add `stylePreprocessorOptions` option under `apps` in `.angular-cli.json`


```js
 "apps": [{
        "root": "src",
        "outDir": "dist",
        "assets": [
            "assets",
            "favicon.ico"
        ],
        "index": "index.html",
        "main": "main.ts",
        "polyfills": "polyfills.ts",
        "test": "test.ts",
        "tsconfig": "tsconfig.app.json",
        "testTsconfig": "tsconfig.spec.json",
        "prefix": "app",
        "styles": [
            "styles.scss"
        ],
        "stylePreprocessorOptions": {
            "includePaths": [
                "node_modules/@syncfusion"
            ]
        },
        "scripts": [],
        "environmentSource": "environments/environment.ts",
        "environments": {
            "dev": "environments/environment.ts",
            "prod": "environments/environment.prod.ts"
        }
    }],
```

## Installing and Running Application

## Installing Angular CLI

To install Angular CLI use the following command

```
npm install -g @angular/cli
```

### Installing Package 

To install required package for this application. Run the below command.

```
npm install
```

### Running Application

To run this application. Run the below command.

```
npm start
```
