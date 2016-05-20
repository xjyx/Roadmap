	Linux Mint 18 Sarah
	===================

        update translations
        update linuxmint-keyring (and sign live repo)
        consider enabling recommends

        [done] mate-terminal lacks prompt colors
        [done] hide imagemagick
        [done] hide openjdk8
        [done] mintmenu favorites

        terminal:
            no transparency?
            no new tab option in context menu

        firefox:
            update bookmarks (remove community or put it at the end)
            update DDG search engine
            consider not using default profile

        artwork:
            update default background in mint-artwork-gnome
            mint-backgrounds-sarah

        mintupdate:
            thicken numbers in status icons

		System:
            Upgrade path from Mint 17.3

		cinnamon 3.0:
            menu doesn't seem to always update itself when installing/removing applications
            upgrade issue? users reported dist-upgrade from Betsy vanilla to Cinnamon 3.0 removed the cinnamon package
			menu: search on non-accentuated versions (for instance, "method" should find mintlocale's im in French)

Maintenance
===========

	cinnamon-spices website:
        reimplement css
		handle utf-8, see comments on http://cinnamon-spices.linuxmint.com/applets/view/171

    upgrade LO to 5.0.6?

    betsy: 3rd Cinnamon 3.0 update pack

Linux Mint 18.1
===============

    system
        consider adding snapd

    cinnamon 3.2
        vertical panels
        retire boxpointers
        remove plug/socket in screensaver
        applets
            menu: adopt this layout (https://raw.githubusercontent.com/The-Panacea-Projects/Gnomenu/master/Screenshot.png), same as ours/mintmenu, only better.
            add a printer applet
        sound: add an option to switch sound to HDMI when an HDMI output device is plugged
        hidpi issues: top of mint menu is cut off in HiDPI (1920×1280)
        gnome-system-monitor moves out of place in Expo
        when battery is very low, battery icon isn't red.. 2% charge, with less than 5 minutes to go, still not red.. bar is red in CCC, icon is red in notification.. but not in applet (and also not in the CCC icon itself either)
        When using Cinnamon bar at top, and secondary monitor with higher height than the main display, some apps like KDE Apps (Krita, Kdenlive) or Wine Based Apps (teamviewer) will display menus from toolbar in the wrong place. Being more specific: The menus will be displayed in the position that they should be displayed at main monitor, however in this case the window is maximized in the secondary monitor.
        accessibility: ability to select files by hovering them
        menu: use search providers to search local files

    mate 1.16
        swith MATE to GTK3
        switch mintmenu to GTK3
        sound events vs sound themes
        multi-monitor: caja doesn't always show the desktop on the primary monitor (using a laptop as main/left monitor, and HDMI screen with higher res on the right, it surprisingly ends up showing icons on the right screen)

    libindicator++?

    xed
        sublime-like search bar

    mintupdate:
        provide a CLI (to let people upgrade automatically)

    gtk3:
        mintsources

    mintwelcome:
        hidpi: don't use 32px png icons

    mintlocale:
        hidpi: don't use fixed-size flag icons

    mintupload:
        use icon names rather than path to SVG

    mintsources:
        port to GTK3
        Select all button in foreign pkgs: https://github.com/linuxmint/mintsources/issues/59

    mintinstall:
        when apt cache is missing, it just says not available. Instead it could tell the user or even help the user to refresh the cache.
        port to GTK3
        redesign main page to feature essential apps

    use aptdaemon?
        aptdaemon doesn't work in LMDE and is being abandoned upstream
        in mintupdate, remove dep on synaptic, remove admin rights for checkAPT.py
        in mintwelcome and codec menu entry, switch from apturl to aptdaemon
        in mintsources, remove dep on synaptic
        remove synaptic from default selection
        remove synaptic from mintmenu's favorites


LMDE +1:
=========

    bashrc: # colored GCC warnings and errors --> export GCC_COLORS='error=01;31:warning=01;35:note=01;36:caret=01;32:locus=01:quote=01' (won't work until gcc 4.9)
    update grub (improves efi support)
    history and completion in bashrc
    install libhal1-flash by default
    consider activating http://backports.debian.org/changes/jessie-backports.html
