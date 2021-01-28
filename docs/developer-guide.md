# Developer Guide

!!! info

    This chapter is only of interest if you want to make changes to the code of the vscode extension!

## Development Basics

### Build dependencies

- [node](https://nodejs.org/) >= v14.12.0
- [npm](https://www.npmjs.com/) >= 6.14.8
- bash

### Building

```bash
npm install # installs all required dependencies
npm run package # builds the .vsix package
```

## Github Release Process

To release a new extension version, the following steps must be followed:

1. Create a new release-tag. Set a meaningful version number and describe what has changed in the new version. The version must be parseable by [semver](https://docs.npmjs.com/cli/v6/using-npm/semver)! If you are not sure about that, you can check it:
   ```bash
   npm install -g semver # install semver
   semver <versiontag> # check if the version can be parsed
   ```
2. Wait. Github will automatically build the extension, publish it to the [Visual Studio Marketplace](https://marketplace.visualstudio.com/publishers/cross-language-cpp) & upload the packaged extension to the release.

That's it! :blush:
