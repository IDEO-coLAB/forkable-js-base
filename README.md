# `forkable-js-base`

This is the IDEO CoLab's base repository for all new projects using JavaScript that will be maintained by the CoLab or people/teams working with the CoLab. 

This repo contains a custom `eslint` config file and the necessary `npm` packages to ensure code linting according to the CoLab javascript styleguide. We currently use the [Airbnb `javascript` styleguide](https://github.com/airbnb/javascript) and the linter ensures adherence to their documentation. 

The base `package.json` file only includes the necessary `devDependencies` and a lint script which you can then run from your project.

## Install

```shell
> git clone -o [your_origin_repo_name] -b master --single-branch https://github.com/IDEO-coLAB/forkable-js-react-static [your_origin_repo_name]
> cd [your_origin_repo_name]

# Init npm
> npm init

# Install project dependencies listed in package.json
> npm install
```

## Usage

```shell
# Run the linter on your code base
> npm run lint
```

## License

MIT © IDEO CoLab
