#Lynis Plugin test

Hello, this git centralize information to do your own plugin \o/  

Lynis is a free security audit system (linux) :   
- https://github.com/CISOfy/lynis/
- https://cisofy.com/documentation/lynis/

first you need to clone an existing plugin. Check in /plugin folder, there are 2 plugin
at the install (plugin_template_phase1 and plugin_pam_phase1) or you can check my ;)

#need to now !
script in sh not bash ! (sorry)  
use _phase2 instead of _phase1 in the name of the plugin. phase1 is for plugin who do nothing (wtf) ... who do thing but show nothing :D

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

Test        : PLGN-00XX (number to register plugin)
Description : Description
```

#register your plugin
use the Register function  


#in conclusion
sh limiting the code ...   

a lot of usefull information is in the /var/log/lynis-report.dat  


#Screen 
![alt tag](https://cloud.githubusercontent.com/assets/8168679/11815492/40858c40-a34c-11e5-9e13-bb0d4daa172d.JPG)
