# Randori Timer

A round timer for judo training: randori, uchikomi, nagekomi, or anything else you run in rounds. You can read the clock from across the mat, and the warnings are bells and beeps like in combat sports, not a spoken countdown.

## Put it on GitHub Pages

1. Create a new public repository on GitHub, for example `randori-timer`.
2. Upload `index.html` and `sw.js` to the root of the repository (**Add file → Upload files**, then commit).
3. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, then pick `main` and `/ (root)`, and save.
4. After a minute your timer is live at `https://<your-username>.github.io/randori-timer/`.

To use it like an app, open that link on your phone and add it to your home screen (Safari: Share → Add to Home Screen; Chrome: ⋮ → Add to Home screen). Once you've opened it one time, it works offline too.

## Defaults

| Setting | Default |
|---|---|
| Rounds | 5 |
| Round length | 4:00 |
| Rest | 1:00 |
| Get ready | 0:10 |
| Warning | Bell with 10 seconds left |
| Countdown beeps | Short beeps at 3, 2 and 1 |
| Round end | Buzzer |
| Round start | Double bell, when get-ready or rest ends |

There are no sounds from 9 to 4 seconds left. The clock keeps counting normally (00:10, 00:09 …), and the screen turns red for the last 10 seconds of each round.

You can change any of this under **Sounds and warnings**: when the warning sounds (or turn it off), how many countdown beeps there are (0–5), and which bell, buzzer or clapper plays for the warning, the round start and the round end. **Hear the last 10 seconds** plays the whole pattern so you can check it before training.

## During a session

- Tap the screen to show the controls. They hide again after a few seconds.
- **Pause/resume**, **skip** (ends the current round or rest now) and **back** (restarts the current part; tap twice to go to the previous part).
- **End** needs two taps, so you can't stop a session by accident.
- On a laptop: `Space` pauses, `←`/`→` go back and skip, `M` mutes, `F` goes full screen.
- The screen stays awake while the timer runs, on browsers that support it.

## Presets and sharing

Randori, Uchikomi and Nagekomi are built in. Change the settings and tap **Save as preset** to keep your own. Presets and settings are saved in that browser.

The page address updates as you change settings, for example `…/#n=Randori&r=5&w=240&b=60&p=10`. Send that link to someone and it opens with the same setup.

To change the built-in presets for everyone, edit the `BUILTIN` list near the top of the script in `index.html` (times are in seconds).

## Sound tips

- Plug the phone or laptop into a speaker for a big dojo. The sounds are made by the browser itself, so there are no audio files to load.
- On an iPhone, turn the media volume up. On iOS 17 or later the timer should play even with the silent switch on; on older versions, turn the silent switch off.
