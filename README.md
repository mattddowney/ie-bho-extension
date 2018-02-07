# ie-bho-extension
Browser Helper Object (BHO) prototype for a IE Extension/Plugin.

## Prerequisites
This project was written and built using Visual Studio Express 2012 on a Windows 7 VM.

To make this work in IE (Tested in IE8):

1. Build the project in 'release' mode
2. Copy the dll (IEExtension.dll) to a folder within the 'Program Files' folder. This is so IE can access it.
3. Open the Visual Studio Command Prompt, browse to the folder where you dropped the IEExtension.dll file (see step 2)
	- To install run: regasm /codebase IEExtension.dll
	- To Unistall run: regasm /unregister IEExtension.dll
	- regasm located in C:\Windows\Microsoft.NET\Framework\v4.0.30319
4. Open IE. Once your homepage is loaded, a POP-UP alert will show the message: "HOLA!!!"
