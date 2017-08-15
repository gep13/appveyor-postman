# appveyor-postman

This repository contains a [Postman](https://www.getpostman.com/) collection and environment file that can be used to exercise the [AppVeyor API](https://www.appveyor.com/docs/api/).

To get started with this collection and test that everything is working, after cloning this repository, follow these steps:

1. Open Postman
1. Click Import
1. Click Choose Files
1. Browse to the location where you cloned the repository to
1. Select the `AppVeyor.postman_collection.json` file and click `Open`
1. Click the `Environment Options` gear at the top right hand corner of Postman
1. Click `Manage Environments`
1. Click Import
1. Click Choose Files
1. Browse to the location where you cloned the repository to
1. Select the `AppVeyor Empty.postman_environment.json` file and click `Open`
1. Click the newly imported Environment
1. Edit the name of the Environment as required (for example, to the name of the AppVeyor project you want to work on)
1. Fill in the required information:

    * _accountName_
      * The name of the account that hosts the AppVeyor project you want to work with
    * _projectSlug_
      * The identifier for the AppVeyor project you want to work with
    * _authenticationToken_
      * The API Token of the user that you want to use to access the API.  Log into `ci.appveyor.com` and then select the drop down list at the top right hand corner and click `API Token`.
    * _recordsPerPage_
      * The number of records to return in historical queries

1. Click Update
1. Close the `Manage Environments` window
1. In the collections list on the left hand side, expand `AppVeyor` then `Projects and Builds`
1. Double click on `Get Projects` request
1. In the Environments drop down list at the top right hand corner of Postman, select the Environment that you named earlier
1. Click send
1. If everything has worked, you should get a list of projects for the account associated with the API Token that you used

Feel free to try out the other requests that are included within this collection.