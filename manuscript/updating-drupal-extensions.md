# Updating Drupal Extensions

## Extend

Drupal has thousands of Community contributed *extensions* spread between both modules and themes.

During this course, Students will actually create their **own** extentions (both modules and themes). These extensions require a relatively simple process for installation.

> **Best Practices** - Instructions are included here for installing/updating modules via the Administrative Interface. These actually are often much simpler and faster using tools like *Drush*, which is what we will be using in-class.

### To **Install** an extension using the Graphic User Interface (GUI) method

##### Find the FTP/URL link for the desired Module
##### Navigate to the **Modules** (*https://mysite.com/admin/modules*) link
##### Click **Install new module** (*https://mysite.com/admin/modules/install*)
##### Paste the link (if FTP access is available)

### To **Update** an extension, the same user

#### If FTP Access is Available
##### Navigate to the **Available updates** (*https://mysite.com/admin/reports/updates/update*) link.
##### Click the HTML Check-Boxes for each module in need of updating
##### Click **Download these updates**
This action will only *download* the required updates into a temporary folder. It will not actually install or upload anything.

##### Click **Continue**
![Install Updates](../../../images/appendix/updates/ftp-update-1.JPG)
Clicking **Continue** on this step will not take any action other than simply downloading the required extension files into a temporary directory.

###### Updating via GUI for Pantheon.io
For Pantheon.io users, **SFTP** must first be enabled in order for *Update.php* to actually work.

![Update Manager](../../../images/appendix/updates/ftp-update-3.JPG)

##### Ensure Username and Password are correct
![Update Manager](../../../images/appendix/updates/ftp-update-2.JPG)

Clicking **Continue** will authorize Drupal to automatically install the updates downloaded in the Download step.
> **Note** - Pantheon.io users will not see this screen.
![Update Manager](../../../images/appendix/updates/ftp-update-4.JPG)

##### Click **Run database updates**
Having *downloaded* and *installed* the modules, now the MySQL database needs to be configured to accept the changes necessary for the updates.

> **Best Practice** - Drupal gives users the authority to download and install **new** modules *while* updating other modules. This is not recommended simply because modules can conflict for any number of reasons.

![Run database updates](../../../images/appendix/updates/ftp-update-5.JPG)

##### Drupal database update
Drupal, thankfully, tries very hard to prevent issues and pushes very hard for users to back up their database prior to updates, so users must click **Continue** one last time prior to completing the update(s), followed by clicking **Apply pending updates**.

![Finalize database updates](../../../images/appendix/updates/ftp-update-6.JPG)

![Finalize database updates](../../../images/appendix/updates/ftp-update-7.JPG)

And here is a great example of why your database should be backed up!

![Database Errors](../../../images/appendix/updates/ftp-update-8.JPG)

#### If FTP Access is Unavailable
##### Download the module in need of an update.
##### Open the Drupal installation file directory.
##### Navigate to the module in need of an update in ```/sites``` folder.
##### Delete the old module folder.
##### Unzip the new module folder.
##### Run update.php (*https://mysite.com/update.php*)

### To Install using Drush, a user would:

#### Open a CLI with Drush installed

#### Navigate to an Active Drupal Directory

#### Run ```drush status``` (Just to be safe)
This is a good best practice because there might be issues in need to addressing *before* you attempt to install or update a module.

#### Run ```drush dl <module>```

#### Run ```drush en <module>```

#### Run ```drush updb``` (which is also ```drush updatedb```)
