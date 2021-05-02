# UXFFconfigurator
Source and support for the configuration app for the UXFFront module.
UXFFront is a replacement board for the ICOM IC-900/IC-901 UX radio modules "Front Unit" that features a
small form-factor 8051 MCU.  This replcement board allows the module to operate as a stand-alone radio.
The configuration application simplifies the setup and configuration of the module's MCU.

configux.exe: A simple console application for WIN10 that provides for management of the UXFFront module.
          Requires a valid COM port# to run.  The port# can be entered at the WIN10 command line or after
          the application has started.  If an invalid COM port is selected on startup, the extended help
          file is opened.
          
          V0.5 fixes the UX-129A/E support and includes the UX-129 RIT/VXO capabiulity.
          
    NOTE: The application is not "signed" so WIN10 may think that it is "dangerous" (yet to be determined).
          The user will have to take the leap-of-faith and "run anyway" since I don't yet know enough about
          WIN apps to get it signed and otherwise righteous.
          
"configux.ini" is an optional ini (text format) file for configuring parameters of the configux.exe application.
"configrun.bat" starts up configux.exe with COM port help if the .ini or default COM port is unavailable.

"ux59.txt" is an example config file for the ICOM UX-59, 6m module.

"list_com_ports.bat" is a utility to quickly list the available COM ports

