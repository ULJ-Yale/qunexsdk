# README file for Quantitative Neuroimaging Environment & ToolboX SDK (Qu|Nex SDK)

This repository contains the software development kit (SDK) for the Qu|Nex suite.
The intentions of this SDK is to provide a consistent workflow across research
teams developing the Qu|Nex suite and to kickstart researchers interested in
integrating their own pipelines into Qu|Nex.

The repository consists of three submodules:
* qunexaccept: acceptance tests for Qu|Nex suite releases.
* qunexcontainer: code for building Qu|Nex suite containers.
* qunexdevops: storage of Qu|Nex development related code, notes and materials.

The Qu|Nex code is is co-developed and co-maintained by the:

* [Anticevic Lab, Yale University](http://anticeviclab.yale.edu/),
* [Mind and Brain Lab, University of Ljubljana](http://psy.ff.uni-lj.si/mblab/en),
* [Murray Lab, Yale University](https://medicine.yale.edu/lab/murray/).


Quick links
-----------

* [Website](http://qunex.yale.edu/)
* [Qu|Nex Wiki](https://bitbucket.org/oriadev/qunex/wiki/Home)
* [Qu|Nex SDK Wiki](https://bitbucket.org/oriadev/qunexsdk/wiki/Home)
* [Qu|Nex quick start](https://bitbucket.org/oriadev/qunex/wiki/Overview/QuickStart.md)
* [Qu|Nex container deployment](https://bitbucket.org/oriadev/qunex/wiki/Overview/Installation.md)
* [Installing from source and dependencies](https://bitbucket.org/oriadev/qunex/wiki/Overview/Installation.md)


Versioning
----------

Latest SDK version: 0.5.10

Submodule versions:

* qunexaccept: 0.5.13
* qunexcontainer: 0.62.5
* qunexdevops: 0.2.8


Change Log
----------

* 0.5.10 [qunexaccept qunexcontainer] New conatiner version, HCYA acceptance test upgrade.
* 0.5.9 [qunexaccept qunexcontainer] New conatiner version for hcpDiffusion, fixed some typos in documentation.
* 0.5.8 [qunexaccept] When steps parameter in acceptance tests is set to initial, tests now work properly.
* 0.5.7 [qunexaccept qunexcontainer qunexdevops] Dynamic branch setting when building containers, batch file optimizations, optimized process for opening new features.
* 0.5.6 [qunexaccept] Fixed the batch file for HCPYA acceptance test.
* 0.5.5 [qunexaccept qunexcontainer] Added HCPYA dataset to acceptance tests, container version update.
* 0.5.4 [qunexaccept qunexcontainer] ICAFIx and MSMAll test optimizations, container version update.
* 0.5.3 [qunexaccept qunexcontainer] Acceptance tests now report repository folder, added CUDA Singularity support in the container.
* 0.5.2 [qunexaccept] Scheduler jobname now shows wheter we are running with container or not.
* 0.5.1 [qunexaccept qunexcontainer qunexdevops] Scheduler is now setup the same way as with Qu|Nex, CNP support, FSL 6.0.4, Diffusion support, Optimized order of operations when opening new branches.
* 0.5.0 [qunexaccept] Major update to the RunTurnkey acceptance testing script, which should now work on all environments.
* 0.4.3 [qunexaccept qunexcontainer qunexdevops] Added gitignore, qunexaccept cleanup.
* 0.4.2 [qunexdevops] Optimized opening hotfixes so they auto checkout the hotfix branch on root repository.
* 0.4.1 [qunexaccept] Added all and noT2w acceptance test variants for hcpls data.
* 0.4.0 [qunexaccept] Updated all acceptance test because of the subject to session rename.
* 0.3.3 [qunexaccept] TestRunTurnkey now enables execution of single commands.
* 0.3.2 [qunexaccept qunexcontainer qunexdevops] READNE updates.
* 0.3.1 [qunexaccept qunexcontainer qunexdevops] License updates.
* 0.3.0 [qunexaccept qunexcontainer qunexdevops] Major rework of acceptance testing scripts, new container release, fixed a bug in hotfix opening.
* 0.2.8 [qunexcontainer] New container release.
* 0.2.7 [qunexaccept] Cores and threads rename to parsessions and parelements.
* 0.2.6 [qunexaccept] Upgraded automated RunTurnkey tests and added MSMAll test to stepwise testing script.
* 0.2.5 [qunexdevops] Releases are now based on the develop branch not master.
* 0.2.4 [qunexdevops] Added scripts for openning new SDK features and hotfixes and suite releases.
* 0.2.3 [qunexaccept] Acceptance tests for HCP MSMAll pipelines and a unit test for hcp_suffix.
* 0.2.2 [qunexdevops] Acceptance tests and DevOps scripts are now accessible in the environment.
* 0.2.1 [qunexaccept qunexdevops] Opening a hotfix now stores the environment in the correct environment.txt, removed a typo from the HCPLS_StepwiseTests.sh.
* 0.2.0 [qunexaccept] Complete rework of the acceptance tests repository.
* 0.1.6 [qunexdevops qunexcontainer] Added openhotfix script and integrated ICAFix into the container.
* 0.1.5 [qunexdevops] Adjustments for GitFlow 
* 0.1.4 [qunexdevops] Fixed a bug in status reporting
* 0.1.3 [qunexdevops] Added updated script for creation of own clone and branch
* 0.1.2 [qunexdevops] Adjusted scripts and add one to create new environment
* 0.1.1 [qunexdevops] Change in the environment setup
* 0.1 Initial pre-alpha release
