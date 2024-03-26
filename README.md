#Ovos-Skil-My-MPD (formaly known as Mympdplaylist-skill)

**Important: The old Mycroft settingsmeta.yaml is replaced by settings.json. There is an example with two servers and two stations. At least one server must be defined. The rest is optionally. Attantion: settings.json needs strict JSON syntax.**

This Mycroft.ai skill tries to make the handling of saved playlists for the player MPD comfortable. In addition, this skill occasionally dialogs with the user or announces information. (There is a very good MPD skill from forslund. If you don't use playlists, but only have a music collection of music files, you should use his skill.) If you can answer three or more questions with yes, you should try this skill:
Are different playlists used in MPD?
Is there more than one MPD player in the network?
Is there more than one Mycroft system in the house / apartment?
Do you want to be able to control all MPD players with all Mycroft systems?
Example sentences:

[alternative phrases are marked thus (term 2 | term 3)] "Turn on the radio" or "Turn on the radio in the kitchen (bedroom | workshop | …)" provided that the MPD software is already running but not currently playing a file or stream.
"Turn the radio a little louder/lower" or "Set the volume to 50"
"Play station (title | position) one (two | three | ..)" - if the player is in the same room
"Play station (title | position) one (two | three | ..) on the radio in (the ) kitchen (bedroom | workshop)"
"Play the first (next | previous | last) track (station | ...)"
"What am I listening to right now?"
"What playlists are there?" After that a dialog is shown to ask for list and start position
"Open the playlist radio stations (or another existing playlist) and play station three" - direct specification of playlist and start position
"Which songs (titles | songs | stations) are in the current playlist (list)"
"What playlists are there?"
"Search (Find | Exists) [search term] in the current playlist." - Search the current playlist
"Search (Find | Exists) [search term] in any playlist." - Search all playlists
"Search (Find | Exists) [search term] in the music database (music collection)." - then dialog for narrowing down search results.
All commands can be executed on a remote device with the addition "on the radio (in the | in the) [room name]".

Under not fully reproducible conditions, conflicts with the mycroft-playback-control.mycroftai skill may occur. Please report on this under Issues

To avoid possible conflicts with the skill mycroft-volume.mycroftai, the announcement to change the volume must be expressed in a differentiated way. the best results are (for an english speaking german) with this words "Turn up (down) the volume of mpd (in the kitchen)". At least a blacklisting of mycroft-volume.mycroftai helps but is not necessary.
Please read at least the configuration section in the wiki.
More information about configuration, functionality and commands in the wiki.

##Requirements

python-mpd2 (pip install python-mpd2)

##Credits

JoergZ2

##Category

Music & Audio

##Tags

ovos, Mpd, playlist, mycroft, skills

