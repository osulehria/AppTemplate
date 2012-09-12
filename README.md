AppTemplate for Rally SDK 1 and 2
=========================

## Overview

This Rakefile can be used to create a skeleton Rally app for use with Rally's App SDK 1 and 2.  You must have Ruby 1.9 and the rake gem installed.

The normal workflow for creating an App is to start by creating an App with the new task.

Available tasks are:

    rake new[app_name,sdk_version]  # Create an app with the provided name (and optional SDK version, defaults to 2.0p3)
    rake debug                      # Build a debug version of the app, useful for local development. 
    rake build                      # Build a deployable app which includes all JavaScript and CSS resources inline. Use after you app is working as you intend so that it can be copied into Rally.
    rake clean                      # Clean all generated output
    rake jslint                     # Run jslint on all JavaScript files used by this app
    rake deploy                     # Deploy the app to a Rally server
    rake deploy:debug               # Deploy the debug app to a Rally server
    rake deploy:info                # Display deployment information
    

## Differences between creating SDK 1 apps vs SDK 2+ apps

The development process for each SDK is different (SDK 1 uses Dojo and SDK 2 uses ExtJS) but there shouldn't be any problems with using the Rakefile to create, build, and debug apps.

There only thing that isn't currently working is the rake:deploy options for SDK1 apps.

## License

AppTemplate is released under the MIT license.  See the file [LICENSE](https://raw.github.com/RallyApps/AppTemplate/master/LICENSE) for the full text.
