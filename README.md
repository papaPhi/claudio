# clAudio
Commandline bluetooth audio player for Linux


clAudio aims to become a simple, yet useful tool in developing, building, testing and using computers without running GUI as wireless audio players using Bluetooth technology.
Aimed primarily at Raspberry Pi and similar small form factor computers, clAudio should fill a gap between simple direct connection of Bluetooth input to audio output, and more complex GUI-based audio players, allowing use cases with non-standart, or indeed non-present, input and output solutions, such as its inspiration - use in automotive appliance with control input/output handled via CAN bus.

Technologically, clAudio runs on Linux OS, using D-Bus to communicate with BlueZ and Pulse Audio, handling the bluetooth device using A2DP to deliver audio and AVRCP to control playback and get information about current playback.
Depending on configuration, clAudio can then output this information to terminal, D-Bus interface and/or a specific other output like a hardware display, or CAN bus message. Meanwhile, input can be collected from keyboard, D-Bus and/or a specific other output like a GPIO-connected set of hardware buttons, or, again, a CAN bus message.
