# Introduction #

This is a checklist of all the things we should check before releasing a version of code as "Stable"

# Details #

## Installation ##
  * Via Bluetooth, Infrared, Cable or OTA - does the application install properly and without errors?
  * You will get the default security warnings, this is expected normal behaviour.

## First Run ##
  * Does the application start properly?
  * Loading... splash screen displayed, and then shows Accounts/Profiles page?
  * Are the menu and quit options in the correct location for your handset (left menu, right quit on Nokia)

  * Quit the application - does it exit gracefully?

Restart then go to:

  * Menu -> New - Displays new profile page with sensible default values?

## Google Talk ##
  * Add your google talk account using non-SSL with port 5222, does it connect ok?
  * Make a note of connection type: GPRS, 3/3.5G, Wifi etc
  * Send a message to a contact and get a reply to ensure two-way traffic is working

  * Exit the application and restart it, then edit the profile and change to SSL with port 5223.
  * Reconnect and test sending a message again.
  * If the profile has vanished, you have a problem with the record store and this is a reportable bug! It shouldn't happen though! ;-)

  * Leave connected for at least a few minutes, preferably 15-30 mins to ensure the keepalive is working ok.

  * Does your buddy list load as expected, including Show/hide offline?
  * Does the application hide (switch to the background) successfully using the hide option?

## Standard XMPP / Jabber ##

If you have your own server, or access to another public XMPP/Jabber server, connect to that account and test it works

  * What is the server running, e.g. Openfire, eJabberd etc
  * What version is the server running?
  * Does it connect with an unsecure connect 5222?
  * Does it work with SSL/TLS?
  * What type of SSL certs are installed? (Self-signed / CA signed)
  * Does the keepalive feature ensure the connection stays active?

Any other notes of observations should be recorded as appropriate