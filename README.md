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

#in conclusion
sh limiting the code ... 

a lot of usefull information is in the /var/log/lynis-report.dat


