# mbcounter 

I like to work on my laptop via LTE services, this allows me to work on all my stuff anywhere. But since I'm not rich yet I have to watch my internet usage, and 
since I couldn't find any linux package that displayed the cumulative data usage and can limit it, I decided to write my own. Obviously it's a little bare atm but thats bc i have no idea 
how this stuff works yet. A couple updates further down the line and its a proper package downloadable via github. 

### Functionality 
  - [x] limiting internet usage; deactivating internet connection at a preset value (-l).
  - [x] present user with cumulative data usage & bandwidth usage per second
  - [ ] notifying the user; through audiovisual channels at a preset value (-n). 
  - [ ] gui in ncurses; indicative colours and a progress bar. 
  - [ ] a reset function, at -r <minutes> the quotum stays the same but the counter drops to 0 mb's 

### Tips
psutil is required, when using manjaro use:
```
sudo pacman -S python-psutil
```

usage:
```
gc -l [limit in mb's: float] -n [mb's for notification: float]
```

### Disclaimer
The information displayed might not be accurate.
