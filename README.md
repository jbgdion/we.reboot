# weeBoot


**DESCRIPTION**

weeBoot is a utility program that shows the remaining time before it restarts the computer.
Default countdown timer is 60 minutes. User can change the time of the restart. The countdown timer will automatically update when the user changes the restart time. 
At less than 30 minutes, it will automatically pop up every 10 minutes as a reminder. At less than 5 minutes, it will be fixed at the bottom right corner. 
All buttons will be disabled except restart. Restart time will be limited to 11:59 PM if the program runs before 5:00 PM. 
If the program runs after 5:00 PM, the hour selection is extended by 8 hours to accommodate work shift. 
The header image can be customized by placing a logo.png file with a size of 350 x 40 pixels.

![This is an image](https://github.com/jbgdion/we.reboot/blob/main/weeboot.png)

Please contact me mobiuxer@gmail.com if you want to use this utility. 


**Usage:**

weeBoot.exe [-lastreboot:n] [-timer:n] [-force] [-float] [-nogui] [-poweroff]

   -lastreboot:n 
  
      Where n is number of days. Default is 0.
    
  -timer:n Where n is number of minutes to countdown.
  
      Default is 60 minutes. Minimum is 15 minutes.Maximum is 360 minutes.
  
  -float Shows title bar at the start to allow moving of the window.
    
  -force Prevents user from changing reboot time.
  
  -nogui No window pop up. No countdown timer. 
      
      Program exits when a user is logged in.
      When no user is logged in, it automatically reboots the computer.
      This option ignores -timer and -float options.
      
  -poweroff Shuts down and powers off the computer. Works only with -nogui option
  

**Example:**

    weeBoot.exe -lastreboot 30
      
       Shows the restart window with the default 60 minute countdown if computer is not rebooted more than 30 days

![This is an image](https://github.com/jbgdion/we.reboot/blob/main/weeboot.gif)
