# It's A Trap!

###### Updates

_3.3_
* The trap creation wizard has been reorganized into groups of related properties. Some properties have been renamed.
* There is a new Set Trigger property that allows you to set the trap's trigger either to the trap's token itself, or a set of closed polygonal paths on the GM layer.

_3.2_
* Fixed 'noticed undefined' bug in passive perception.
* Traps' type property is now a text input instead of a predefined list.

This is a script that allows GMs to quickly and very easily set up traps,
secret doors, and other hidden things on the GM layer, and detect when tokens
on the objects layer move over them. This trap detection even works for tokens
moving by waypoints.

Combined with modules called Trap Themes, this script also allows system-specific
automation of trap effects and passive perception used to spot them.

### Creating traps:

Place the token for your trap on the ```GM layer```. Give it the ```cobweb```
<img src="http://game-icons.net/icons/lorc/originals/png/cobweb.png" width="32"> status marker.
Then, select the trap token and activate its 'ItsATrap_trapCreationWizard' token macro.
This will present a menu for setting up the trap's configurations.

### Setting trap triggers:

As of version 3.3, traps can be set to be triggered either by their own token or
by a set of paths on the GM layer. By default, the trap's token is used as
its trigger. The trap's ```Trap Shape``` property determines the token shape
(circle or rectangle) used for the collision.

You can change this by opening the trap's creation wizard in the chat,
selecting a set of polygonal or freehand paths from the GM layer, and then setting
the ```Set Trigger property``` for the trap to ```Paths```.

Note: Elliptical token shapes are not currently supported (unless they are circles).

### Activating traps:

If a token moves across a trap or its trigger paths at ANY point during its
movement, the trap will be activated!

A trap can also be manually activated by clicking the 'Activate Trap' button
in the trap's configuration menu.

### TrapThemes:

TrapThemes are used to provide support for formatting messages for traps and
automating system-specific trap activation and passive search mechanics.

If you are using the One-Click API Library, you can specify which theme to use
in the ```theme``` user option.

By default the ```default``` theme will be used. This is a very basic,
system-agnostic TrapTheme which provides support for the basic TrapEffect properties
and has no passive search mechanics.

Additional system-specific themes will be made available as their own API scripts.
If you would like to implement a TrapTheme for your system, take a look at
the ```default``` or ```5E-OGL``` TrapThemes as an example to get you started.

## Help

If you experience any issues while using this script or the trap themes,
need help using it, or if you have a neat suggestion for a new feature, please reply to this thread:
https://app.roll20.net/forum/post/3280344/script-its-a-trap-v2-dot-3
or shoot me a PM:
https://app.roll20.net/users/46544/stephen-l

## Show Support

If you would like to show your appreciation and support for the work I do in writing,
updating, and maintaining my API scripts, consider buying one of my art packs from the Roll20 marketplace (https://marketplace.roll20.net/browse/search/?keywords=&sortby=newest&type=all&genre=all&author=Stephen%20Lindberg)
or, simply leave a thank you note in the script's thread on the Roll20 forums.
Either is greatly appreciated! Happy gaming!
