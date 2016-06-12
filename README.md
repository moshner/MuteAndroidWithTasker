#  Mute Your Phone By Turning It Upside Down

![Icon for project][icon-phone-mute]

**Problem**: I forget to mute my phone in meetings sometimes.

**Solution**: Mute my phone automatically by the simple act of turning it upside down on the table.

Overview
--------
This solution uses **tasker** for Android to sense the orientation of your phone and turn off the volume. Optionally, you can then create an exit task to return the phone to a more normal volume.

* Orientation Face Down
* On Entrance - Mute phone, all volumes to 0, end call, screen off
* On Exit - Unmute phone, all voluems to 5

Requirements
------------

* Android
* Tasker

Detailed Steps
--------------

**Setup**

1. Download and install [tasker][taskerurl]

**Profile**

2. Create new profile: State, Sensor, Orientation

3. Set the Orientation state to 'is Face Down'

4. Save / Back Button

**Entrance Task**

5. Create a new task and call it *Silent Mode*.

5. Add Action: Audio, Silent Mode. Set to "Vibrate".

5. Add Action: Audio, Media Volume. Set to "0".

5. Add Action: Audio, Ringer Volume. Set to "0".

5. Add Action: Audio, System Volume. Set to "0".

5. Add Action: Audio, Alarm Volume. Set to "0".

5. Add Action: Audio, Alarm Volume. Set to "0".

5. Add Action: Audio, Alarm Volume. Set to "0".

5. Add Action: Phone, End Call.

5. Add Action: Display, System Lock.

5. Back Button out

**Exit Task**

1. Long press on the entrance tasks on Profile screen.

1. Select "Add Exit Task"

1. Create a new taks and call it *Normal Mode*

1. Add Action: Audio, Silent Mode. Set to "Off".

1. Add Action: Audio, Media Volume. Set to "5".

1. Add Action: Audio, Ringer Volume. Set to "5".

1. Add Action: Audio, System Volume. Set to "5".

1. Add Action: Audio, Alarm Volume. Set to "5".

1. Add Action: Audio, Alarm Volume. Set to "5".

1. Add Action: Audio, Alarm Volume. Set to "5".

1. Back Button out

[taskerurl]: http://tasker.dinglisch.net/
[icon-phone-mute]: /icon-phone-mute--black.png "Mute your phone"
