#Lynis Plugin test

Hello, this git centralize information to do your own plugin \o/  

Lynis is a free security audit system (linux) :   
- https://github.com/CISOfy/lynis/
- https://cisofy.com/documentation/lynis/

first you need to clone an existing plugin. Check in /plugin folder, there are 2 plugin
at the install (plugin_template_phase1 and plugin_pam_phase1) or you can check my ;)

#need to now !
Script in sh not bash ! (sorry) If you want to use bash you need to check if /bin/bash is install first.  
Use _phase2 instead of _phase1. Phase 1 is for collecting data. Then normal tests run, and finally phase 2 of the plugins is executed. Phase 1 helps with collecting data used by tests. Phase 2 is for displaying things (like a report).If you want to add data to the /var/log/lynis-report.dat use the "report" function. In _phase2 you can grep data in this file.  
Active the plugin in the default.prf file  

usefull, plugin include function   
- https://github.com/CISOfy/lynis/blob/master/include/functions#L186

#header of the file
```
PLUGIN_AUTHOR=name <name@email.com>
PLUGIN_CATEGORY=what you want
PLUGIN_DATE=date YYYY-MM-DD
PLUGIN_DESC=Description
PLUGIN_NAME=plugin name (use for the activation in the ../default.prf)
PLUGIN_PACKAGE=all  (don't now)
PLUGIN_REQUIRED_TESTS= (don't now)
PLUGIN_VERSION=1.0.0 (version)

Test        : CUST-00XX (number to register plugin)
Description : Description
```

#register your plugin
use the Register function  


#in conclusion
- sh limiting the code ... but you can use /bin/bash (if you test it first).
- create collect plugin (store data in the /vat/log/lynis-report.dat) (_phase1)  
- create check plugin (can use lynis-report.dat) (_phase2)  

a lot of usefull information is in the /var/log/lynis-report.dat (and can be use in the _phase2 plugin) 


#Screen 
![alt tag](https://cloud.githubusercontent.com/assets/8168679/11815492/40858c40-a34c-11e5-9e13-bb0d4daa172d.JPG)

**22 and 3128 is for the exemple ;)**
