# Onboarding flow

## Description

Many times teams struggle with proper onboarding process due to the fact of adding user to many tools. It is time-consuming and can lead to mistakes. This flow can automate this process by adding user added to SharePoint list (access tracker) to selected Security Group which is assigned to many different Office Apps like SharePoint, Power Apps or Power BI. At one time we can grant access to all apps we need in our process.

Recommended place to run: Cloud flows designer with enabled copilot.

Recommended implementation approach:
1) Open new empty flow with enabled copilot
2) Add first prompt (remember to adjust parameters):
    > Use trigger When an item is created or modified. Enter trigger Site Address custom value: 'YOUR SITE ADDRESS' and custom List Name value: 'YOUR LIST NAME'. 
3) Add second prompt (remember to adjust parameters):
    > Add Get user profile and use "['SHAREPOINT FIELD STORING INFO ABOUT USER']?['Email']" in UPN.
4) Add third prompt (remember to adjust parameters):
    > Add Entra action Add member to group. As user Id enter id from Get User profile. As Group Id enter: 'YOUR SECURITY GROUP ID'.
5) Add fourth prompt:
    > Send email to user added to the group. Fill in subject and body. At least 5 sentences.
6) Save and test flow.

Potential things to consider:
- Add member to group action requires admin right.

## Prompt

### Supported Language(s)

[English](./en-us/prompt.md)

## Authors

Solution|Author(s)
--------|---------
Onboarding flow | [Andrzej Bożyk](https://www.github.com/abozyk1990) ([@BozykAndrzej](https://twitter.com/BozykAndrzej)), Individual Contributor


## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/samples/power-automate/onboarding-flow" aria-hidden="true" />
