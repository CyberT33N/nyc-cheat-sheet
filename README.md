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
  }
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


