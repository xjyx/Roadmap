=======================================================================
Bugs found in Mint 15 RC
=======================================================================

9 mintSources 
-------------

    - Add-apt-repository missing
    - mintSources doesn’t react to clicking on maximize window button. The border changes a little as if the window is maximizing – but it stays within the same boundaries as before.
    - mintSources window’s minimal width is larger than 1024 so it’s not convenient for testing in 1024×768 and may be an issue for some netbooks
    - When choosing a mirror, clicking on the “Country” column header does nothing, I guess it should’ve sorted it by country instead
    - mintSources doesn’t show when it’s done measuring speeds
    - mintSources seems to get the speed wrong: I get 20 kB/s when fetching the package lists from the mirror that was shown as the fastest one. Or maybe I wasn’t patient enough, but I couldn’t know how long I should wait (see the previous issue)
    - mintSources freezed a couple of times while measuring mirror speeds. Had to kill the application
    - The speed test of sources sometimes seems to take a while, but it’s actually working in the background from my experience. The list is just pretty long, so you have to be a bit patient. On the other hand, one should have to do it only once, right?
    - the mirror speed evaluation software seems to hang indefinitely if (when) it finds an unresponsive mirror. 
        
4 MDM 
-----

    - MDM can't shutdown/restart/suspend
    - "Why can not Bumblebee work with Cinnamon? with MDM login screen.
        When I replace MDM Login Screen with LightDM login screen then it works
        with bumblebee.Bumblebee loads on startup.
        And I can choose the Nvidia card with optirun
        Other operating systems I’ve tried has worked
        Zorin Os works
        Ubuntu works"
    - I confirm the problem with bumblebee. It does not start with mdm but well with any other display manager (lightdm, gdm,…)
    - Enable remote logins via XDMCP causes Xauthority error dialog on login.
    
5 mintInstall 
-------------

    - mintinstall navigation broken in breadcrumb when going to reviews/screenshots
    - mintinstall freezes at startup
    - No explanatory password sentence
    - Interesting, in Software Manager the acroread package has -81 reviews.
    - "It all looks great again, but I can’t get the software manager to work.
        It hangs in the startup-screen, saying it is gathering information on packages.
        Cinnamon 64"
        
5 Cosmetic    
----------

    - ubiquity icon is missing
    - print test page shows ubuntu logo
    - Please update the plymouth theme, its too outdated to match the awesomeness of cinnamom. yes i am talking about the fade-in of the Mint logo, please give it a new design. You can take a look at elementary os Luna’s boot up theme
    - The part in the installation review of LM where it talks about videos shows the included software are VLC,Totem and Video Codecs, only there is no VLC included preinstalled. So you should update the pic to show VLC as featured
    - OMG there is no shutdown plymouth animation! I would like the LM logo from the boot to turn back off just like luna
        
