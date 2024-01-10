# Geektrack BETA

A versatile logging and tracking solution leveraging the [Telegram](https://telegram.org/) platform, which I've been building for myself and friends since 2022.

<img width="640" alt="Group 2 (3)" src="https://github.com/mxgrn/geektrackbot/assets/33935/146064e1-bc2c-4262-b5de-ddbb3c06a56a">

## Features

- Cumulative tracking (e.g. time spent reading/meditating, amount of water consumed, expenses, exercise reps, etc)
- Streaks (e.g. how many days in a row you logged something) and breaks (how many days you did _not_ log something specific)
- Automatic daily, weekly, monthly, and yearly reports. Reports are sent at midnight.
- Record reports: if you had a record month of meditating, Geektrack will notify you about it
- Charts and other visual UI to help you reflect, analyze, and grow
- Automatic timezone supports. Moving around the globe? Geetrack adapts.

## Getting started

- Create a Telegram group per tracked activity, e.g. "Jogging, min"
- Add https://t.me/geektrackbot to that group as you would any other user
- Start posting your log entries into that group, e.g. "50"

Press the "App" button at the bottom of your _chat with the bot itself_ (that is, [here](https://t.me/geektrackbot) - the button is available after you _start_ the bot) to open the app.

## Data entry format

Currently, Geektrack supports the following data entry formats

- Integers, e.g. "100"
- Decimals, e.g. "10.5"
- Time entry, stored as _minutes_
    - 10:30 is 10.5 minutes
    - 0:45 is 0.75 minutes
    - 1:10:00 is 70 minutes

The entry should start with a know format. The text that follows, is ignored, but stored internally (it may turn into notes later).
If an antry cannot be parsed, it'll be silently ignored.

### Editing an entry

- You may edit an entry by editing on of the previous messages. If the new value isn't parsable, the entry is _deleted_.
- To _delete_ an entry, do not simply _delete_ the message (Telegram bot does not detect that, at least for now). Edit the message and replace it with a "-" or any other unparsable log entry.

### Coming-soon features

- Data export. I know how important it is to know you have an access to all your data at any time.
- Support for trend tracking (e.g. weight, mood, energy levels, etc). The difference with cumulative tracking is that it doesn't make sense to sum up weight, mood, etc.
- Next to cumulative tracking, I'll add more forms of aggregate tracking (e.g. a *count* of certain log entries)
- More data formats
- Many more configuration options
- Many more (configurable) notifications - e.g. streak records, a reminder to keep the streak, etc.

### Distant-future plans

- API to invite all sorts of integrations and plugins

Besides, I have a very long list of other ideas that I would like to implement at some time, but I won't rush into discussing them. For 2 years Geektrack has been grown along my own needs, and I'm only starting, really.

Need a specific feature? [Let me know](https://t.me/geektracktalk).

## FAQ

### Is this open source?

Geektrack is not (yet) open source. If you feel like help me develop it (and maybe, as a result, use Geektrack for free, forever), [reach out](https://x.com/mxgrn) to me, and we may set you up as a contributor to the private repo.

### Why not a native app?

For the purposes of Geektrack, Telegram covers the 2 most important use cases: entering data, and getting notifications. Besides, it even provides a close-to-native experience in a webview.
Additionally, it has the following advantages:

- No need to install yet another app on your phone or computer (given you already use Telegram, the Porsche of messengers)
- No need for me to go through app store moderation
- Updates are frequent and instant, as it's "just" a web service
- Works on any platform, both from mobile phones and desktops

## Discussions

Feel free to join our discussion group on Telegram to provide feedback, request features, report issues, and share any other thoughts.

You may also open issues on this repository.

I'm especially interested to hear about various use cases that you might use Geektrack for.

## Pricing

During the Beta period Geektrack is free to use, no limits. Once out of beta, there will be some generous usage limits for those who choose to use it for free. Exact price isn't yet known, and it'll probably be a one-time payment.

---
(c) 2024 Max Gorin
