# *Microsoft Defender Emulation Detection*

## Authorship information
* Name or nickname (required): @luc4m
* Twitter: https://twitter.com/@luc4m
* Website: 
* Linkedin: 
* Email: 
  
## Technique Information
* Technique title (required): Anti-Emulation check for Windows Defender 
* Technique category (required): Antivirus Evasion
* Technique description (required): The Windows Binary emulator scanning engine inside Windows Defender's `mpengine.dll` retrieves several hard coded values, for instance the sample executable image is hardcoded as `C:\myapp.exe`, the computer name as `HAL9TH`, and the current username as `JohnDoe`. Malware families such as xLoader and PureLog uses `GetComputerNameA` and `GetUserNameA` API to check if it is running under the Windows Defender emulator engine, where the mentioned values are respectively `HAL9TH` and `JohnDoe`. 

## Additional resources

* https://i.blackhat.com/us-18/Thu-August-9/us-18-Bulazel-Windows-Offender-Reverse-Engineering-Windows-Defenders-Antivirus-Emulator.pdf
* https://av.tib.eu/media/39670
* https://twitter.com/eckes/status/1349438295298760704 

## Code snippets
* Please add your code in separate files.

## Detection rules
* Please add your rules in separate files.
