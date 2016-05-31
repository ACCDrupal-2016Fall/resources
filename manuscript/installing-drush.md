# Installing Drush

## Background
Many Web Authoring tasks in Drupal tend to be highly repetitive.

Downloading a module may only be something you do once during installation, but how often are updates required on modules?

### To Install using the Graphic User Interface (GUI) method, a user would:

##### Find the FTP/URL link for the desired Module
##### Navigate to the **Modules** (*https://mysite.com/admin/modules*) link
##### Click **Install new module** (*https://mysite.com/admin/modules/install*)
##### Paste the link (if FTP access is available)

### To update, the same user

#### If FTP Access is Available
##### Navigate to the **Available updates** (*https://mysite.com/admin/reports/updates/update*) link.
##### Click the HTML Check-Boxes for each module in need of updating
##### Click **Download these updates**

##### Click **Continue**
![Install Updates](../../../images/appendix/updates/ftp-update-1.JPG)

###### Updating via GUI for Pantheon.io
For Pantheon.io users, **SFTP** must first be enabled in order for *Update.php* to actually work.
![Update Manager](../../../images/appendix/updates/ftp-update-3.JPG)

##### Ensure Username and Password are correct
![Update Manager](../../../images/appendix/updates/ftp-update-2.JPG)

> **Note** - Pantheon.io users will not see this screen.

![Update Manager](../../../images/appendix/updates/ftp-update-4.JPG)

##### Click **Run database updates**
![Run database updates](../../../images/appendix/updates/ftp-update-5.JPG)

##### Drupal database update
![Finalize database updates](../../../images/appendix/updates/ftp-update-7.JPG)

#### If FTP Access is Unavailable
##### Download the module in need of an update.
##### Open the Drupal installation file directory.
##### Navigate to the module in need of an update in ```/sites``` folder.
##### Delete the old module folder.
##### Unzip the new module folder.
##### Run update.php (*https://mysite.com/update.php*)
**See above**
![Install Updates](../../../images/appendix/updates/ftp-update-1.JPG)

###### Updating via GUI for Pantheon.io
For Pantheon.io users, **SFTP** must first be enabled in order for *Update.php* to actually work.
![Update Manager](../../../images/appendix/updates/ftp-update-3.JPG)

##### Ensure Username and Password are correct
![Update Manager](../../../images/appendix/updates/ftp-update-2.JPG)

Clicking **Continue** will authorize Drupal to automatically install the updates downloaded in the Download step.
> **Note** - Pantheon.io users will not see this screen.
![Update Manager](../../../images/appendix/updates/ftp-update-4.JPG)

##### Click **Run database updates**
![Run database updates](../../../images/appendix/updates/ftp-update-5.JPG)

##### Drupal database update
![Finalize database updates](../../../images/appendix/updates/ftp-update-7.JPG)



### To Install using Drush, a user would:

#### Open a CLI with Drush installed

#### Navigate to an Active Drupal Directory

#### Run ```drush status``` (Just to be safe)
This is a good best practice because there might be issues in need to addressing *before* you attempt to install or update a module.

#### Run ```drush dl <module>```

#### Run ```drush en <module>```

#### Run ```drush updb``` (which is also ```drush updatedb```)

#### DONE!

It really is that simple. Drush removes many of the *repetitive* tasks and simplifies them.
