# Creating a BitBucket Account

![BitBucket](../images/unit-1-preparing-your-development-environment/bitbucket/atlassian_logo-lockup-5-a.png)

## Prerequisites

An email address for account verification.

## Goals

* Create an account at *BitBucket.org*
* Open Git Bash
* Learn the basics of SSH Keys and Secure Deployment
* [Generate an SSH Key](https://confluence.atlassian.com/bitbucket/set-up-ssh-for-git-728138079.html "Generate an SSH Key")
* Add SSH Key to your BitBucket Account


## [BitBucket.org/](https://bitbucket.org/ "bitbucket.org")

There are a number of Git repositories online where an account can be created, such as GitHub, BitBucket, and GitLab. They each have their upsides and downsides. What is important for this course it to understand *how* to use the following:

* Git Bash
* Git GUI
* BitBucket.org

That's it.

Real projects in the business world require careful navigation between Branches, Projects, Upstreams, Downstreams, and many other buzzwords. These real-world scenarios though will generally all have two things in common, if using Git: **Documentation** and **Workflow**.

> Because each online Repository is unique, they each have their own naming conventions for common tasks. This curriculum will follow BitBucket terminology, so keep this in mind if choosing to use GitHub or GitLab.

| BitBucket  | GitLab  | GitHub   | Definition  |
| :-------------: |:-------------:| :-----:|:--: |
| Pull Request  | Merge Request   | Pull Request  | This task *pulls* in a specified Branch and applies the differences to the currently active Branch.   |
| Snippet   | Snippet   | Gist   | BitBucket and GitLab definitely have the better definition here. A 'Gist' or 'Snippet' is simply a chunk of code, whether a single script or patch, that is just too small to include within a full repository.   |
| Repository  | Project   | Repository  | The Repository is (should be) your complete Project, from source code to documentation.   |
| Teams   | Groups   | Organizations  | A project is added into Teams (or an Organization) to add group-level Administration. Adding your Git Repository for this class to the Repository assigned by your professor, for example, would add you to the *Team* created for the class and give you access to all *Projects* for that *Team*.  |

## Step-By-Step Account Creation

* **Creating a BitBucket Account**
 * [Step 1 - Create the Account](../manuscript/unit-1-preparing-your-development-environment/creating-bitbucket-account/creating-bitbucket-account_step-1.md "Step 1 - Create the Account")
 * [Step 2 - Create an SSH Key Account](../manuscript/unit-1-preparing-your-development-environment/creating-bitbucket-account/creating-bitbucket-account_step-2.md "Step 2 - Create an SSH Key Account")
 * [Step 3 - Add the SSH Key to BitBucket Account](../manuscript/unit-1-preparing-your-development-environment/creating-bitbucket-account/creating-bitbucket-account_step-3.md "Step 3 - Add the SSH Key to BitBucket Account")

 Congratulations!

 Your local version of Git and remote account on BitBucket are both configured and ready to work with other software packages.... like Drupal!

### What's Next?

Now that your local version of Git and remote BitBucket is completely configured, it's time to create our first Drupal project!

See the next section to create an account with Pantheon.io and begin working with both GitHub and Pantheon together!


## Further Reading
* **Git**
 * [Git-SCM = Pro Git](https://git-scm.com/book/en/v2 "Git-SCM = Pro Git") - The entire Pro Git book by Scott Chacon and Ben Straub (published by Apress) has been made available online as a free resource for interested Git users.
 * [GitHub Guides = Hello World](https://guides.github.com/activities/hello-world/ "GitHub Guides = Hello World") - Taking the **Hello World** approach to learning what Git is and how to use it. For those without programming experience, any time you learn a new language the *first* program you will always create is one that simply prints "Hello World" on the screen.
* [Git-Hub = Generate an SSH Key](https://help.github.com/articles/generating-an-ssh-key/ "Git-Hub = Generate an SSH Key")
* [BitBucket = Generate an SSH Key](https://confluence.atlassian.com/bitbucket/set-up-ssh-for-git-728138079.html "BitBucket = Set up SSH for Git")
* [BitBucket = How to install a public key on your Bitbucket Cloud account]https://confluence.atlassian.com/bitbucket/how-to-install-a-public-key-on-your-bitbucket-cloud-account-276628835.html "BitBucket = How to install a public key on your Bitbucket Cloud account")
