# Dependency confusion test
Test all the Node.js projects of a Github account for the dependency confusion vulnerability. More info about this vulnerability [here](https://medium.com/@alex.birsan/dependency-confusion-4a5d60fec610).

## Install
```
npm install -g confusion-test
```

## Use
To run this test you will need a Github token. Generate it [here](https://github.com/settings/tokens).

Example for one account:
```
$ echo 'notsag-dev' | confusion-test --token {{GITHUB_TOKEN}}
```

Example for multiple accounts (one per line):
```
$ cat accounts.txt | confusion-test --token {{GITHUB_TOKEN}}
```

To disable console output add `--silent`.

## Results
A file will be created with information about the packages that are available on the npm registry.

Line format: `{{account}};{{package-name};{{package-version}};{{repository}};{{package-json-path}}`
