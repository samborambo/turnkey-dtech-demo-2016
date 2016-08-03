# Simplified DTech 2016 Repository 
Welcome to the OpenFMB Repo for a simplified microgrid demonstration from the 2016 DistribuTECH Conference.

In the original demonstration on the Distributech floor, multiple vendors were connected over wireless communications to simulate a small microgrid system with actual resource controllers.  

This repository contains the code base of the simplified demo. This demonstration contains OpenFMB CIM data structures and is based on the MQTT publish and subscribe application layer protocol.  This site contains a [WIKI](https://github.com/openfmb/dtech-demo-2016/wiki) for deploying the demo system. 

All code leverages various open source licenses, please refer to the specific module for its LICENSE.txt file.

For futher information requests or for reporting issues please submit an [New Issue](https://github.com/openfmb/dtech-demo-2016/issues/new)


# Demo Project Repo Dependencies

 + openfmb-simulators - https://github.com/openfmb/openfmb-simulators
 + openfmb-hmi - https://github.com/openfmb/openfmb-hmi
 + openfmb-adapters https://github.com/openfmb/openfmb-adapters
 + DNP3 - https://github.com/gec/dnp3
 + Modbus - https://github.com/gec/modbus

# Beta Testing Package

Last update: July 31, 2016

This is an interim package for the simulation and after further testing the final package will be released.  The wiki will then be upgraded.


Requirements:
Follow the dependencies installation from the [wiki](https://github.com/openfmb/dtech-demo-2016/wiki)

You will need to setup your workspace. The following are recommendations:
```
mkdir ~/workspace
mkdir ~/workspace/openfmb
```
Download the latest demo package from the [release tab] (https://github.com/openfmb/dtech-demo-2016/releases)

Untar the demo_stage_<date>.tar.gz in the openfmb directory.
 ```
tar -xzf demo_stage_<date>.tar.gz
```

The wiki information on building the code and setting up the workspace manually will provide general descriptions of files and startup procedures.

To get going fast - go to the stage directory and either one of the following.

```
>./simgo.sh
>./simgoDNP3.sh
```


NOTES:

Remember that all .sh shell script need the executable bit   -> chmod +x <script>.sh
We have included a MQTT-SPY in the distribution for ease in observing publish and subscribe traffic.
We would expect you to install chrome per instructions in the wiki for the web page to automatically startup.
We have a shell script called fetch.sh that will grab the new target files you choose for building the system from the code base.







