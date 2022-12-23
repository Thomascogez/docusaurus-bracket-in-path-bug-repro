# Docusaurus bracket in path bug reproducible example

This is a minimal example of a bug in Docusaurus where a bracket in the path causes the build to fail.

## Steps to reproduce

1 - Clone this repo

2 - cd into `[bracket]` folder

3 - Run `yarn install`

4 - Run `yarn build`

5 - Observe the following error:

```sh
[ERROR] Error: EISDIR: illegal operation on a directory, open '/Users/user/Documents/projectPath/docusaurus-bracket-in-path-bug-repro/[bracket]/build'
[ERROR] Unable to build website for locale en.
[ERROR] Error: EISDIR: illegal operation on a directory, open '/Users/user/Documents/projectPath/docusaurus-bracket-in-path-bug-repro/[bracket]/build'
```

## Expected behavior

The build should succeed.

## Actual behavior

The build fails with the following error:

```sh
[ERROR] Error: EISDIR: illegal operation on a directory, open '/Users/user/Documents/projectPath/docusaurus-bracket-in-path-bug-repro/[bracket]/build'
[ERROR] Unable to build website for locale en.
[ERROR] Error: EISDIR: illegal operation on a directory, open '/Users/user/Documents/projectPath/docusaurus-bracket-in-path-bug-repro/[bracket]/build'
```
