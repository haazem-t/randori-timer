# Randori Timer

A round timer for judo training: randori, uchikomi, nagekomi, or anything else you run in rounds. You can read the clock from across the mat, and the warnings sound like a real fight: a wooden clapper at 10 seconds, then the bell.

## The main page

1. Pick a timer: **Randori**, **Uchikomi**, **Nagekomi**, or one you saved.
2. Set the **round time**, **rest time** and number of **rounds**.
3. Tap a **round color** and a **rest color**. The rainbow square lets you pick any color.
4. Choose the **round sound**: boxing bell, boxing bell ×3, gong, hand bell, buzzer and more.
5. Press **Start**.

Everything else is under **More settings**.

## What you hear

With the Randori defaults (5 × 4:00 rounds, 1:00 rest):

| When | Sound |
|---|---|
| Round starts | Boxing bell |
| 10 seconds left | Wooden clapper (clack-clack-clack) |
| 3, 2, 1 | Short beeps |
| Round ends | Boxing bell |
| 3 seconds before the next round | "Ready!" |

There are no sounds from 9 to 4 seconds left. The clock keeps counting normally, and the screen turns red for the last 10 seconds.

## More settings

- **Timer name** and **Get ready** time (the countdown before round 1).
- **Warnings:** when the warning sounds, which sound it is (wood clapper, door knock, bells…), how many countdown beeps there are, a different sound for the **end of round** (for example the gong), and whether the warnings also play during rest.
- **Voice:** the call before each round, and when it's said.
- **Colors** for get-ready and the final seconds.
- **Volume**, and **Hear the last 10 seconds** to check the whole pattern.

The **gong** is modelled on the match-end gong at the Olympic judo events (Tokyo 2020): a deep, soft gong that swells in and hangs in the air for about six seconds.

To keep a setup, change it and tap **Save this timer**.

## Record your own "Ready!"

A recorded voice sounds like a real coach; the phone's built-in voice doesn't.

1. Open **More settings → Voice** and tap **Record**.
2. Shout "Ready!" the way you would on the mat. It stops by itself after 3 seconds, or tap **Stop**.
3. The timer trims the silence, makes it loud, and plays it back. From now on it plays your call at 3 seconds before every round.

The recording is saved in that browser only. To use it on every device (the dojo iPad, your phone, the laptop):

1. Tap **Save as file** to download `ready.wav`.
2. Upload `ready.wav` to your GitHub repo next to `index.html`.

Every device that opens the site then uses it automatically. You can also upload your own `ready.mp3` or `ready.m4a`, for example a voice memo from your phone.

If there's no recording, the timer uses the device's built-in voice.

## Keeping the screen awake

While a session runs, the timer asks the device to keep the screen on. It also plays an invisible, silent video in the background, which keeps laptops and phones awake the same way a YouTube video does.

## Put it on GitHub Pages

1. Create a public repository, for example `randori-timer`.
2. Upload `index.html` and `sw.js` to the root (**Add file → Upload files**, then commit).
3. **Settings → Pages**: choose **Deploy from a branch**, then `main` and `/ (root)`, and save.
4. After a minute or two it's live at `https://<your-username>.github.io/randori-timer/`.

To update it later, upload the new `index.html` and let GitHub replace the old file. Your saved timers and colors stay.

Open the link on your phone and add it to your home screen to use it like an app. After the first visit it also works offline.

## During a session

- Tap the screen to show the controls: **pause**, **skip** (ends the current round or rest), and **back** (restarts it; tap twice to go to the previous part).
- **End** needs two taps, so it can't be stopped by accident.
- On a laptop: `Space` pauses, `←`/`→` go back and skip, `M` mutes, `F` goes full screen.

## Sound tips

- For a big dojo, plug the phone or laptop into a speaker.
- On an iPhone, turn the media volume up. On iOS 17 or later the timer should play even with the silent switch on; on older versions, turn the silent switch off.
- The page address includes the timer settings, so you can send someone a link that opens with the same setup.
