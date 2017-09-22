# SmartApps
This section contains various SmartApps for SmartThings Hub.


## Switch Command Repeater ##
[SwitchCommandRepeater](jbienz/switch-command-repeater.src/switch-command-repeater.groovy) Allows [Switch](http://docs.smartthings.com/en/latest/capabilities-reference.html#switch) commands to be repeated a configurable number of times. This is handy for switches that do not accurately report their status and sometimes need to be commanded multiple times in order to reach a desired state. For example, it can be used with the [Somfy ZRTSI](http://a.co/gTMFagf) blind controller (which does not support command confirmation) to ensure the blinds actually respond.

#### Options ####
**Switch to manage:** The switch that should be monitored.

**Number of times:** The number of times that each command should be repeated. Min: **1** Max: **Unlimited**. Recommend **3** for the ZRTSI.

**Seconds between repeats:** How many seconds to pause between each repeat of the command. Min **1** Max: **Unlimited**. Recommend **2** for the ZRTSI.