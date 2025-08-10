+++
author = "Ted Chen"
date = '2025-08-10'
draft = false
title = "Audio Blog Feature Test"
description = "Testing the new audio player feature for blog posts with a sample audio file."
tags = ['test', 'audio', 'feature']
audio = ["/audio/sample.aac"]
+++

---

This is a test blog post to demonstrate the new audio player feature. You should see an audio player displayed near the date and author information above.

<!--more-->

## Audio Player Features

The audio player includes:

- Play/pause button with hover effects
- Progress bar that matches the theme colors
- Current time display
- Volume control and mute button
- Keyboard accessibility
- Responsive design that works on all devices

## How to Use

To add an audio player to any blog post, simply add the `audio` parameter to your front matter:

```toml
+++
title = "My Blog Post"
audio = "/audio/my-audio-file.aac"
+++
```

The audio player supports common audio formats:
- AAC (.aac)
- MP3 (.mp3)
- WAV (.wav)

## Styling

The audio player automatically adapts to the theme's color scheme, including dark mode support. It uses the same design language as the rest of the blog for a cohesive experience.

The player is positioned right after the post metadata (author, read time, date) and before the main content, making it easily discoverable for readers who want to listen to the audio version of your post.
