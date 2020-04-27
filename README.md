# README file for Quantitative Neuroimaging Environment & ToolboX SDK (Qu|Nex SDK)

This repository contains the software development kit (SDK) for the Qu|Nex suite.
The intentions of this SDK is to provide a consistent workflow across research
teams developing the Qu|Nex suite and to kickstart researchers interested in
integrating their own pipelines into Qu|Nex.

The repository consists of three submodules:
* qunexaccept: acceptance tests for Qu|Nex suite releases.
* qunexcontainer: code for building Qu|Nex suite containers.
* qunexdevops: storage of Qu|Nex development related code, notes and materials.

The Qu|Nex code is is co-developed and co-maintained by the 
[Mind and Brain Lab led by Grega Repovs](http://psy.ff.uni-lj.si/mblab/en) 
and the [Anticevic Lab](http://anticeviclab.yale.edu/).


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

Latest SDK version: 0.2.8

Submodule versions:

* qunexaccept: 0.2.5
* qunexcontainer: 0.51.0
* qunexdevops: 0.2.1


Change Log
----------

* 0.2.8 [qunexcontainer] New container release.
* 0.2.7 [qunexaccept] Cores and threads rename to parsessions and parelements.
* 0.2.6 [qunexaccept] Upgraded automated RunTurnkey tests and added MSMAll test to stepwise testing script.
* 0.2.5 [qunexdevops] Releases are now based on the develop branch not master.
* 0.2.4 [qunexdevops] Added scripts for openning new SDK features and hotfixes and suite releases.
* 0.2.3 [qunexaccept] Acceptance tests for HCP MSMAll pipelines and a unit test for hcp_suffix.
* 0.2.2 [qunexdevops] Acceptance tests and DevOps scripts are now accessible in the environment.
* 0.2.1 [qunexaccept qunexdevops] Opening a hotfix now stores the environment in the correct environment.txt, removed a typo from the HCPLS_StepwiseTests.sh.
* 0.2.0 [qunexaccept] Complete rework of the acceptance tests repository.
* 0.1.6 [qunexdevops, qunexcontainer] Added openhotfix script and integrated ICAFix into the container.
* 0.1.5 [qunexdevops] Adjustments for GitFlow 
* 0.1.4 [qunexdevops] Fixed a bug in status reporting
* 0.1.3 [qunexdevops] Added updated script for creation of own clone and branch
* 0.1.2 [qunexdevops] Adjusted scripts and add one to create new environment
* 0.1.1 [qunexdevops] Change in the environment setup
* 0.1 Initial pre-alpha release
