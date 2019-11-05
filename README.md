# PureThermal2 Testing

Screen capture of VLC Media Player during first use of PureThermal2

![](images/screenshot.jpg)

This was taken on a windows 10 computer.

## Connecting to the Device using VLC Media Player

I have no prior experience with VLC Media Player. The following shows how I connected to the device.
Note this gave a slow update of about one frame a second. Changing some setting will likely speed that up.

![](images/vlc-open01.jpg)

![](images/vlc-device.jpg)

## Inserting Camera into Board
 
Used image at [https://groupgets.com/manufacturers/getlab/products/purethermal-2-flir-lepton-smart-i-o-module](https://groupgets.com/manufacturers/getlab/products/purethermal-2-flir-lepton-smart-i-o-module)
to get correct orientation of module in socket. 
 
![](https://groupgets-files.s3.amazonaws.com/PT2/PT2_Description_Diagram.png)
 
### Anti-static Precautions

Used anti-static strap plugged into ground.

Also used sheet of black anti-static foam grounded at one corner as a mat.

### Concern about retaining Camera Module in Socket

The thermal Camera Module was carefully inserted in the socket and so far it does not appear to be ready to just fall out; however I have read concerns about 
that possibility. I decided to look for any recommendations on mounting the camera module and the camera board before proceeding to avoid any missteps 
(since the module is about $300 CAD).

found at [https://groupgets.com/manufacturers/getlab/products/purethermal-2-flir-lepton-smart-i-o-module]

~~~~
    b-cubed  Tom • 3 months ago
    Yes, I talked to FLIR. They pointed out page 68 of their FLIR LEPTON® Engineering Datasheet where it shows that 
	the Lepton is meant to be retained in the socket by a gasket / window / cover. The assumption is that the 
	Lepton will need to be protected from environmental hazards.

    While waiting to get through to FLIR I purchase another Lepton and PureThermal-2 (as well as some Molex sockets) 
	to see what I could learn about the socket retention. After inspecting the hardware and talking to the FLIR support 
	people, it is clear that the intent is that the socket holds the Lepton in place, but only in a tentative way.
~~~~

The FLIR LEPTON Engineering Datasheet mentioned is here:
[https://www.flir.com/globalassets/imported-assets/document/flir-lepton-engineering-datasheet.pdf​] 

It says: (page 68)

~~~~
    6.2 Mechanical Considerations The socket described in Socket Information on page 66 is not intended 
	    to retain the Lepton assembly under high-shock conditions. It is recommended to incorporate 
		front-side retention such as illustrated in Figure 46. Note that a maximum, uniform, load of 1kgF 
		can be applied to the shutter face without causing failures in shutter actuation. When designing 
		the foam thickness and compression the tolerances have to be such that the maximum force of 1kgF 
		at the same time as enough force is exerted to keep the Lepton in the socket. 
~~~~

So I'm thinking we can mount it in a case. There are four mounting holes in the board. A window is also recommended. 

~~~~
    The Lepton camera is not a sealed assembly. Consequently, for most applications it is recommended to locate the assembly 
    behind a sealed protective window. Common materials for LWIR windows include silicon, germanium, and zinc selenide 
    (LWIR absorption in silicon is on the order of 15%/mm, which means NEDT is adversely affected using a silicon window. 
    Bulk absorption in germanium and zinc selenide is negligible, and performance is essentially unchanged provided both 
    surfaces of the window are anti-reflection (AR) coated.) Note that the window should be sized large enough to avoid 
    encroaching upon the optical keep-out zone (see Optical Considerations, page 69)
~~~~