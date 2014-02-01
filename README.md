# TimeTrack

A little doodad to track my time.

I tend to forget what I've been working on
and what I've been doing, so I've taken
to keeping a time-stamped list that looked like this:

```
1:24 PM   Fixed DOC-518
          Added myself to scrumbot
          made some changes to it
          Played with Calendar apps
2:31 PM   Made a little tool to switch my creds
4:02 PM   Closed DOC-515 (notes were behind)
```

I figured I could write a simple command tool
to make it easier and that I could hook it into an
Alfred workflow. The hotkey for this is Shift-Command-space,
but you can change it of course.

This workflow writes whatever you enter in Alfred to
a file `$HOME/.track/YYYY-MM-DD`. Each line has the
time of day (HH:MM) unless the time would be the same
as the previous line:

```
00:31   Now we begin
00:32   Worked on the time tracker
        Gave it an Icon
00:49   README for track
00:58   Push TimeTrack to github
```



You can download it [here](https://raw.github.com/pborenstein/track/master/TimeTrack.alfredworkflow)
or use this command:

```
curl -O https://raw.github.com/pborenstein/track/master/TimeTrack.alfredworkflow
```

The clock icon is from https://github.com/driftyco/ionicons.
