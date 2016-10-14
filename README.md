# `forkable-js-base`

This is the IDEO CoLab's base repository for all new projects using JavaScript that will be maintained by the CoLab or people/teams working with the CoLab. 

This repo contains a custom `eslint` config file and the necessary `npm` packages to ensure code linting according to the CoLab javascript styleguide. We currently use the [Airbnb `javascript` styleguide](https://github.com/airbnb/javascript) and the linter ensures adherence to their documentation. 

The base `package.json` file only includes the necessary `devDependencies` and a `lint` script which you can then run from your project.

## Purpose

The purpose of using this project as the base repo for all javascript projects is to ensure code consistency across all CoLab projects using javascript. 

**Note**: We are not automating the running of the `lint` command which comes bundled with the repo (see below). It is up to you to run it as much as you like during development. **Simply be sure to lint your code before committing.**

## Install

```shell
> git clone -o [your_origin_repo_name] -b master --single-branch git@github.com:IDEO-coLAB/forkable-js-base.git [your_origin_repo_name]
> cd [your_origin_repo_name]

# Init npm; set up your package.json config
> npm init

# Install project dependencies listed in package.json
> npm install
```

## Usage

**Note: Whether manually or in a custom build script that you create, the `lint` command needs to be run before commiting any code.**

After you setup your repo with `npm init` and `npm install`, then you can run the `lint` command that automatically came bundled in your project's `package.json` file.

### Example

Assuming you have some new `.js` files in your project...

```shell
# Run the linter
> npm run lint
```

## License

MIT © IDEO CoLab
