# `forkable-js-base`
This is the IDEO CoLab's base repository for all new JavaScript projects. When creating a new project that uses JavaScript and will be maintained by the CoLab, please [fork this repo](https://help.github.com/articles/fork-a-repo/) and use it as the base for your new project. 

## What This Includes

### Git Hooks

You will find all Git Hooks in your project's `.git/hooks/` folder. This base repo includes custom Hooks which are automatically run when certain Git events are triggered.

#### pre-commit hook

**Description:** This hook is run before any `git commit ...` command and tests for adherence to the [Airbnb `javascript` styleguide](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb-base). Full documentation for the guide can be [found here](https://github.com/airbnb/javascript).

**Location:** `<project_root>/.git/hooks/pre-commit`

## Learning Resources

### Git Hooks

To learn more about Git hooks, check out [this chapter](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks) on customizing Git. This link is to a Git-Hook-relevant chapter, but the book, overall, is a great guide to using Git.

## Contribute

PRs are welcome!

## License

MIT © IDEO CoLab
