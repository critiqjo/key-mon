# Wrong or Missing Keys #

If you download the source there is a file called xlib.py which can be run to see the keystrokes, or mouse click events.


```
$ python src/keymon/xlib.py 
Press ESCape to quit
Xlib.protocol.request.QueryExtension
Xlib.protocol.request.QueryExtension
type:EV_KEY scancode:30 code:KEY_A value:1
atype:EV_KEY scancode:30 code:KEY_A value:0
type:EV_KEY scancode:48 code:KEY_B value:1
btype:EV_KEY scancode:48 code:KEY_B value:0
type:EV_KEY scancode:1 code:KEY_ESCAPE value:1
^[
```

If you send the me information for the keys that aren't working and what they should be I can try and fix it.

Create a new issue http://code.google.com/p/key-mon/issues/entry so I can track the bug a little easier.