README File for Qu|Nex SDK repository
=====================================

The repository consists of three submodules:
* qunexaccept: acceptance tests for Qu|Nex suite releases.
* qunexcontainer: code for building Qu|Nex suite containers.
* qunexdevops: storage of Qu|Nex development related code, notes and materials.

Versioning
----------
Latest SDK version: 0.1.5

Submodule versions:
* qunexaccept: 0.1.3
* qunexcontainer: 0.1.3
* qunexdevop: 0.1.3

Installation and setup 
----------------------

### Step 1. Clone all Qu|Nex SDK repositories and initiate submodules.

* cd to Qu|Nex $TOOLS folder
* Clone the main repository: `git clone git@bitbucket.org:oriadev/qunex-sdk.git`
* Initiate submodules from inside the cloned repository's folder: `git submodule init`
* Pull and update all submodules: `git pull --recurse-submodules && git submodule update --recursive`
* Checkout master branch for each submodule: `git submodule foreach git checkout master`
* Update submodules to latest commit on the branch: `git submodule foreach git pull origin master`

### Step 2. Configure the Qu|Nex development environment by running the following script

```
$TOOLS/qunexsdk/qunexdevops/environment/qunex_setdevenv.sh
```

Please note that this script will archive the existing .bash_profile and replace it with a new one.


### Step 3. Prepare your development folders

We use the GitFlow branching model (https://nvie.com/posts/a-successful-git-branching-model/, https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow). In GitFlow one should never develop directly on the master branch, all development work should take place at the individual `feature` branches or at the `develop` branch. To set this up follow the instructions below.

Generate the folder `$TOOLS/qunexdev` and repeat Step 1 into this folder, but this time around checkout the `develop` branch.

Generate the folder `$TOOLS/qunexfeatures`, you can create new feature branches or checkout existing ones by using the same procedure as for the `master` and `develop` branches. To enable automated switching between feature branches you should repare a list of environments and store it in `$TOOLS/qunexfeatures/environments.txt`

each line should have three entries:

```
<name of the feature> <folder within $TOOLS where the clone is located> <branch to use>
```

The creation of feature clone and its registration in `$TOOLS/qunexfeatures/environments.txt` is automated using:

```
$TOOLS/qunexsdk/qunexdevops/environment/qunex_openfeature.sh
```


### Step 4. Use the following functions to manage features

* qxreportenv -> to show the current Qu|Nex clone and environment
* qxshowenvs  -> to show the available environments
* qxsetenv    -> to set the desired environment


Qu|Nex SDK Versioning
---------------------

Qu|Nex SDK follows the semantic versioning system (https://semver.org/). 
Given a version number MAJOR.MINOR.PATCH, the increments reflect:

* MAJOR version when backwards incompatible API changes are made,
* MINOR version when new functionality is added in a backwards-compatible manner, and
* PATCH version when backwards-compatible bug fixes are made.

The version history and change log is listed below. The Qu|Nex SDK version of the current release 
is listed in the VERSION file.

* `qunex --version`

Change Log
----------

* 0.1.5 [qunexdevops] Adjustments for GitFlow 
* 0.1.4 [qunexdevops] Fixed a bug in status reporting
* 0.1.3 [qunexdevops] Added updated script for creation of own clone and branch
* 0.1.2 [qunexdevops] Adjusted scripts and add one to create new environment
* 0.1.1 [qunexdevops] Change in the environment setup
* 0.1 Initial pre-alpha release
