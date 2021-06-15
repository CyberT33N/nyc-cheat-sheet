# NYC Cheat Sheet
NYC Cheat Sheet with the most needed stuff..














<br><br>

# Install
```bash
npm i -D nyc
```



















<br><br>
____________________________________
____________________________________
<br><br>





# How do I read an Istanbul Coverage Report?
- https://stackoverflow.com/questions/26618243/how-do-i-read-an-istanbul-coverage-report




<br><br>

- There are a number of coverage criteria, the main ones being:

  - **Function coverage** - Has each function (or subroutine) in the program been called?
  - **Statement coverage** - Has each statement in the program been executed?
  - **Branch coverage** - Has each branch (also called DD-path) of each control structure (such as in if and case statements) been executed? For example, given an if statement, have both the true and false branches been executed? Another way of saying this is, has every edge in the program been executed?
  - **Line coverage** - Has each executable line in the source file been executed?
For each case, the percentage represents executed code vs not-executed code, which equals each fraction in percent format (e.g: 50% branches, 1/2).








































<br><br>
____________________________________
____________________________________
<br><br>

# package.json
```json
{
  "name": "sample-project",
  "version": "0.0.1",
  "description": "any description",
  "main": "src/index.js",
  "scripts": {
    "coverage": "nyc npm run test",
    "integration-test": "mocha test/integration/**/*.test.js --exit",
    "unit-test": "mocha test/unit/**/*.test.js --exit",
    "test": "npm run integration-test && npm run unit-test",
  },
  "files": [
    "src",
    "README.md",
    "CHANGELOG.md"
  ],
  "repository": {
    "type": "git",
    "url": "http://github.com/sample-project/sample-project.git"
  },
  "keywords": [
    "test",
    "apple"
  ],
  "author": "CyberT33N",
  "license": "SEE LICENSE IN LICENSE.txt",
  "dependencies": {
    "dotenv": "*"
  },
  "devDependencies": {
    "nyc": "*",
    "mocha": "*"
  }
}
```

```bash
npm run coverage
```

<br><br>


