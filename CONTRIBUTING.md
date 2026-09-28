# Contribution Guidance

If you'd like to contribute to this repository, please read the following guidelines. Contributors are more than welcome to share their learnings with others in this centralized location.

## Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information, see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

Remember that this repository is maintained by community members who volunteer their time to help. Be courteous and patient.

## Question or Problem?

Please do not open GitHub issues for general support questions as the GitHub list should be used for feature requests and bug reports. This way we can more easily track actual issues or bugs from the code and keep the general discussion separate from the actual code.

If you have questions about how to use Power Platform or any of the provided prompts, please visit the [Power Platform Community](https://powerusers.microsoft.com/) at <https://powerusers.microsoft.com/>


## Typos, Issues, Bugs and contributions

Whenever you are submitting any changes to the community sample repositories, please follow these recommendations.

* Always fork the repository to your own account before making your modifications
* Do not combine multiple changes to one pull request. For example, submit any prompts and documentation updates using separate PRs
* If your pull request shows merge conflicts, make sure to update your local main to be a mirror of what's in the main repo before making your modifications
* If you are submitting multiple prompts, please create a specific PR for each of them
* If you are submitting typo or documentation fix, you can combine modifications to single PR where suitable

## Sample Naming and Structure Guidelines

When you are submitting a new sample, it has to follow up below guidelines

* You will need to have a `README.md` file for your contribution, based on [the provided prompt sample template](./templates/prompt-sample/README.md). Copy the template to your prompt folder and update it accordingly. The file must be named exactly `README.md` -- with capital letters -- because this is the information used to publish your sample.
* Prompts that should appear in the sample gallery must include `assets/sample.json`. Keep its title, descriptions, repository URL, products, tags, categories, and authors consistent with the root `README.md`.
* If your prompt includes `assets/sample.json`, the final non-empty line of the prompt's root `README.md` must be the visitor tracker below. Replace `{prompt-path}` with the repository-relative path to the prompt folder, using forward slashes with no leading or trailing slash (for example, `prompts/power-automate/reminder-workflow`).

  ```html
  <img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/{prompt-path}" />
  ```

* The sample should include a folder for each prompt language. For example, for an English prompt, create an `en-us` folder containing a `prompt.md` file with only the prompt text.
* If you find an existing sample which is similar to yours, please extend the existing one rather than submitting a new similar sample
  * When you update existing prompts, please update also `README.md` file accordingly with information on provided changes and with your author details
* When submitting a new prompt, please name the prompt folder accordingly
* Do not use period/dot in the folder name of the provided sample
* All folders should be in lower case

## Submitting Pull Requests

Here's a high-level process for submitting new prompts or updates to existing ones.

1. Sign the Contributor License Agreement (see below)
2. Fork the [pnp/powerplatform-prompts repository](https://github.com/pnp/powerplatform-prompts) to your GitHub account
3. Sync your fork's `main` branch with this repository, then create a new branch for your contribution
4. Include your changes to your branch
5. Commit your changes using a descriptive commit message. These messages are used to track changes for monthly communications
6. Open a pull request from your fork's contribution branch to the `main` branch of `pnp/powerplatform-prompts`
7. Describe the prompt, metadata changes, and validation performed in the pull request

If you feel insecure about that process or are new to GitHub, please consider to attend the [Sharing Is Caring sessions from the PnP team](https://pnp.github.io/sharing-is-caring/#pnp-sic-events) in which the Microsoft 365 PnP team provides hands-on guidance for first time contributors.

Before you submit your pull request consider the following guidelines:

* Search [GitHub](https://github.com/pnp/powerplatform-prompts/pulls) for an open or closed Pull Request
  which relates to your submission. You don't want to duplicate effort.
* Make sure your local clone has an `upstream` remote pointing to [pnp/powerplatform-prompts](https://github.com/pnp/powerplatform-prompts):

  ```shell
  # check if you have a remote pointing to the Microsoft repo:
  git remote -v

  # if you see a pair of remotes (fetch & pull) that point to https://github.com/pnp/powerplatform-prompts, you're ok... otherwise you need to add one

  # add a new remote named "upstream" and point to the Microsoft repo
  git remote add upstream https://github.com/pnp/powerplatform-prompts.git
  ```

* Sync your fork, then create a contribution branch:

  ```shell
  git fetch upstream
  git switch main
  git merge --ff-only upstream/main
  git push origin main
  git switch -c YOUR-SOLUTION-NAME
  ```

* Push your branch to GitHub:

  ```shell
  git push --set-upstream origin YOUR-SOLUTION-NAME
  ```

## Community calls and demos

Weekly Copilot, Microsoft 365, and Power Platform community calls are open to everyone. Join the calls at <https://aka.ms/community/calls>.

To share your learnings and input with the community, request a demo slot at <https://aka.ms/community/request/demo>.

## Merging your Existing GitHub Projects with this Repository

If the sample you wish to contribute is stored in your own GitHub repository, you can use the following steps to merge it with this repository:

* Fork the `powerplatform-prompts` repository from GitHub
* Create a local git repository

    ```shell
    md powerplatform-prompts
    cd powerplatform-prompts
    git init
    ```

* Pull your forked copy of `powerplatform-prompts` into your local repository

    ```shell
    git remote add origin https://github.com/yourgitaccount/powerplatform-prompts.git
    git pull origin main
    ```

* Pull your other project from GitHub into the `prompts` folder of your local copy of `powerplatform-prompts`

    ```shell
    git subtree add --prefix=prompts/YOUR-SOLUTION-NAME https://github.com/yourgitaccount/YOUR-SOLUTION-NAME.git main
    ```

* Push the changes up to your forked repository

    ```shell
    git push origin main
    ```

## Signing the CLA

Before we can accept your pull requests you will be asked to sign electronically Contributor License Agreement (CLA), which is a pre-requisite for any contributions all PnP repositories. This will be one-time process, so for any future contributions you will not be asked to re-sign anything. After the CLA has been signed, our PnP core team members will have a look at your submission for a final verification of the submission. Please do not delete your development branch until the submission has been closed.

You can find Microsoft CLA from the following address - <https://cla.microsoft.com>.

Thank you for your contribution.

> Sharing is caring.
