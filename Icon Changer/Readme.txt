******************************************************************************
Written by Yash Kumar (aka OrdinaryGuy)
Copyright (c) Yash Kumar, 2002

Purpose: Module allows you to extract and replace any Win32 EXE's icon

Bugs: You may not always be able to sucessfully replace the icon of every
Win32 EXE. If someone is able to figure out why, please do email me with
the updated code.

License: You are free to use this code in anyway you like including commercial purposes
No credit is required. If you want to help me then the best you can do is vote :)

You can contact me at: OrdinaryGuy@gamebox.net or yash.kumar@devawards.com
Visit my upcoming site - www.DevAwards.com :)

*****************************************************************************
SwapIcon.bas

Public Procedures:
	1 -  ExtractIcons (ByVal strSource As String, ByVal strDest As String)
	      Arguments ---

       		 strSource = The full pathname (including extension) of the executable file which
			     contains the icons to be extracted and saved to .ico files.

		 strDest   = The full pathname (including extension) of the new .ico file which
			     will be created.

              Return value ---
	         Returns the error code.

	
	2 -  InsertIcons (ByVal strSource As String, ByVal strDest As String)
              Arguments ---
		 strSource = The full pathname (including extension) of the .ico file which
			     contains the icons to be inserted into the destination executable.

		 strDest   = The full pathname (including extension) of the executable file
			     into which the icons will be inserted.
	      Return value ---
		 Returns the error code.

	      IMPORTANT ---
		 Icons in the destination executable will be overwritten.  If you wish to save
		 these icons, use ExtractIcons() to save them to .ico files before calling
		 InsertIcons()

*******************************************************************************