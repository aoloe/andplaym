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
- Get notified when a files has finished playing.
- Show the current state of the playing file.
- Pause the playing.
- Fastforward and backward the playing.
- Restart the playing of the current track.
- Skip to the next file in the queue.
- Set the volume (eventually)
- Settings to define the address of the server
- Create and manage playlists (eventually)

Create web services that can:

- Show the list of files and directories at a specific path (and it's subpaths).
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

- communication over json
- server side in python. several small webservices?
