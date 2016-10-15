# `forkable-js-base`

This is the CoLab's base repository to be used for all new projects using JavaScript that will be maintained by the CoLab, or people working with the CoLab.

This repo contains a custom `eslint` config file and the necessary `npm` packages to ensure code linting according to the CoLab javascript styleguide. We piggyback off the [Airbnb styleguide](https://github.com/airbnb/javascript), and the automated linter ensures strict adherence to the docs.

This repo's `package.json` file includes *only the minimum* necessary `devDependencies` and a `lint` script which you can run within your project. This way you're completely free to use this as the base for any new project, and still `npm init` without running into issues or odd configurations.

## Purpose

The purpose of this repo is to act as a base for all new, long-term CoLab projects that use javascript, thus ensuring code consistency within CoLab.

Note: We haven't automated the running of the `lint` command in this repo since where it fits best might vary from project to project. However, we strongly suggest you make the `lint` command an automated part of your process. See the Usage section for helpful `lint` automation tips.

**Be ye warned: Lint your code before committing!**

## Setup

Here is an example for how to use this repo as the base for a new CoLab javascript project. Your new project's name is, of all things, `my_new_project`.

1. Create a new GitHub repo. We'll assume that it, too, is named `my_new_project` (you'll use this repo as your new project's `origin` repo).

2. Clone the `forkable-js-base` repo to use as `my_new_project`'s foundation.

```shell
> git clone -b master --single-branch https://github.com/IDEO-coLAB/forkable-js-base.git my_new_project
```

3. Set `my_new_project`'s origin to point at your new GitHub project repo (see step 1) for `my_new_project`.

```shell
# Enter your my_new_project's directory
> cd my_new_project

# Set my_new_project's remote origin to be the GitHub repo you created for it.
> git remote set-url origin git@github.com:<YOUR_GITHUB_USERNAME>/my_new_project.git
```

4. Install the project dependencies listed in package.json.

```shell
> npm install
```

5. Add informtion about your project to `package.json` by running `npm init`.

```shell
> npm init
```

At this point, you're all set! 

## Usage

After you setup your repo with `npm init` and `npm install`, then you can run the `npm lint` command that automatically came bundled in your project's `package.json` file at any time.

**Note: Whether manually run, or run via a custom build script, the `lint` command must be run before commiting your code.**

### Example

Here's how you can manually run the linter.

```shell
# First, add some crappy js to your project...
> touch foo.js
> echo 'var foo = 2' > foo.js

# Then watch the linter complain!
> npm run lint
```

## Additional References

- [Setting git remote urls](https://help.github.com/articles/changing-a-remote-s-url/) (referenced above in [Setup](#setup))
- [Adding a remote](https://help.github.com/articles/adding-a-remote/) (additional reference)

## License

MIT © IDEO CoLab
