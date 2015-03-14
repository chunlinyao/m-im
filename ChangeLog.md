# Introduction #

This gives a high-level overview of the changes in each release

# Details #
## v1.5.0 ##
  * rewrite xmpp protocol based on kxml.

## v1.3.2 ##

  * Chunlin has backported the Chinese translations for 1.3.1. We also took the decision to make English the default language to ease deployment around the world. No significant code changes in this patch release, application data is backwards compatible to 1.3.x.

## v1.3.1 ##

  * Improved handling of network disconnections
  * Internal code tidy up and optimisations

## v1.2.0 ##
**Application Data NOT backwards compatible with v1.1.0**

Either uninstall v1.1.0 then install v1.2.0 or answer "No" if your phone prompts you to keep the existing application data

  * New Keepalive Option
    * Added XMPP Pinger class which sends an IQ PING packet (XMPP standard) every 5 minutes to the server, to keep the connection alive.

  * Some UI changes

  * Added Mute / Unmute menu options to quickly turn off sound notifications

  * Added detection of S40 / S60 Nokia handsets to optimise menu options on both platforms

  * Added "Global Preferences" which eases setting up new profiles with similar details

  * A few bug fixes and low-level code optimisations

## v1.1.0 ##
**Application Data NOT backwards compatible with v1.0.0**

Either uninstall v1.0.0 then install v1.1.0 or answer "No" if your phone prompts you to keep the existing application data

### New Functionality ###

  * Customisable "Resource" property for XMPP connection

  * Added "Display Name" to connection profile

  * Added vibrate function for supported handsets (most)

  * Minimise Support - allows running in the background

  * Added user-friendly titles to all screens
    * Chat with <Remote User Display Name> for ChatUI
    * Profile Name for ContactListUI, rather than JID

  * Restricted port number dialog entry to numbers only

### Known Issues ###

Need to add a method "supportsBackgroundRunning()" which returns
true if the phone supports minimise/background running of J2ME
applications, and false otherwise. This can then be used to
determine whether minimise or another function is assigned
to the right screen key on the UI

## v1.0.0 ##
(Initial Release uploaded to googlecode by chunlinyao)

### Known Issues ###

  * A few missing titles, and some UI Strings are hardcoded

  * On S60, right joypad does not increase volume or vibrate time on the slider control, but left click DOES decrease it!

  * When contacts go offline, their status icon changes to red (busy), rather than the grey cross (offline). This means it's hard to distinguish if someone has gone to DND or offline

  * "Error message" dialogue doesn't always dissappear properly