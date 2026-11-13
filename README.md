# SnoozeFox

Content and updates for **SnoozeFox**, a sleep app with bedtime stories, music, sleep sounds and an alarm.

The Android app reads `content/manifest.json` from this repo, downloads only the files whose SHA-256 changed,
and offers an in-app update when `app/SnoozeFox.apk` has a newer version code.

```
content/manifest.json        story list, file hashes and sizes, latest app version
content/stories/<id>_voice.ogg     narration
content/stories/<id>_fx.ogg        real-world sound effects, mixed to the story
content/stories/<id>_music.ogg     the story's own score, ducked under the voice
content/stories/<id>_ambience.ogg  seamless loop that can keep playing after the story
content/stories/<id>.json          timing and mix settings
app/SnoozeFox.apk                  latest app build
```

## Credits

- Narration: [Kokoro](https://huggingface.co/hexgrad/Kokoro-82M) text-to-speech (Apache 2.0).
- Scores: composed for each story and performed with the **VS Chamber Orchestra: Community Edition** samples
  by Versilian Studios, Sam Gossner, Simon Dalzell and Ivy Audio (CC0).
- Sound effects: field recordings from [Radio Aporee](https://aporee.org) on the Internet Archive, marked public domain.
- "The Fox Who Told the Truth" written by Joseph Miller (J Fox).
