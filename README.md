
# Genediad Veleg
Genedid Veleg coming from the Sindarin for Great Calendar is based on Etar!

![Etar Calendar](./assets/_pre_prod/publish/v1.0/animation.gif)

## Why?
Well, I wanted a calendar planner that was similar to the planner used by LDS missionaries.

## Special thanks

[Etar Calendar project](https://github.com/xsoh/Etar-Calendar)

The application is an enhanced version of AOSP Calendar. Without the help of
[Free Software for Android](https://github.com/Free-Software-for-Android/Standalone-Calendar) team, 
this app would be just a dream. So thanks to them!

## Features
- Month view.
- Week, day & agenda view.
- Uses Android calendar sync. Works with Google Calendar, Exchange, etc.
- Material designed.
- Agenda widget.

## Future Features
- Goals (Daily, Weekly, Monthly... maybe yearly)
- Todo lists
- Study section (Both spiritual and secular)
- Notes

### Build instructions
```
git submodule init
git submodule update

gradle build
```

### How this was done
- see ``build.gradle`` and the modifications to ``AndroidManifest.xml``
- ``fix_strings_and_import.py`` was created to fix a build problem and rename imports of R.java
- get time zone data from http://www.iana.org/time-zones write ``backward`` and ``zone.tab`` to assets and to assets of https://github.com/dschuermann/standalone-calendar-timezonepicker
- comment out code in https://github.com/dschuermann/standalone-calendar-frameworks-ex
