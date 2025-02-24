---
Order: 15
xref: ccm-administration-settings-website
Title: Website
Description: Information about setting Website settings within the Administration Settings screen
---

> :choco-info: **NOTE**
>
> This feature is available in Chocolatey Central Management starting with version 0.11.0.

When Chocolatey Central Management sends out emails, they need to know the hostname of the CCM server in order to be able to correctly link back to the Chocolatey Central Management website. When Chocolatey Central Management is installed, it tries to determine the website host and stores it in the Website Settings as the `Web site root address`. If the hostname used to access the Chocolatey Central Management website changes, you will want to update this setting. Follow these steps to configure the Web site root address for Chocolatey Central Management.

1. Open the CCM Site in the browser.
1. Login with the `ccmadmin` user.
1. In the left-hand menu click on `Administration` and then `Settings`.
1. Click on the `Website` tab in the `Settings` screen.

    ![Chocolatey Central Management Website Settings](/assets/images/ccm/setup/website/website-settings.png)

1. Adjust the Web site root address.
1. Click the `Save All` button to save changes.

As noted in the User Interface, any modifications to this section of the settings will require the Chocolatey Central Management Service to be restarted.  This can be completed by doing the following:

1. Get direct access to the machine that is hosting the Chocolatey Central Management Service.
1. Open an administrative PowerShell session.
1. Run the following command: `Restart-Service chocolatey-central-management`.
