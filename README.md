# taskbarPin
pure ideas to construct the XML:
https://vcl.ncsu.edu/get-help/documentation/how-to-create-windows-images/adding-items-to-the-taskbar-in-windows-10/
https://docs.microsoft.com/en-us/windows/configuration/configure-windows-10-taskbar

then this is to upload it and apply it

![image](https://user-images.githubusercontent.com/44326428/130174175-2316cdea-2ae2-4726-86bd-8b0c0a1d3fc8.png)







Scripted version:
create the xml

Import-StartLayout -LayoutPath C:\TEMP\xml.xml -MountPath c:\


working on how to Add links to it
https://itectec.com/superuser/windows-how-to-pin-lnk-files-to-taskbar-in-powershell/


maybe helpful
```
import-startlayout 
export-startlayout 
```



TEMPLATE
```
<?xml version="1.0" encoding="UTF-8"?>

-<LayoutModificationTemplate Version="1" xmlns:taskbar="http://schemas.microsoft.com/Start/2014/TaskbarLayout" xmlns:start="http://schemas.microsoft.com/Start/2014/StartLayout" xmlns:defaultlayout="http://schemas.microsoft.com/Start/2014/FullDefaultLayout" xmlns="http://schemas.microsoft.com/Start/2014/LayoutModification">


-<CustomTaskbarLayoutCollection>


-<defaultlayout:TaskbarLayout>


-<taskbar:TaskbarPinList>

<taskbar:DesktopApp DesktopApplicationLinkPath="%ALLUSERSPROFILE%\Microsoft\Windows\Start Menu\Programs\Accessories\Paint.lnk"/>

<taskbar:UWA AppUserModelID="Microsoft.Reader_8wekyb3d8bbwe!Microsoft.Reader"/>

<taskbar:DesktopApp DesktopApplicationLinkPath="%appdata%\Microsoft\Windows\Start Menu\Programs\System Tools\Command Prompt.lnk"/>

<taskbar:DesktopApp DesktopApplicationLinkPath="%appdata%\Microsoft\Windows\Start Menu\Programs\System Tools\Calc.lnk"/>

<taskbar:DesktopApp DesktopApplicationLinkPath="%appdata%\Microsoft\Windows\Start Menu\Programs\System Tools\notepad.lnk"/>

<taskbar:DesktopApp DesktopApplicationLinkPath="%ALLUSERSPROFILE%\Microsoft\Windows\Start Menu\Programs\WinSCP.lnk"/>

<taskbar:DesktopApp DesktopApplicationLinkPath="%ALLUSERSPROFILE%\Microsoft\Windows\Start Menu\Programs\onedrive.lnk"/>

<taskbar:DesktopApp DesktopApplicationLinkPath="%C:\Temp\services.lnk"/>

<taskbar:DesktopApp DesktopApplicationLinkPath="%C:\Temp\lyrSucks.lnk"/>

</taskbar:TaskbarPinList>

</defaultlayout:TaskbarLayout>

</CustomTaskbarLayoutCollection>

</LayoutModificationTemplate>
```




