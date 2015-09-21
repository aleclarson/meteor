
The `devel` branch represents the version of [meteor/meteor](https://github.com/meteor/meteor)
last used to update each React Native compatible package.

See all available packages [**here**](https://github.com/aleclarson/meteor-client/wiki/Available-Packages).

To check if a specific package is out-of-date (compared to [Meteor's `devel` branch](https://github.com/meteor/meteor/tree/devel)):

```bash
# Make sure the 'upstream' branch is up-to-date
git checkout upstream
git fetch upstream devel
git reset --hard upstream/devel

# See the out-of-date packages
git diff --name-only devel upstream -- packages/*.js
```
