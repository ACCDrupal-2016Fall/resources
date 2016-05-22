# Creating a GitHub Account
## Step 2 - Create an SSH Key

SSH keys are the digital versions of the car-clicker that unlocks your car as you approach it.
Instead of plugging the key into the door (aka: typing a password), you instead create a keycard called an **SSH Key** and add a copy of the Public version to GitHub. Their computers will compare the Public version they have with the Private version you have, then unlock the car!

> Just like with your real car, you don't have to know **how** the clicker unlocks the car. You should instead know that it **does** unlock the car.

### Generating an SSH Key

> The ```~/``` means "current user's root folder" or "your home folder". This is important because the files created at ```~/.ssh``` are only visible and available to you and people who have Administrator access to the computer where it was installed.

> This means that all SSH Keys should be removed from your GitHub account at the end of the Semester, just to be safe!

#### Check for existing SSH Keys
It is always best to check for existing SSH Keys before starting *any* project. Especially if creating a new project on a computer you have never logged into before. If a Key already exists, contact your Administrator immediately because there is probably a virus on the computer.

#### Generate the SSH Key
* Open Git Bash
 <placeholder>
* Enter this command: ```ssh-keygen -t rsa -b 4096 -C "your_email@example.com"```
 <placeholder>
* When prompted for a location to place the file, just press Enter.
 <placeholder>
* When prompted, enter a passphrase, for security.
 <placeholder>

#### Add the SSH Key to ```ssh-agent```
Git for Windows and Git Bash come with a useful tool called ```ssh-agent```.

This useful package locally stores *your* SSH information so that you do not have to input your GitHub password each time you ```push``` or ```pull``` content from GitHub.

* Turn on the ```ssh-agent```
 <screenshot>
* Add SSH Key to ```ssh-agent```
 <screenshot>
