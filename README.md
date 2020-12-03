# Beatsy (Beta)

Beatsy is an augmented reality music visualizer app for iOS. Distort real world surfaces using the beat of music.

The app is currently in beta testing.

## Providing feedback

Right now, the app is in beta testing with Test Flight. If you are interested in becoming part of the beta, just follow this link on an iPhone: https://testflight.apple.com/join/64mlg2hm

While testing, you can either file bugs and suggestion through the TestFlight app or on this repository. Make sure to include steps to reproduce any bugs.

## Using the app

### Placing the AR plane

To get started, first you need to select which real world surface you want the visualizer to distort. You can place the visualizer on any flat horizontal or vertical surfaces. The app will walk you through the placement process.

> 🎵 **Note**: Drag horizontally to rotate the plane and pinch to scale it up and down. These controls also work after you have place the plane.

If you are having trouble placing the visualizer:

- Try moving the phone about a little. On phones without a LiDAR sensor, this helps with surface detection.
- Make sure there is enough light for the cameras. Surface detection struggles in low light scenes.
- Use a surface that has some visual details. Surface detection struggles when pointed at solid color surfaces, such as white walls.

### Selecting music

Beatsy can visualize sound from the microphone or music stored on your iPhone.

By default, Beatsy uses the microphone. This is shown by the red microphone button. Just talk or make sound to see the visualizer kick in.

> 🎵 **Note**: If the microphone is not working, make sure Beatsy has microphone permissions. In the Settings app, search for `Beatsy` and make sure `Microphone` is checked.

To visualize music, tap the center icon with the musical note. This should bring up a music selector. If you instead see an alert about an `Internal Error`, then Apple Music app is not currently installed on your phone. Make sure to reinstall it before trying again.

Beatsy can only visualize songs that you have copied to the device. It does not support streaming music from cloud services such as Apple Music. It also cannot visualize music with DRM protection. I know these limitations suck. I even [wrote a whole piece](https://blog.mattbierner.com/the-war-we-forgot/) about why they exist and why they suck. Unfortunately, I cannot work around them.

> 🎵 **Note**: You can play streaming music from Spotify over the speaker and use the microphone's input.

> 🎵 **Note**: Services such as [Bandcamp](https://bandcamp.com) offer DRM free music. Just copy it to your phone to 

### ...