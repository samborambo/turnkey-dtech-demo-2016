# Simplified DTech 2016 Repository 
Welcome to the OpenFMB Repo for the simplified demonstration from 2016 DistribuTECH Conference

In the original demonstration on the Distributech floor, multiple vendors were communicating over wireless to simulate a small microgrid system with actually resource controllers.  

This repository is for the code base of the simplified demo.   This site contains a [WIKI](https://github.com/openfmb/dtech-demo-2016/wiki) for deploying the demo. 

All code leverages various open source licenses, please refer to the specific module for its LICENSE.txt file.

For futher information requests or for reporting issues please submit an [New Issue](https://github.com/openfmb/dtech-demo-2016/issues/new)


# Demo Project Repo Dependencies

 + openfmb-simulators - https://github.com/openfmb/openfmb-simulators
 + openfmb-hmi - https://github.com/openfmb/openfmb-hmi
 + openfmb-adapters https://github.com/openfmb/openfmb-adapters
 + DNP3 - https://github.com/gec/dnp3
 + Modbus - https://github.com/gec/modbus

# Beta Testing Package

Last update: July 28th, 2016

This is the interm package for the simulation and after further testing the final package will be released.  The wiki will then be upgraded.


Requirements:
Follow the dependencies installation from the [wiki](https://github.com/openfmb/dtech-demo-2016/wiki)

You will need to setup your workspace. The following are recommendation.
```
mkdir ~/workspace
mkdir ~/workspace/openfmb
```
Download the latest [demo package](https://github.com/openfmb/dtech-demo-2016/releases/download/v1.0_beta/demo_stage_7282016.tar.gz) 

Untar the demo_stage_<date>.tar.gz in the openfmb directory
 ```
tar -xzf demo_stage_<date>.tar.gz
```

The wiki information on building the code and setting up the work space manually will provide general descriptions of files and startup procedures.

To get going fast - go to the stage directory and either one of the following.

```
>./simgo.sh
>./simgoDNP3.sh
```


NOTES:

Remember that all .sh shell script need the executable bit   -> chmod +x <script>.sh
We have included a MQTT-SPY in the distribution for ease
We would expect you to install chrome per instructions in the wiki for the web page to automatically startup
We have a shell script called fetch.sh that will grab the new target files is you choose to build the system from the code base.







