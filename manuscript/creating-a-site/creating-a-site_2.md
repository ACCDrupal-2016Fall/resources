# Creating Your First Site

## Step 2 - Installing Your First Site

### Navigate to Pantheon.io Dashboard
![MySite.Pantheon.io](../../images/creating-a-site/creating-a-site_2-1.JPG)

### Click **Your Site**
![Create New Site](../../images/creating-a-site/creating-a-site_2-2.JPG)

### Click *Visit Development Site*
![Visit Development Site](../../images/creating-a-site/creating-a-site_2-3.JPG)

### Configure Your Site

#### Choose Profile
The profile has already been chosen through Pantheon.io's "Upstream" repository method, so it will be the only Distribution available.

> **Note** - If choosing one of the other Distributions, multiple Installation Profiles may be available.

![Choose Profile](../../images/creating-a-site/creating-a-site_2-4.JPG)

#### Choose Language
Drupal has *extensive* Multilingual support for Site Administration **and** content generation. Students are encouraged to explore multilingual possibilities under their own initiatives.

#### Verify Requirements
Because we are installing on Pantheon.io, we have little worry for the requirements needed.

> **Note** - Drupal 7 requires PHP 5.3, whereas Drupal 8 requires a minimum of PHP 7.0. Some **extensions** however may have an increased requirement for full functionality.

#### Set up database
When working locally, the settings.php file and local-settings.php files will need to be configured prior to reaching this step.

> **Best Practices** - Some Web Authors/Developers recommend using settings.local.php or local.settings.php for securing your private content. The choice is not important as long as the file is included and this line is included in <root>/sites/default/settings.php

````php
if (file_exists(__DIR__ . '/local-settings.php')) {
  include __DIR__ . '/local-settings.php';
}
````

This is some generic PHP telling Drupal (through ```settings.php```) to check the local directory for any files named ```local-settings.php``` and, if the file exists, to load it as if it was *part* of ```settings.php```.

#### Install profile
As a reminder, this was chosen through Pantheon's Site Creation tool, which is not "build-in" to Drupal. Because of the *Modularity* of Drupal though, Students were able to choose their installation profile prior to *starting* their installation. *Modularity* is such a great addition to any Web Author's tool-belt.

Because of this, Pantheon skips straight through and installs the chosen profile, including all required modules!

#### Configure Site
![Configure Site](../../images/creating-a-site/creating-a-site_2-5.JPG)

| **Enter the Following:**  |
| :-------------: |:-------------:|
| **Site Information**  |
| *Site name*  | Choose an appropriate Site name. For this class, use your Pantheon chosen site-name https://**mysite**.pantheon.io/  |
| *Site e-mail address*  | This is the *Administration* email address. Notices about Security Updates, Error Reports, Logs, etc. will be sent to this email address.   |
| **Site Maintenance Account**  |
| Username  | Also known as *UID 1* throughout the Drupal Community, the Site Maintenance Account is the *initial* Super-Duper-In-Charge Administrator account created when your Drupal site is created. This can be changed later.  |
| E-mail address  | Not to be confused with the *Site e-mail address* above, this email address is attached to the User account created for UID 1. See **USER ACCOUNTS (EDIT THIS)** for more information on UID 1.  |
| Password  | Because this account will have **full** access to your site, a highly complicated password is recommended.  |
| Server Settings  |
| Default country  | Set this to the Default country where the site will be accessed *primarily*.  |
| Default time zone  | Also set this based on the *primary* user-access. If your Portfolio is set to run [Cron](https://www.drupal.org/cron "Cron") at midnight and you choose a control halfway around the world, your site may just be down for maintenance at a vital moment (when that employer is checking your website!).  |
| Update Notifications  |
| Check for updates automatically  | This should always be enabled. Advanced Users may disable it when created custom Drupal Distributions or other similar high-level tasks.  |
| Receive e-mail notifications  | This question is for the *Site e-mail address* and will only sent out email such as Security Update notices, Site Issues, etc.  |

### Congratulations, you installed Drupal!
![Congratulations, you installed Drupal](../../images/creating-a-site/creating-a-site_2-6.JPG)
You have successfully *created* Your First Site!

Now, let's *Visit your new site*!
