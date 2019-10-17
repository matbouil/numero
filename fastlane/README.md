fastlane documentation
================
# Installation

Make sure you have the latest version of the Xcode command line tools installed:

```
xcode-select --install
```

Install _fastlane_ using
```
[sudo] gem install fastlane -NV
```
or alternatively using `brew cask install fastlane`

# Available Actions
## iOS
### ios test
```
fastlane ios test
```
Runs all the tests
### ios build_before_deploy
```
fastlane ios build_before_deploy
```
Build and prepare deployment
### ios deploy_alpha
```
fastlane ios deploy_alpha
```
Deploy a new alpha version (internal) on TestFlight 

This action does the following:



- Ensures a clean git status and checkout from remote branch

- Increment the build number

- Build and sign the app

- Upload the ipa file to hockey

- Commit and push the version bump and build tag
### ios deploy_beta
```
fastlane ios deploy_beta
```
Deploy a new beta version on TestFlight 

This action takes changelog = 'Something new happened' as input parameter

This action does the following:



- Ensures a clean git status

- Increment the build number

- Build and sign the app

- Upload the ipa file to hockey

- Commit and push the version bump and build tag
### ios release
```
fastlane ios release
```
Deploy a new version to the App Store

----

This README.md is auto-generated and will be re-generated every time [fastlane](https://fastlane.tools) is run.
More information about fastlane can be found on [fastlane.tools](https://fastlane.tools).
The documentation of fastlane can be found on [docs.fastlane.tools](https://docs.fastlane.tools).
