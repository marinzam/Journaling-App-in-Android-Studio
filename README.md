# Journaling-App-in-Android-Studio
Final project for android development course
CSC 214 Project 3 DayToDay

Author: Geraldine Marin-Zamora

*** Test on tablet 10.1 Emulator for best performance *** (Geocoder works on tablet?) I’m using 10.1 API 25:5554 according to emulator

This is a journaling app, powered by SQL. Before testing, you must allow permissions in the settings of the device. 

By signing up, you can create Journal Entries and view them in Master Detail by rotating the device. When creating entries, you can take a picture (no post-image capture rotation of image if device is landscape when taking picture) or upload from gallery. You can pick a date, which uses a DatePickerDialog, type an entry, as long as you please, enter what the weather was like, and look up the location via coordinates or address/city name. The address name uses a Geocoder Intent Service to get the coordinates to then display in a GoogleMaps View underneath. (If service is “not available”, try a few more times.M) When the entry is saved, you can select an existing entry and it will show all saved information, and rather than the GoogleMaps view, it loads a picture of the searched location using a Static GoogleMaps url.

In settings, you can edit your user information, change your password, and set the application theme to dark. In the RecyclerView, you can long click on an item to delete it, an Alert dialog comes up to confirm.

Schema saves most recent login, user info, and journal entries pertaining to each user. From the JournalEntriesActivity, you can create an entry via NewEntryActivity, edit an entry via EditEntryActivity, see an existing entry via ExistingEntryActivity. The rest of the classes are self explanatory (Login, Signup, EditPassword, etc).

I run Nougat on my tablet and all services worked. If it doesn’t on an emulator, I’d be glad to send a video of its functionality on the tablet.

“I affirm that I will not give or receive any unauthorized help on this exam, and that all work will be my own.” - Geraldine Marin-Zamora


The goal of Project 3 is to create an app of your own design that meets the requirements below.
0. Basic Features
Your App Must Include  all  of the following features.
● A design based on Model View Controller (MVC)
● Best Practices for communication between fragments and activities.
● A custom theme that includes custom colors and styles for at least the most common
widgets ( TextView , B  utton , E  ditText ).
● Separate interfaces for phone and tablet form factors; make good use of the space on
larger screens.
● A landscape orientation that makes sense. And no, “facebook and twitter do it” does not
excuse locking the orientation.
● At least 2 activities.
● A layout comprised of one or more fragments. There should not be any widgets outside
of a fragment other than the layouts containing the fragments.
● Up navigation.
● An options menu.
● A  RecyclerView  or a V  iewPager .
● Persistence: your app must function properly even if the “don’t keep activities” developer
option is enabled. The TAs will be instructed to enable this setting.
● At least one dialog.
● At least one toast.
● Logging, logging, logging.
● Robust error handling. Your app should not crash.
● A SQLite Database used for persistence across restarts.
1. Advanced Features
Your app must feature at least 5 of the following features
● The ability to use the camera to take and save photographs
● The ability to use the camera to record and save video
● Playing sounds with SoundPool
● Playing longer sounds or video with MediaPlayer
● Network connectivity
● Services
● One or more Google Play services (e.g. Maps)
