# Beatsy

Beatsy is an augmented reality music visualizer app for iPhone and iPad. Distort real world surfaces using the beat of music. The app is [available for free on the App Store][app].

This documentation covers the basics of using Beatsy. If you run into any issues or have any feature requests, you can also [file an issue][issues] here.

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

Tap on the wave icon to change the visualizer or edit the settings for the current visualizer. Beatsy currently offers four built-in visualizers:

- `Speaker` — Circular visualizer that distorts the surface using smooth waves. The visual effect is sort of like a giant speaker.

- `Wave` — Breaks music up into sections (e.g. bass, mid, treble) and visualizes how the intensity of the music changes over time. 

- `Ferro` - A visualizer inspired by magnetic fluid. Offers a number a customization options.

- `Spectrum` - Simple spectrum visualizer with 3 display modes.

I plan on adding more visualizers in the future too!

### Immersive visualizers

For users that have a device with a LiDAR sensor, you can also try Beatsy's immersive visualizers. Unlike the standard visualizers, these can distort the world around you in three dimensions instead of having to be placed on on a flat surface.

By default, immersive visualizers will distort the world around your current position. If you open up the visualizer settings and switch to center the visualizer at `Placement position`, the visualizer will instead be centered at .wherever you place it in the world.

> 🎵 **Note**: Immersive visualizers work by building up a 3D model of the world around you. This model may be incomplete. To improve the quality of the distortion effects, pan your phone over any areas of the scene you'd like to distort. You can also try viewing the same part of the scene from different angles to improve the 3D world model.


### Sharing

Tap the camera button on the right side to capture a screenshot of the current visualization. This screenshot hides all UI elements so that you only see the visualizer.

Tap the video button to start recording a video. This will show a prompt asking if you'd also like to record your microphone input in addition to any playing music. Tap the video button again to stop recording.

> 🎵 **Note**: Keep in mind that while you are free to share any content created with Beatsy, music may be subject to copyright. To be safe, make sure to get the copyright holder's permissions before publicly posting videos with music.

After taking a video or screenshot, you can download it to your photos or share it using the standard iOS share sheet. You can also trim videos right in the app.

## Advanced options

### Foreground occlusion

(Note that foreground occlusion requires a device with a LiDAR sensor, such as the iPhone 12 Pro)

Foreground occlusion uses depth data from the LiDAR sensor to avoid distorting objects that appear in front of the visualizer effects. This foreground object could be a person, your hand, or a wall. The result makes it look like the effect is better integrated into the world instead of merely being an effect on your screen.

To enable foreground occlusion, tap the lightbulb icon and toggle "Foreground Occlusion". Keep in mind that the effect is not perfect. If you don't need it, I suggest turning the feature off.

For best results with foreground occlusion:

- Make sure the visualizer plane is exactly placed on the real world surface. You may notice significant issues if the plane is placed a few cm above or below the real surface. 

- Only enable foreground occlusion if the surface is flat. If the surface is angled or pitted, foreground occlusion may cause weird artifacts.

- Keep in mind that objects only a few cm from the surface will be considered part of the surface. Foreground occlusion works best when there is at least a 25cm difference in depth between the foreground object and the surface (although the margin it uses internally is closer to 15cm). 

- Foreground objects can only be around 4 meter from the phone. This is a limitation of the LiDAR sensor.


## Feedback

Love Beatsy? Be sure to tell your friends about it and share any cool visualizations you create using the app. If you are feeling especially generous, please also write an App Store review. This really helps other people find the app.

Run into a bug or want to request a new feature? Just [file an issue][issues]!

[app]: https://apps.apple.com/us/app/beatsy/id1543162330
[issues]: https://github.com/mattbierner/beatsy-support/issues
