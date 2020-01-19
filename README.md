README File for Qu|Nex SDK repository
=====================================

The repository consists of three submodules:
* qunexaccept: acceptance test for testing new versions of Qu|Nex before releases.
* qunexcontainer: code for building Docker and singularity Qu|Nex containers.
* qunexdevops: storage of Qu|Nex development related code, notes and materials.


Installation and setup 
----------------------

### Step 1. Clone all Qu|Nex SDK repositories and initiate submodules.

* cd to Qu|Nex $TOOLS folder
* Clone main repository: `git clone git@bitbucket.org:oriadev/qunex-sdk.git`
* Initiate submodules from inside cloned repo folder: `git submodule init`
* Pull and update all submodules: `git pull --recurse-submodules && git submodule update --recursive`
* Checkout master branch for each submodule: `git submodule foreach git checkout master`
* Update submodules to latest commit on the branch: `git submodule foreach git pull origin master`

### Step 2. Configure the Qu|Nex development environment by running the following script

```
$TOOLS/qunex-sdk/qunexdevops/environment/qunex_setdevenv.sh
```

Please not that this script will archive the existing .bash_profile and replace it with a new one.


### Step 3. Prepare your environments

Generate folder `$TOOLS/qunexdev`

In that folder create clones of Qu|Nex that you would work on

Prepare a list of environments and store it in `$TOOLS/qunexdev/environments.txt`

each line should have three entries:

```
<name of the environment> <folder within $TOOLS where the clone is located> <branch to use>
```

### Step 4. Use the following functions to manage environments

qxreportenv -> to show the current Qu|Nex clone and environment
qxshowenvs  -> to show the available environments
qxsetenv    -> to set the desired environment


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

* 0.1 Initial pre-alpha release.
* 0.1.1 [qunexdevops] Change in the environment setup.
* 0.1.2 [qunexdevops] Adjusted scripts and add one to create new environment.
* 0.1.3 [qunexdevops] Added updated script for creation of own clone and branch
