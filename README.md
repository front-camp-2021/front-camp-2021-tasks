[![](https://github.com/Eleks-front-camp/front-camp-2021/actions/workflows/tests.yml/badge.svg)](https://github.com/Eleks-front-camp/front-camp-2021/actions)

# Tasks list

| **Task name**       | **Dragonkills points** | 
|:---                 |:---:                   |
| "pick"              | 5                      |
| "omit"              | 5                      |
| "highestAndLowest"  | 4                      |
| "largestPairSum"    | 4                      |
| "repeatString"      | 8                      |
| "getLastWordLength" | 3                      |
| "chunk"             | 3                      |
| "sameParityFilter"  | 8                      |
| "trimSymbols"       | 10                     |
| **Total**           | 50                   |

## To start project:

To start project, please run the next commands:

* `npm install` - install dependencies

**Note:** You must have installed Nodejs and Npm on your local machine  
To check versions of Nodejs and Npm please run in terminal: `node -v` и `npm -v`  
Required versions:
```
  "engines": {
    "node": ">=14.0.0",
    "npm": ">=6.0.0"
  }
```

## To run tests:

### To run all tests

To run all project tests:

`npm test`

### To run tests from a specific directory

Please use next command to run tests from a specific directory

`npm test -- --findRelatedTests <path>`

For example, the next command runs all "spec" files from "01-sum" directory:

`npm test -- --findRelatedTests 01-sum/**/*.spec.js`

where `01-sum/**/*.spec.js` is a path to task directory 

### To run a single test

To run only one test, please use next command:

`npm test -- -t '<describeString> <itString>'`

* `describeString` is a name of "describe" block
* `itString`is a name of "it" block

For example, next command runs "describe" with name "sum" and "it" with name "should return sum of numbers":

`npm test -- -t 'sum should return sum of numbers'`

For more details please check official Jest documentation [Jest](https://jestjs.io/docs/en/cli.html#--testnamepatternregex)
