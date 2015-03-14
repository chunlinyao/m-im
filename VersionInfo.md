# Introduction #

Here's how our version numbers work..

  * v X.Y.Z (.a)

  * X = Major version - version 1 currently, version 2 would be a very significant change
  * Y = Minor version - something quite big changed, or we've introduced a significant new feature or changed quite a bit of code
  * Z = Revision (sub-version)
    * x.x.0 = First stable release of that version of m-im
    * x.x.1 = First patch release - bug fixes, tweaking of code, little optimisations, translations etc.

  * .a
    * beta / b = a Beta release, by all means test it, but it might crash or have bugs!
    * rc = release candidate - pretty stable, but we're not 100% confident in it

  * DEBUG = a debug build (LOGGING = true), this is designed for geeks or running in an emulator, by all means install it on your phone if you feel like it. A DEBUG version should be STABLE if the build number indicates it should be stable, but the debugging might do weird things and it might not be as fast as the production version.