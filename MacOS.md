```sh
# Hide the other username in login screen

# All the above posts, are various sides of the truth on this topic. Pay attention especially to the points made by John Lockwood and Old Toad.
# Yes, it is possible to do it like you want to. It is also possible to revert back. In what is other user in login window? the method has been covered. It is also possible for it not to display the login name at startup, but then the Mac has to be bounded to an OD and the User login's used above 1000, ie Network Users. That removes the security concern raised by Old Toad in a way.
 
# Instead of what Linc has reccommended, you will enter:
 
sudo defaults write /Library/Preferences/com.apple.loginwindow SHOWOTHERUSERS_MANAGED -bool FALSE
 
# and to revert:
 
sudo defaults write /Library/Preferences/com.apple.loginwindow SHOWOTHERUSERS_MANAGED -bool TRU
```