# Github Guide
A guide to use GitHub


### Git Global Configuration

* **For just one repo:**
``` html
git config user.name "Your Name Here"
git config user.email your@email.com
```

* **For (global) default email (which is configured in your ~/.gitconfig):**
``` html
git config --global user.name "Your Name Here"
git config --global user.email your@email.com
```

* **For check configuration:**
``` html
git config --list"
```

```php
popopopopopo popoponm klklklklklklklklklk
<php?                                        >
```

---
### Setup GIT with SSH Key
* **Step 1** Download GIT Bash [from here.](https://git-scm.com/downloads) & Install with recommended settings.
* **Step 2** Open Gitbash
* **Step 3** SSH key generate :point_right: **ssh-keygen -t rsa -b 4096 -C "email"** [*-t: type; -b: bytes; -C: require email address*]
* **Step 4** After enter key generate command it will ask **Enter passphrase (empty for no passphrase)**
* **Step 5** Start SSH Agent :point_right: **eval $(ssh-agent -s)** [*Example: It will return Agent pid 1007*]
* **Step 6** Add your SSH private key to the ssh-agent :point_right: **ssh-add ~/.ssh/id_rsa**
* **Step 7** Copy public key to clipboad :point_right: **clip < ~/.ssh/id_rsa.pub** [*This command will automatically copy the key*]
* **Step 8** Open and login to github and go to **settings** :arrow_right: **SSH and GPG keys** or after login click [here.](https://github.com/settings/keys)
* **Step 9** Click on New SSH Key. Give a Title, Paste key in Key input and Save.

**Git SSH key setup done.**
