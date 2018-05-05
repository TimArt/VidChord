![logo](https://timart.me/img/vidchord-logo.svg)
# VidChord
A MaxForLive MIDI device that triggers videos to play based on MIDI chords.

## How to Install
1. Download the .zip file from GitHub.
2. Unzip the folder.
3. Place the folder in a location where you want Ableton to see it. Do NOT remove items from the folder. VidChord will only work if both Max files are in the folder.
4. Drag and drop the folder into the "Places" tab in the Ableton browser so Ableton will see it.
5. Open the folder in Ableton and drag n drop the VidChord plugin on a MIDI track.

## How to Use
1. Choose a folder of video files you want to trigger.
2. Make sure VidChord is "Started" by clicking the "Start/Stop" toggle button.
3. To test the videos, click the "Trigger Random" button to trigger a random video.
4. To trigger videos on a chord change, set the "MIDI Note Threshold" to the desired number of MIDI Note On messages held down at the same time that you want to trigger a new video. Then play a chord with that many notes in it and another video should randomly be chosen.
5. Set the "Video Buffer" to be the number of videos you want to be stored in memory at once. This allows you to flip through videos quickly without any video lag. If you are running low on memory or have a particularly memory intensive Ableton project, you may want to decrease this number. If you are changing through many videos really fast, you may want to increase this number to eliminate any video lag that happens.

## FAQ
**Q:** How random is it?

**A:** VidChord will randomly choose each video in the folder once. Then, after having played every video once in a random order, the process starts over with a new random order of choosing videos.

**Q:** Will there be more features in the future?

**A:** Yes, I eventually plan to add some video manipulation features such as live color changing, glitching, and video position scrolling.

**Q:** Why do some videos just freeze on the first frame and not play? Or why do my videos drop frames occasionally?

**A:** This is because the video buffer has run out and is trying to load new videos to be ready to trigger them. Essentially, you are triggering videos too quick for the software to load your videos and play them back. To fix this, make the "Video Buffer" a larger number. On my 2013 MacbookPro, I was able to keep the "Video Buffer" at 6 trigger videos at a moderate speed with no issues.

## Known Issues
- After making the video full screen, if you attempt to remove VidChord from a MIDI track, it will crash Ableton Live.
- After choosing the folder of videos to use, if you immediately attempt to trigger a random video, it will freeze on the first frame of the video because it is trying to load videos into the video buffer. If you give it a few seconds, this is no problem. Also if it freezes on the first video, you can just trigger a new one with no problem.
