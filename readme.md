Hide Shortcut Arrow Overlay:
	open regedit
	go to "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer"
	create "Shell Icons"
	create string-value within Shell Icons named "29"
	double-click "29" and enter "%windir%\System32\shell32.dll,-50"
	restart explorer

Hide Shortcut UAC Overlay:
	open regedit
	go to "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer"
	create "Shell Icons"
	create string-value within Shell Icons named "77"
	double-click "77" and enter "%windir%\System32\shell32.dll,-50"
	restart explorer

- - - - - - - - - - - -

3     normal folder icon
8     fixed drive folder icon
11    removable drive folder icon
15    network drive icon in the explorer address bar
29    shortcut overlay icon
34    explorer navigation pane root icon labelled 'Desktop'
51    network folder icon
77    UAC (administrator) overlay icon
107   os drive folder icon
179   compressed file/folder overlay icon