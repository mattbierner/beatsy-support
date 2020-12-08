# Beatsy

Beatsy is an augmented reality music visualizer app for iOS. Distort real world surfaces using the beat of music. The app is [available for free on the app store][app].

This repo provides documentation on using Beatsy. If you run into any issues or have any feature requests, you can also [file an issue][issues] here.

## Using the app

### Placing the AR plane

To get started with Beatsy, first you need to select a real world surface for the visualizer to distort. You can place the visualizer on any flat horizontal or vertical surfaces. The app will walk you through the placement process.

> 🎵 **Note**: Drag horizontally to rotate the visualizer and pinch to scale it up and down. These controls also work after you have place the visualizer.

If you are having trouble placing the visualizer:

- Try moving the device about a little. On devices without a LiDAR sensor, this helps with surface detection.
- Make sure there is enough light for the cameras. Surface detection struggles in low light scenes.
- Use a surface that has some visual details. Surface detection struggles when pointed at solid color surfaces, such as white walls.

### Visualizing microphone

By default, Beatsy visualizes input from the microphone. This is shown by the red microphone button. Just talk or make sound to see the visualizer kick in.

> 🎵 **Note**: If the microphone is not working, make sure Beatsy has microphone permissions. In the Settings app, search for `Beatsy` and make sure `Microphone` is checked.

You can also use the microphone to visualize audio from other apps playing over the speakers. Beatsy pauses active audio when it launches, but you can resume the audio from control center.

### Visualizing music

To visualize music, tap the center icon with the musical note. This will bring up a music selector. If you instead see an alert title an `Internal Error`, then the Apple Music app is not currently installed on your device. Make sure to reinstall it before trying again.

Beatsy can only visualize songs that you have copied to your device. It does not support streaming music from cloud services such as Apple Music or Spotify. It also cannot visualize music with DRM protection. I know these limitations suck—I even [wrote a whole piece](https://blog.mattbierner.com/the-war-we-forgot/) about why they exist and why they suck—unfortunately I cannot work around them however.

> 🎵 **Note**: You can play streaming music from service such as Spotify over the speaker and use the microphone's input.

> 🎵 **Note**: Services such as [Bandcamp](https://bandcamp.com) offer DRM free music. After purchasing a song, download it and copy it to your device to load it up in Beatsy.

### Customizing the Visualizer

Tap on the wave icon to change the visualizer or edit the settings for the current visualizer. Beatsy currently offers two built-in visualizers:

- `Speaker` — Circular visualizer that distorts the surface using smooth waves. The visual effect is sort of like a giant speaker.

- `Wave` — Breaks music up into sections (e.g. bass, mid, treble) and visualizes how the intensity of the music changes over time. 

I plan on adding more visualizers in the future too!

### Sharing

Tap the circular camera button to capture a screenshot of the current visualization. This screenshot hides all UI elements so that you only see the visualizer.

Tap and hold the camera button to start recording a video. This starts a countdown, with recording starting after three seconds. Tap the camera button again to stop recording. While recording, you can interact with the app and adjust the visualizer. Videos also record the microphone input.

> 🎵 **Note**: Keep in mind that while you are free to share any content created with Beatsy, music may be subject to copyright. To be safe, make sure to get the copyright holder's permissions before publicly posting videos with music.

After taking a video or screenshot, you can download it to your photos or share it using the standard iOS share sheet.

## Feedback

Love Beatsy? Be sure to tell your friends about it and share any cool visualizations you create using the app. If you are feeling especially generous, please can also write an App Store review. This really helps other people find the app.

Run into a bug or want to request a few feature? Just [file an issue][issues]!

[app]: https://apps.apple.com/us/app/beatsy/id1543162330
[issues]: https://github.com/mattbierner/beatsy-support/issues
