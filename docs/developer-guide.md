# Developer Guide

!!! info

    This chapter is only of interest if you want to make changes to the code of the vscode extension!

## Development Basics

### Build dependencies

- [node](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

### Building

```bash
npm install # installs all required dependencies
npm run package # builds the .vsix package
```

## Github Release Process

To release a new extension version, the following steps must be followed:

1. Create a [new release](https://github.com/cross-language-cpp/vscode-djinni/releases/new) on Github like [described here](https://docs.github.com/en/github/administering-a-repository/managing-releases-in-a-repository). 
   Set a tag version following [semantic versioning](https://semver.org/) rules (`v<MAJOR>.<MINOR>.<PATCH>`) and describe what has changed in the new version.
2. Wait. Github will automatically build the extension, publish it to the [Visual Studio Marketplace](https://marketplace.visualstudio.com/publishers/cross-language-cpp) & upload the packaged extension to the release.

That's it! :blush:
