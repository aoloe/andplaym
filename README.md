#andplaym

Android App to get a Linux media server to play music.

## Features

Create an Android App that can:

- Query a list of folders on a distant Linux server.
- Show the list of folders (and subfolders).
- Show the list of files contained in each folder.
- Search the names of the folders and files (eventually in a recursive way).
- Add individual files or directories to a queue of files to be played.
- Show the current queue of files on the server.
- Remove individual files from the queue.
- Shuffle the queue (eventually).
- Reorder the queue (eventually).
- Add item to the top of the queue.
- Show the current state of the playing file.
- Get notified when a files has finished playing.
- Pause the playing.
- Fastforward and backward the playing.
- Restart the playing of the current track.
- Skip to the next file in the queue.
- Set the volume (eventually)
- Settings to define the address of the server
- Create and manage playlists (eventually)

Create web services that can:

- Show the list of files and directories at a specific path (and its subpaths).
- Add items to a queue of files to be played.
- Remove an item from the queue.
- Clear the queue.
- Show the queue.
- Pull items from the queue of files and play them.
- Play a file.
- Give the status of the current playing track.
- Pause a file.
- Skip to the next file.
- Fastforward and backward the playing.
- Volume control.


## Mockups

### Show the list of directory and files

    +---------------------------------------------------+
    | Browse                                            |
    |---------------------------------------------------|
    |                                                  ^|
    |  ▷ cox_-_ed_cox/                                 #|
    |  ▷ clogs/                                        #|
    |                                                  #|
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  v|
    |---------------------------------------------------|
    |  ◀ ‖ ▷ ▶  On the Edge                 1:23 ▁▂▃▄▅▆ |
    +---------------------------------------------------+

- clicking on a directory, changes the view to its content.
- context menu on the directory gives the following options:
  - add content to the queue,
  - add content to the beginning of the queue,
  - browse.
- clicking on a file adds it to the queue
- content menu on the file gives the following options:
  - add to the queue,
  - add to the beginning of the queue.

    +---------------------------------------------------+
    | Queue                                             |
    |---------------------------------------------------|
    |                                                  ^|
    |  Clogs         6. Adages of Cleansin             #|
    |  Ed Cox        1. The Triumphant March of Piaf   #|
    |                                                  #|
    |                                                  #|
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  v|
    |---------------------------------------------------|
    |  ◀ ‖ ▷ ▶  On the Edge                 1:23 ▁▂▃▄▅▆ |
    +---------------------------------------------------+

    +---------------------------------------------------+
    | Preferences                                       |
    |---------------------------------------------------|
    |                                                  ^|
    |  Server:       [______________________________]  #|
    |  Port:         [______________________________]  #|
    |                                                  #|
    |                                                  #|
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  ||
    |                                                  v|
    +---------------------------------------------------+

- The tabs are activated by buttons in the lower Android command area.

## History

http://developer.android.com/training/basics/firstapp/index.html

## Ideas

- onStart should check that wlan is enabled

      LocationManager locationManager = (LocationManager) getSystemService(Context.LOCATION_SERVICE);
      boolean gpsEnabled = locationManager.isProviderEnabled(LocationManager.GPS_PROVIDER);
      if (!gpsEnabled) {
          // Create a dialog here that requests the user to enable GPS, and use an intent
          // with the android.provider.Settings.ACTION_LOCATION_SOURCE_SETTINGS action
          // to take the user to the Settings screen to enable GPS when they click "OK"
      }

## Ideas

- communication over json
- server side in python. several small webservices?

## Deugging

- As of February 24 2013, on debian 64 bit you need lib32z1 installed (the 32 bit installer). Eclipse will complain if you need it!
- If the ABT Manager does not work, run it from Eclipse
