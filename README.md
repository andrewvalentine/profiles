Configuration Profiles for use in the management of macOS

**Notes on Microsoft-AutoUpdate-settings.mobileconfig**

* Sets MAU to update all Microsoft Office apps to the current release. At the time of writing, this is the `2019` branch.
* This includes Skype for Business and Microsoft Remote Desktop.
* Sets update channel to MS 'Production' (Insider Slow).
* Disables user ability to modify MAU update channel setting.
* Enables verbose logging.
* Disables 'SendAllTelemetryEnabled'.
* Enables 'AutomaticDownload' of updates.
* Starts MAU daemon on launch of any Office app.
* Sets update check frequency to 12 hours.

**Notes on Stata15-update-settings.mobileconfig**

At the time of writing, a means of obtaining and deploying updates to Stata from macOS software management tools does not exist. This profile was therefore constructed to enable updates and control their behaviour.

This profile does the following:

* Supresses the advertisement of updates to the user
* Enables update checks
* Disables the prompt for whether the application should check for updates
* Sets the autoupdate check to every 7 days

Testing has shown that when an update is detected by the automatic check:

* It will be advertised to the user
* The update can be applied without admin rights
