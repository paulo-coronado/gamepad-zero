                   .:                     :,                                          
,:::::::: ::`      :::                   :::                                          
,:::::::: ::`      :::                   :::                                          
.,,:::,,, ::`.:,   ... .. .:,     .:. ..`... ..`   ..   .:,    .. ::  .::,     .:,`   
   ,::    :::::::  ::, :::::::  `:::::::.,:: :::  ::: .::::::  ::::: ::::::  .::::::  
   ,::    :::::::: ::, :::::::: ::::::::.,:: :::  ::: :::,:::, ::::: ::::::, :::::::: 
   ,::    :::  ::: ::, :::  :::`::.  :::.,::  ::,`::`:::   ::: :::  `::,`   :::   ::: 
   ,::    ::.  ::: ::, ::`  :::.::    ::.,::  :::::: ::::::::: ::`   :::::: ::::::::: 
   ,::    ::.  ::: ::, ::`  :::.::    ::.,::  .::::: ::::::::: ::`    ::::::::::::::: 
   ,::    ::.  ::: ::, ::`  ::: ::: `:::.,::   ::::  :::`  ,,, ::`  .::  :::.::.  ,,, 
   ,::    ::.  ::: ::, ::`  ::: ::::::::.,::   ::::   :::::::` ::`   ::::::: :::::::. 
   ,::    ::.  ::: ::, ::`  :::  :::::::`,::    ::.    :::::`  ::`   ::::::   :::::.  
                                ::,  ,::                               ``             
                                ::::::::                                              
                                 ::::::                                               
                                  `,,`


http://www.thingiverse.com/thing:1635363
RetroPie Zero NES Controller by bfesser is licensed under the Creative Commons - Attribution - Non-Commercial - Share Alike license.
http://creativecommons.org/licenses/by-nc-sa/3.0/

# Summary

This is my design of a replacement back for an original Nintendo gamepad, for use with a Raspberry Pi Zero V1.2,  Raspberry Pi Zero V1.3 (camera), or Raspberry Pi Zero W V1.1 (wireless) running <a href="https://retropie.org.uk/" target="_blank">RetroPie</a>.  I've designed this for genuine NES-004 controllers, so it's probably incompatible with the modern 'retro' hardware from China.  This isn't strictly a remix, but I like to credit those who came before me.

Print with support inside the recesses for the case screws, and depending on how well your printer handles bridging, inside the port openings.  I recommend PLA with 0.4mm extrusion, 0.18mm layers, 2 perimeters, 25% infill.  Taking the outermost perimeter slowly will reduce ringing artifacts on most printers, for cleaner port labels and mushberry.

My favorite cables to use with this:
https://smile.amazon.com/dp/B00DIGCBQY/
https://smile.amazon.com/dp/B018RAW642/

# Post-Printing

Zach from howchoo has written an excellent project guide:
<a href="https://howchoo.com/g/zdqxnzblmzm/gamepad-zero-a-raspberry-pi-retro-gaming-rig-in-an-nes-controller" target="_blank">GamePad Zero: a Raspberry Pi Retro Gaming Rig inside an Original NES Controller</a>

<em>Thanks, Zach!</em>

If the audio isn't coming through to your TV, run the following command:
sudo sed -i '/hdmi_drive=2/s/^#//' /boot/config.txt 

# How I Designed This

Designed from scratch in TinkerCad, you can modify it here:
https://tinkercad.com/things/1mLws3kjBLr

Fusion 360 version:
http://a360.co/2i62ytA

Some of my design considerations (not nearly comprehensive):
- simplicity, rigidity, comfort
- HDMI output near center so it's not awkwardly weighed down on one side
- proper support for PCB under buttons gives the best tactile feel and durability
- assembles without modification to original case top
- compatibility with either revision of the Pi Zero
- thicker than original controller; more comfortable for adult hands
- edge and corner radii matched to original case
- precise off-the-print-bed fit to top-half with no trimming, sanding, etc.
- stainless Torx screws; not inferior Phillips drive [original screws are JIS, not Phillips]
- clearly labeled ports for friends and family who aren't RasPi-holics
- 'Mushberry' RetroPie logo, because it was perfect and the new one sucks
- durable enough for my 3 and 4-year-old nephews

# Legal Notice

## ROMs & Emulation

The boneheads at Nintendo consider <em>any</em> duplication of their ROMs to be illegal, so what you do with this thing is up to you.

https://www.nintendo.com/corp/legal.jsp#roms

That being said, it's compatible with NES, Game Boy, and Game Boy Color games — those requiring only two buttons and a D-pad.

Some free (legal) NES games to get you started [my favorite is <a href="http://forums.nesdev.com/viewtopic.php?p=81978" target="_blank">Alter Ego</a>]:
http://www.nesworld.com/article.php?system=nes&data=neshomebrew_bestof

## Model & Design File Licensing

I've released this model and the design files under a <a href="https://creativecommons.org/licenses/by-nc-sa/3.0/" target="_blank">Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported</a> license.  <em>Please respect the license; I've put countless hours of work into refining these models.</em>  Also, if you happen to see this thing for sale anywhere, please let me know in the comments.