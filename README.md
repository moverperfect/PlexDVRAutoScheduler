# PlexDVRAutoScheduler
Script that can generate scheduled tasks for plex recordings


# Findings

Local\Plex Media Server\Plug-in Support\Databases\com.plexapp.plugins.library.db contains a table called "media_grabs", this contains the subscriptions that we need to discover. Inside the column "extra_data" there is two data values "beginsAt" and "endsAt", these are EPOCH counters that can be used to determine the scheduled tasks for windows.
