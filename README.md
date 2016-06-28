# npm-demo

You can find the tests under the test folder.
In order to run the test use npm test

### Installation 
go to the project directory and run:
 npm install -g $(pwd)

### Pipeline script
```
node {
  stage 'Clone Npm Demo git repo'
  git url: 'https://github.com/TamirHadad/npm-demo.git'
  stage 'install dependencies'
  sh "npm install"
  stage "Let's test"
  sh "npm test"
  stage "Let's Deploy"
  sh "npm publish"
}
```


After the npm install you can run  testgen that will print a number to your console
