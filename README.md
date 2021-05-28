# Dependency confusion test
Test all the Node.js projects of a Github user for the dependency confusion vulnerability.

## Install
```
npm install -g confusion-test
```

## Use
```
$ echo 'notsag-dev' | confusion-test --token {{GITHUB_TOKEN}}
```

## Results
A file will be created with information about the packages that are available on the npm registry.

Line format: `{{organization}};{{package-name};${package-version};{{repo}};${package.json path}}`
