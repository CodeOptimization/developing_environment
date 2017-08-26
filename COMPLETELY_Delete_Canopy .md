# developing_environment

Recently, I have been using Jupyter and it seems conflict with my Canopy. So I decide to uninstall the Canopy.


1. I followed the stemp from https://support.enthought.com/hc/en-us/articles/204469700-Uninstalling-and-resetting-Canopy-v1; 
which does not work. I was really upset about this, since Canoy want me to keep a couple of folders left. Why would I keep them while I'm 
deleting?!

2. I mannuly delete the folder: /users/name/Library/Enthought. Then I got a wired suggestion when starting the Terminal: "-bash: /Users
/MyName/Library/Enthought/Canopy_64bit/User/bin/activate: No such file or directory"

3. Then I dive into my ~/.bash_profile file and luckily, find the last sentence: 
  * #Added by Canopy installer on 2014-02-11
  * #VIRTUAL_ENV_DISABLE_PROMPT can be set to '' to make bashprompt show that Canopy is active,       otherwise 1
  * VIRTUAL_ENV_DISABLE_PROMPT=1 source /Users/MyUserame/Library/Enthought/Canopy_64bit/User/bin/activate"
Just delete it.

4. type _source ~.bash_profile_ int terminal, fixed.
