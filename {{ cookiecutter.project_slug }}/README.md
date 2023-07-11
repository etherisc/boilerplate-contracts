# {{ cookiecutter.project_name }}

Welcome to your new project!

The project is based on the GIF sandbox. Please see https://docs.etherisc.com/sandbox/ for more information.

## Sample contracts

The `contracts` folder contains sample contracts for a Fire insurance product. You can use them as a starting point for your own project.

## Github actions

The project is configured to use Github actions for CI/CD. 

- The _Build_ action (`.github/workflows/build.yml`) will compile the contracts and run the tests. It will also run `solhint` with the rules defined in `.solhint.json`.
- In case you want to puslish your contracts to npmjs, the `build.yml` action contains commented outcode at the end of the file to do so. Please make sure the `package.json` file is configured correctly before enabling the action. You will also need to configure a `NPMJS_ACCESS_TOKEN` secret in your repository for the action to work.

## Dependabot

The project is configured to use Dependabot to keep the dependencies up to date. The configuration file is located at `.github/dependabot.yml`. To enable using the automated PRs, you will need to enable the commented out code in the file.

