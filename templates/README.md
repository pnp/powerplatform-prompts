# Templates

In this directory, you will find a directory named `prompt-sample` which you can use as the starting point of your prompt sample. Make sure to follow the following steps:

1. Copy the directory
1. Paste it into the `prompts` directory 
1. Rename the directory and give it a name like `email-generator` or `email-summarizer` - don't use capital letters
1. Update the `README.md` file in your sample folder
1. Enter the prompt in the `prompt.md` file inside
1. Optional: Add additional languages. For instance use `fr-fr` for French.

If the prompt includes `assets/sample.json`, its root `README.md` must end with the following visitor tracker:

```html
<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/{prompt-path}" />
```

Replace `{prompt-path}` with the repository-relative path to the prompt folder, using forward slashes with no leading or trailing slash. For example, a prompt stored in `prompts/power-automate/reminder-workflow` uses that exact value as the suffix after `powerplatform-prompts/`.
