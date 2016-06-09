# Extending Drupal

As we have discussed, one of the greatest strengths of Drupal is just how *modular* and *extensible* it is. Drupal has thousands of Community contributed *extensions* spread between both modules and themes.

During this course, Students will actually create their **own** extensions (both modules and themes). These extensions require a relatively simple process for installation.

To **use** these extensions however, they must first be installed. Throughout the course, you will receive the instruction *'Install <this> module'* or *'Install <this> theme'*. It will be assumed that you know the basics of *installing* each extension, whether a module or a theme (though we will not touch on themes until **Unit Three**).

If you need a review at any time, do not hesitate to review the steps below for installing modules.

## Challenge!

### Installing Modules

> **Best Practices** - Instructions are included here for installing/updating modules via the Administrative Interface. These actually are often much simpler and faster using tools like *Drush*, which is what we will be using in-class.

#### Keeping in line with the concept of **modularity**, there are multiple options for installing a module in Drupal:
1. **Install via the Graphic User Interface (GUI) while logged into the site.**
2. **Install via Drush**
3. Install via Drupal Console
4. Install via Secure File Transfer Protocol (SFTP) and the Command Line

For this course, we will review both installation via the GUI and installation via Drush (which is much, **much** faster!).

> **Note** - Drush and Drupal Console are only *two* of the many Drupal Developer Tools. [Pantheon.io's](https://pantheon.io/ "Pantheon.io's") [Terminus](https://github.com/pantheon-systems/terminus "Terminus"), for example, supports a number of Drush commands while supporting a CLI version of Pantheon's Developer Dashboard.

> **Best Practices** - SFTP using tools like [FileZilla](https://filezilla-project.org/ "FileZilla") has been an available method of file-system management since the inception of Drupal, but has never been the **best** method of file management. By using enforced version control through Git, there are no **quirky** files hidden somewhere in the Nether corrupting the entire system. See Section 6.3: WSOD - The "White Screen of Death" Errors for some of the more common issues that can arise by using this method of file control.

### Graphic User Interface (GUI) method

##### Find the FTP/URL link for the desired Module
##### Navigate to the **Modules** (*https://mysite.com/admin/modules*) link
##### Click **Install new module** (*https://mysite.com/admin/modules/install*)
##### Paste the link (if FTP access is available)

### Installing Themes
See Unit Three - Section III: The Drupal Theme Engine (unwritten)

## Step-by-Step Module Installation
### GUI Module Installation
* [Step 1 - Download CTools](../manuscript/unit-1-preparing-your-development-environment/installing-modules/installing-modules_1.md "Section 1.10.1: GUI : Step 1 - Download CTools")
* [Step 2 - Install CTools](../manuscript/unit-1-preparing-your-development-environment/installing-modules/installing-modules_step-2.md "Section 1.10.1: GUI : Step 2 - Install CTools")
* [Step 3 - Configure CTools](../manuscript/unit-1-preparing-your-development-environment/installing-modules/installing-modules_step-3.md "Sect3on 1.10.1: GUI : Step 3 - Configure CTools")

### Drush Module Installation
* [Drush : Step 1 - Download CTools](../manuscript/unit-1-preparing-your-development-environment/installing-modules/installing-modules_step-4.md "Drush : Step 1 - Download CTools")
* [Drush : Step 2 - Install CTools](../manuscript/unit-1-preparing-your-development-environment/installing-modules/installing-modules_step-5.md "Drush : Step 2 - Install CTools")
* [Drush : Step 3 - Configure CTools](../manuscript/unit-1-preparing-your-development-environment/installing-modules/installing-modules_step-6.md "Drush : Step 3 - Configure CTools")


## Further Reading
