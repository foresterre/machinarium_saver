Machinarium Saver
=================

##### Why?

My flash data files are removed after each execution of Flash Player.
Because Machinarium runs on flash and stores its data to a flash local shared object (.sol), the save file is also removed.
Instead of restarting, anytime I play Machinarium, I use these scripts.

There is an alternative solution, which might be easier in your case:
http://forum.amanita-design.net/index.php?topic=809.0
The link in this forum to the binary is broken, but you should be able to run the provided code it in the REBOL core interpreter as well. Or create an .exe using e.g. NSIS.

As a third alternative you could use a provided save files, as described here:
http://forum.amanita-design.net/index.php?topic=1274.0



##### Requirements
* Powershell & Windows

* Powershell script execution rights
If you want to set these, be sure you know the consequences.
Execute in powershell with Administrator rights:
<pre>Set-ExecutionPolicy RemoteSigned</pre>
(Click here for more information...)[https://technet.microsoft.com/en-us/library/ee176961.aspx]

* Change the designation folder settings in both scripts, if you don't want to use the default setting ($<user>/Desktop/MachinariumSave/saves)

##### How to ...
For my convenience I usually play in windowed mode. 

(After starting machinarium & saving to a slot in game)
(Before closing the game)

* Save: execute machinariumSaver.ps1

(Before starting the game)

* Restore: execute machinariumSetback.ps1

##### License (MIT)

Copyright (c) 2015 Foresterre

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.