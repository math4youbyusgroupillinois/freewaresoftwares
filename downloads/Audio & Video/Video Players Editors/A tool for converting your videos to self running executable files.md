# Download: A tool for converting your Videos to self-running executable files.

**Program name:**

## MakeInstantPlayer 1.60

  
**Thumbshot:** ![](http://www.freewarefiles.com/screenshot/makeinstplyr13_md.jpg)   
  
**Download link:** [Download A tool for converting your Videos to self-running executable files.](http://freesoftwares.boysofts.com/MakeInstantPlayer_program_27606.html)  
  


**Publisher's Description**  
  


MakeInstantPlayer is a tool for converting video files into self-running executables. This is very useful for distributing video clips, as the user doe NOT need any additional software for playback! As MakeInstantPlayer uses the MPlayer engine for playback, it supports almost any video format in existence. 

The user interface is based on MPUI, a very lightweight MPlayer front-end by Martin Fiedler. Furthermore MakeInstantPlayert uses NullsoftA's Scriptable Install System to pack everything into a single EXE file. In order to start playback simply double-click on the Instant Player file and enjoy the show!

* * *
    
    
    MakeInstantPlayer, written by Lord_MuldeR
    Version 1.50, Released 2010-09-18
    
    Using MPlayer SVN-r32198 and MakeNSIS v2.46
    
    
    1. Introduction
    ________________________
    
    MakeInstantPlayer is a tool for converting video files 
    into self-running executables.
    This is very useful for distributing video clips, as the 
    user doe NOT need any additional software for playback!
    As MakeInstantPlayer uses the MPlayer engine for playback, 
    it supports almost any video format in existence.
    The user interface is based on MPUI, a very lightweight 
    MPlayer front-end by Martin Fiedler.
    Furthermore MakeInstantPlayert uses NullsoftA's Scriptable 
    Install System to pack everything into a single EXE file.
    In order to start playback simply double-click on the 
    Instant Player file and enjoy the show!
    
    
    2. Vista Warning
    ________________________
    
    By default MPlayer uses the Overlay (DirectX) renderer 
    for video output on Microsoft Windows.
    On Windows XP the Overlay renderer works flawlessly. But 
    then came Windows Vista. And along with Vista came Aero.
    Aero isnA't compatible with the Overlay renderer, so using 
    the Overlay renderer on Vista MAY cause problems!
    So if you intend to run your Instant Player on a Vista machine, 
    it is recommended to NOT use the Overlay renderer.
    Problems can be avoided by using the OpenGL renderer (-vo gl) 
    or the Direct3D renderer (-vo direct3d) instead.
    Please note that this information applies to the upcoming 
    Windows 7 as well!
    
    
    3. Options
    ________________________
    
    Source File:
      The media file that will be converted into a self-running 
      executable.
      Note that this can be any kind of media file playable in MPlayer, 
      such as AVI, MPEG, MKV or MP4 files.
    
    Output File:
      The executable file that is going to be created. Will be o
      verwritten if already in existence!
    
    Homepage:
      The URL of your homepage. The specified URL needs to start 
      either with "http://" or "https://".
      If you specify an URL, the user will be redirected to that 
      URL when the player exits.
    
    Splash File:
      The image file that will be displayed on the screen while 
      your Instant Player is starting up.
      Supported image types are BMP, GIF and JPEG. The image 
      dimensions shouldnA't exceed the size of a typical screen.
    
    Icon File:
      The icon file that will be used for the executable file. 
      This must be a valid ICO file.
    
    Fullscreen:
      If checked, your Instant Player will start up in fullscreen mode. 
      Hence the video will fill the entie screen.
      Note that this can NOT be used in combination with "compact" mode.
    
    Compact:
      If checked, your Instant Player will start up in compact mode. 
      Hence the windowA's titlebar will be hidden.
      Note that this can NOT be used in combination with "fullscreen" mode.
    
    Auto Quit
      If checked, your Instant Player will terminate immediately after 
      the video playback has stopped.
    
    Stay On Top
      If checked, your Instant Player will stay on top of other 
      windows that are active on the userA's machine.
    
    Loop
      If checked, your Instant Player will replay the media over 
      and over again, until the user stopps playback.
    
    Include Codecs
      If checked, your Instant Player will include the "Binary Codecs" 
      for MPlayer.
      Note that this is usually NOT required. Also this will 
      significantly increase the size of your Instant Player!
      Only some proprietary video formats require these Codecs, 
      formats that should be avoided anyway.
    
    Parameters:
      Here you can specify additional parameters that will be passed 
      to MPlayer. This is intended for advanced users.
      Furthermore you can specify MPlayerA's video renderer here 
      (see the "Vista" chapter for details).
      Note that your parameters will NOT be checked, so wrong 
      parameters may result in serious playback problems!
      Please see the MPlayer documentation for a complete list of 
      all the available parameters.
      
    Language:
      Here you can specify the user interface language of your 
      Instant Player.
    
    
    4. Commandline Usage
    ________________________
    
    The commandline options described in ths section can be used 
    with all "Instant Player" executables.
    
    Please be aware: These option do NOT apply to MakeInstantPlayer 
    itself, only to the executables it creates.
    Also they do NOT apply to MPlayer itself. Do NOT enter them 
    into the "Parameters" edit box!
    
    Basic commandline syntax:
    
      MyInstantPlayer.exe [/?] [/NOSPLASH] [/NOGUI[=]] 
      [/NOHOME] [/EXTRACT[=]]
    
    Available parameters:
    
      /?
        Display an about dialog containing version information 
    	and a list of all commandline arguments.
    
      /NOSPLASH
        Do NOT display the splash screen on startup. This way 
    	the Instant Player will start up much faster.
    
      /NOGUI[=]
        DonA't run the graphical user interface (MPUI). Call 
    	MPlayer.exe directly instead.
        If specified, the additional commandline arguments 
    	 will be passed to MPlayer on startup.
        This option is intended for advanced users only!
    
      /NOHOME
        Do NOT open the hompage in the userA's web-browser 
    	after the playback has terminated.
    
      /EXTRACT[=]
        Extract the media file from the Instant Player executable, 
    	so it can be opened in an external player.
        By default the media file will be extracted to the folder 
    	where the Instant Player executable is located.
        If specified, the media file will be extracted to the 
    	 directory.
        Please note that the Instant Player will NOT play back the 
    	media file when the /EXTRACT argument is used!
    
    Examples:
    
      InstantPlayer.exe /NOSPLASH                         
      Skip the splash screen
      
      InstantPlayer.exe /NOGUI                            
      DonA't use graphical user interface
      
      InstantPlayer.exe /NOGUI=-fs                        
      DonA't use graphical user interface, invoke fullscreen
      
      InstantPlayer.exe "/NOGUI=-vo gl:yuv=2"             
      DonA't use graphical user interface, use OpenGL renderer
      
      InstantPlayer.exe /NOHOME                           
      DonA't visit the homepage after playback has ended
      
      InstantPlayer.exe /NOSPLASH /NOGUI /NOHOME          
      Skip spash screen, donA't use GUI and donA't visit homepage
      
      InstantPlayer.exe /EXTRACT                          
      Extract media file to Instant PlayerA's directory
      
      InstantPlayer.exe /EXTRACT=C:\Temp                  
      Extract media file to the "C:\Temp" directory
      
      InstantPlayer.exe "/EXTRACT=C:\My Documents"        
      Extract media file to the "C:\My Documents" directory
    
    Note that NSIS uses a pretty unorthodox way of dealing with 
    whitespaces in commandline arguments!
    
    
    5. Copyright Information
    ________________________
    
    MakeInstantPlayer
    Copyright (C) 2007-2010 LoRd_MuldeR
    
    MPlayer - The Movie Player
    Copyright (C) 2000-2010 MPlayer Team
    
    MPUI - MPlayer for Windows
    Copyright (C) 2005 Martin J. Fiedler
    
    Nullsoft Scriptable Install System
    Copyright (C) 1995-2009 NSIS Contributors
    
    This program is free software; you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.
    
    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.
    
    
    6. Contact
    ________________________
    
    Future updates for this software will be available from my homepage:
    http://mulder.dummwiedeutsch.de/home/?page=projects#instplay
    
    For help and support, please refer to the corresponding thread on Doom9A's forum:
    http://forum.doom9.org/showthread.php?t=124111
    
    The official MPlayer project homepage can be found here:
    http://www.mplayerhq.hu/
    

  
  
Screenshot: ![](http://www.freewarefiles.com/screenshot/makeinstplyr13.jpg)   
**For more freeware softwares visit [Freeware software downloads.](http://freesoftwares.boysofts.com/)**   
**And [Free softwares and php script downloads.](http://www.boysofts.com/)**
