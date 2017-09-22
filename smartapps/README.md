# SmartApps
This section contains various SmartApps for SmartThings Hub.


## Switch Command Repeater
[SwitchCommandRepeater](jbienz/switch-command-repeater.src/switch-command-repeater.groovy) allows [Switch](http://docs.smartthings.com/en/latest/capabilities-reference.html#switch) commands to be repeated a configurable number of times. This is handy for switches that do not accurately report their status and sometimes need to be commanded multiple times in order to reach a desired state. For example, it can be used with the [Somfy ZRTSI](http://a.co/gTMFagf) blind controller (which does not support command confirmation) to ensure the blinds actually respond.

#### Options
**Switch to manage:** The switch that should be monitored.

**Number of times:** The number of times that each command should be repeated. Min: **1** Max: **Unlimited**. Recommend **3** for the ZRTSI.

**Seconds between repeats:** How many seconds to pause between each repeat of the command. Min **1** Max: **Unlimited**. Recommend **2** for the ZRTSI.



## Installing Custom SmartApps
The links in each section above (e.g. [SwitchCommandRepeater](jbienz/switch-command-repeater.src/switch-command-repeater.groovy)) point to a file with the **.groovy** extension. These files contain the SmartApp logic.

#### To install: 

1. Open one of the links above to the SmartApp you want to install
1. Click the Raw button to view the raw source code for the SmartApp
1. Select everything in the window and copy it to your clipboard
1. Log into [https://graph.api.smartthings.com](https://graph.api.smartthings.com) with the same credentials you use for your SmartThings hub
1. Click "SmartApps"
1. Click "New SmartApp"
1. Click "From Code"
1. Paste the code from step 3 above
1. Click "Create"
1. Click "Save"
1. Click "Publish"
1. Click "For Me"