28 Cinnamon 
-----------

    - Cinnamon: dim mai 5 instead of dim 5 mai (MATE gets it right)
    - Cinnamon: Screensaver doesn't forget away_message
    - DND layers in Cinnamon/muffin
    - expo distorts image bg http://imgur.com/Arzksxc
    - The only niggle so far is panel autohide never comes back after hide (Baldr, VBox FWIW).
    - One small remark though, i couldn’t help but notice that the text on title window on top isn’t centered. It looks like it is shifted regarding position of the minimize, maximize and close buttons. Is this intented behavior?
    - Cairo-dock session no longer works out of box, and simply installing it at this time BREAKS CINNAMON, and leaves you with a cairo-dock session with no windows manager by default
    - Show/Hide delay for the panel (in autohide mode) doesn’t work. Didn’t work in LM14, either, btw.
    - Keyboard shortcuts for custom launchers using the Windows key (Super) do not work. (They’re good e.g. for switching workspaces, so in principle they do work.) This was reported months ago, and it’s a little disappointing to see this bug still alive and well.
    - Nemo: If you ‘X’ a file transfer dialog for a large file, there is no way of bringing it back from notification area.
    - "/usr/lib/cinnamon-settings/bin/ExtensionCore.py
        Replace
        showTypes.append([SHOW_ALL, _(""All %s"") % (self.pl_noun)])
        to
        showTypes.append([SHOW_ALL, _(""All %s"").decode(""utf-8"") % (self.pl_noun)])"
    - Do not work themes, desklets, extations and applets. empty window in system settings. sorrow.
    - * Screenshot button doesn’t work?!
    - New nemo is *extremely* cool. Looks amazing but won’t remember the last opened tree location and there is no option to rename folders and files in the save dialog. I don’t know of any other OS that won’t - allow this to be done. If I can create a new file or folder on the spot, I could be able to rename existing files and folders in the location of concern on the fly.
    - I’ve intalled today and it’s awesome, my laptop’s battery life is much longer now, however I’ve found a bug: when I close my laptop I have it configured to suspend, no problem here, but when I open it, the screensaver does not appear and don’t ask for my password. Hope you can fix this before the final release.
    - The Configure cog button doesn’t work in the Desklets area or the Themes selection area. A padlock icon appears too which doesn’t do anything?
    - If you try to set SUPER + E or SUPER + T to home folder and terminal in the keyboard shortcut area, the shortcut will never work. This has really irked me since Mint 13. It’s never been fixed. I’ve reported a bug numerous times.
    - Using ALT and left click won’t move the window (this works in every other version of Linux I’ve ever used. The same is true for ALT + middle click for window resizing
    - * Settings Advanced/Normal button is confusing and it’s toggle setting shouldn’t impact Mint Menu search results IMO. AFAIK if you know what you’re searching for, you shouldn’t need extra steps to see it.
    - why is Keyboard only shown in Advanced Mode? I like to change my keyboard repeat delay to a faster value. This is no advanced thing.
    - it would be nice if I set proxy settings in "System Settings / Networking: Proxy" to set proxy settings also in the files etc/environment and /etc/apt/apt.conf e. g. with a option "set proxy systemwide"
    - Bug with this Cinnamon x64: Wi-Fi access point setup… I click to open and set up for hidden wireless access point, it always closes immediately. Need to fix for hidden wireless access point.
    - The cinnamon brightness and volume icon that appears on screen when I use the keyboard shortcut on my laptop does not show any bar, is that normal? Also, the brightness icon appears and disappears with a noticeable delay while the volume one has no such issue.
    - i was just curious on mint 15 cinnamon is there an option im missing to enable the lockscreen after closing laptop to suspend
    - Desklets luncher only lunches system settings, even if edited to start firefox then it crushes cinnamon
    - when I unistall a theme (right click-unistall), the theme is removed from the list but a new grey pop up window appears and doesn’t dissolve away. to solve I need to restart cinnamon.
    - I can’t reach some settings simply by typing a keyword in the Mint menu like it was possible in the previous versions, ie in Mint 14, when I would type Screen in the mint menu, I could reach the screen manager and manage my dual screens. Now, that setting was hidden in the advanced cinnamon settings and I had a hard time finding it.
    - Theres is a major bug with cinnamon 1.8. I have an nvidia gtx660 video card. In Cinnamon 1.8 vsync does not work
    
8 mintMenu    
----------

    - if you enable GTK “favourites” in MintMenu it wont show them and it tends to bug out a bit until you deactivate them
    - korean doesn't show right in mintmenu http://4.bp.blogspot.com/-as_e0DHueFY/UZMcMVXqV8I/AAAAAAAAGSI/8tIJYnNxkvk/s1600/min-olivia-7.png
    - mintMenu crashed once for no reason (I wasn’t using it at that time)
    - I can’t find the Gnome Network Manager in the Mint Menu, it used to be in 14
    - Cannot edit mintmenu / main menu.
    - My keyboard freezes up when I try using the Super key too often (or Ctrl+Super, as I like to use for mintMenu). When it happens, it seems to think I always have Ctrl pressed down, and trying to use any command that calls `gksu` will cause `gksu` to mention being unable to detect my keyboard.
    - In accessibility, enable OSK and click on MintMenu. Any attempt to enter text into the MintMenu search will close the menu and OSK
    - MATE:  In nearly every other Mint I’ve used, the default view for “Menu” is “Favorites”, however in Mint 15 the first click pops up the “All” Applications menu. Just out of curiosity, why the change?
        
8 MATE    
------

    - Disk utility (gnome-disks) is listed twice in the mintMenu.
    - I would like gnome-system-tools installed as standard in order to be able to add user(s).
    - MATE 64: Every java app with maximized window is unusable, for example josm or jdownloader: menus are not working!
    - MATE 64: Every maximized program, for example eye of mate, shows crap borders in the corner
    - MATE 64: No raw image files thumbnails
    - MATE 64: A standard keyboard shortcut like ctrl alt t for terminal is missing.
    - JAVA problems in MATE: http://forums.linuxmint.com/viewtopic.php?f=47&t=134097&p=720249#p719854
    - I add a drawer to the panel. When I add an applet to the drawer, the drawer icon disappears from the panel. Clicking on the place in the panel where the icon was will show the drawer and the added applet. - The applet will run at this time. Logoff and login and the drawer icon is again showing on the panel, but clicking on it does not show the added applet, so said applet can not be started.
        
1 mintUpdate  
------------
    
    - No explanatory password sentence
        
        
11  System  
----------

    - no sound?
    - gksu doesn’t offer to remember the password. Well, it’s not a new issue, all recent Ubuntu-based Mints are like that, I’m just used to that feature in LMDE. Is there any configuration option I’ve missed?
    - MATE 32: after update im stuck in an ubuntu login screen and cant boot
    - If I hit enter during the countdown the boot menu comes up okay. It’s just if I wait for the countdown to finish that it hangs.
    - Compiz Fusion icon does not start
    - Anyone have an issue using openVPN through the network manager in Cinnamon 15rc 64 bit? Also, I can’t delete any of the VPN entries in Network Manager using the “-”. openvpn connects via command line, though.
    - Synaptic freezes computer, also following the use of apt in terminal. Nothing found in var/logs.
    - Love it great work. I noticed Daniel says HDMI audio is not working for him on nvidia drivers, well, HDMI audio is unfortunately not working for me either (intel hd 4000). When I click in the volume/sound menu on the taskbar there is no option to switch outputs, nor in the regular menu. Hope this gets fixed.
    - On the live system and after install, Network Manager crashes after selecting ‘connect to hidden network’. 
    - apparently medibuntu has been dropped by the maintainer. https://launchpad.net/medibuntu/+announcements
    - Mint-mdm-themes takes way too much space on HDD
        
1 mintDrivers 
-------------

    - Device Drivers/Driver Manager closes straight after launch
                
        
2 Totem
-------

    - First, Totem crashes after it finishes the first song and goes to the next in a playlist or just by pressing the next button to go to the next song. Secondly, it does not display any visual effects rather than a blank screen. The mp3 files are read from a SD card if that matters which I believe is irrelevant.
    - Totem crashes a lot. I tried to download subs with the plugin and as soon as I pressed ‘Play with Subtitle’ it crushed again.
        
        
82 Total   
--------





=======================================================================
Upcoming
=======================================================================

Cinnamon
--------

    - Couldn't find UUID when installing gtile... crash when uninstalling it.
    - Nemo: Add devices to MoveTo/CopyTo context menu
    - Nemo: when the breadcrumb is full, and you use the back button to show the start of it.. the forward button doesn't do anything so you can't get back to the end. Also, the last two items on the first page are not clickable.
    - Desklet position is lost after killing MDM

MDM 1.2
-------
    
    - Performance improvements
    - GDM Greeter: Add a "border" property to "entry" objects so themes can get borders around text fields
    - HTML Greeter: Remove white screen appearing before the theme is loaded
    - HTML Greeter: When there's a lot of languages the whole theme itself gets a scrollbar instead of just the language menu
    
Mint 15
-------

    - UI Improvements for Software Management    
    - Implement nemo actions
    - Nightlife: Upgrade to 1.8, improve the title of the selected window in the scale plugin, improve look of widgets in notifications    
    - Finalize artwork
    - Can't remove software-properties-gtk because apturl requires it (hack apturl to cope with the loss)
    - Check if xterm is needed (by xinit)


=======================================================================
Long term
=======================================================================

Cinnamon 2.0
------------

 - Calendar events - similar to KDE's implementation [lockjs]
 - Configurable color schemes for themes    
 - Upgrade Menu applet with mintMenu features (highlight new apps, install/remove apps, search the Web) [clem]
 - Rethink Cinnamon 2D, fallback to a non-shadow CPU-less intensive session in software rendering mode and/or Muffin/OpenBox (whatever happens, the user should know he's not running the "real" Cinnamon, he should be told why, and he should find himself with a working WM (even a minimalistic one like OpenBox)).
 - Use bumpmaps, make them optional, make compositing optional if possible

    NEW APPLETS
    
    - email notifier (imap/pop)
    - Pulse-like RSS reader
    
    NEW DESKLETS
    
    - System monitor

Nemo 2.0
--------

    - File preview

R&D
---        
    - Add ubiquity features to live-installer (better partitioning, fs support, EFI, OEM..etc)

