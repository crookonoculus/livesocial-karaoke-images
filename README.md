# LiveSocialVR Karaoke Images

Independent image feed for the four Karaoke Frame Pics displays.

## Update the pictures without an APK upload

1. Upload JPG or PNG pictures to this repository.
2. Edit `karaoke-images.json`: add each picture's raw GitHub URL to `images`, or remove URLs you no longer want displayed.
3. Increase `version` by one and commit the changes. Also increase it when replacing an existing picture with the same filename.

The running app checks the feed every two minutes. GitHub caching can add a delay. The next picture cycle adopts a successfully downloaded update. Keep at least four different images to fill all four displays without repeats. Smaller feeds leave some frames blank rather than duplicate pictures.

Pictures rotate in randomized rounds. Every frame sees every image during a complete cycle. Frames fade fully out before the next set fades in, so images cannot overlap across frames during a change.

The original seven pictures are bundled with the scene as an offline fallback. Download errors preserve the last complete working set. This repository is public and separate from the events, gallery, and landing-poster feeds.
