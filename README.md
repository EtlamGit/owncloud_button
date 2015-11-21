# owncloud_button
ownCloud 'Log in' screen with separate button below the credentials forms.

## Motivation
As of [ownCloud](https://www.owncloud.org) 8.2.0 the former log in button was removed and embedded inside the password form. This is a decision of the [ownCloud design team](https://owncloud.org/contribute/design/) and very unlikely to be reverted. As I personally prefer to have a separate button for usability reasons, some convenient way was needed to get the button back. It is not well seen to clutter the ownCloud configuration with tons of parameters that affect the GUI, therefore only modification of the personal ownCloud instance is possible. But these changes have to be redone for every release of ownCloud. To keep track of my changes I created this repository. And of course I hope to get help and verification from others.

## How to use
This repository holds separate branches for each version of ownCloud. Files contained in a branch should replace the originally shipped ones in the personal ownCloud installation:

```
# clone this repository
git clone https://github.com/EtlamGit/owncloud_button
cd owncloud_button

# get list with all supported ownCloud versions
git tag

# checkout the version matching your ownCloud version
git checkout v8.2.0

# replace files and ensure file rights
sudo cp -r core /var/www/owncloud/
sudo chown -R root:www-data /var/www/owncloud/core
```

## Disclaimer
You are free to use the files in this repository for your cloud. But I do not guaranty to update to each and every version of ownCloud. And update will be much later than official releases.

## License
The original sources are provided by the [ownCloud project](https://github.com/owncloud/core/). As they use the GNU Affero General Public License, all modified files provided here are most likely also to be provided with that license.
