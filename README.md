# Dependency confusion test
Test all the Node.js projects of a Github account for the dependency confusion vulnerability. To run this test it is mandatory to count with a Github token.

## Install
```
npm install -g confusion-test
```

## Use
```
$ echo 'notsag-dev' | confusion-test --token {{GITHUB_TOKEN}}
```
or 
```
$ cat orgs.txt | confusion-test --token {{GITHUB_TOKEN}}
```

## Results
A file will be created with information about the packages that are available on the npm registry.

Line format: `{{organization}};{{package-name};{{package-version}};{{repository}};{{package.json path}}`
