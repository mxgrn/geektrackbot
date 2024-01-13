<img alt="Geektrack screenshots" src="https://github.com/mxgrn/geektrackbot/assets/33935/146064e1-bc2c-4262-b5de-ddbb3c06a56a">
<br>

A versatile [logging and tracking solution](https://t.me/geektrackbot) I've been building for myself and friends since 2022. Now in public beta.

It's built on top of the [Telegram](https://telegram.org/) platform. Using chats as trackers turned out to be a very [powerful and simple idea](https://github.com/mxgrn/geektrackbot?tab=readme-ov-file#why-not-a-native-app).

_This repo is [NOT](https://github.com/mxgrn/geektrackbot?tab=readme-ov-file#is-this-open-source) source code for the service, but rather a hub for docs, FAQs, discussions, issues, and feature requests._

## Features

- Cumulative tracking (e.g. time spent reading/meditating, amount of water consumed, expenses, exercise reps, etc).
- Streaks (e.g. how many days in a row you logged something) and breaks (how many days you did _not_ log something specific).
- Daily, weekly, monthly, and yearly reports. Reports are sent at midnight.
- Record reports: if you had a record month of meditating, Geektrack will notify you about it.
- Charts and other visual UI to help you reflect, analyze, and grow.
- Timezone support. Moving around the globe? Geetrack adapts.
- Support for dark themes.

### Upcoming features

- Data export. I know how important it is to have access to all your data at any time.
- Support for trend tracking (e.g. weight, mood, energy levels, etc). The difference with cumulative tracking is that it doesn't make sense to sum up weight, mood, etc.
- Next to cumulative tracking, I'll add more forms of aggregate tracking.
    - An example could be a *count* of certain log entries, e.g. when you want to know _how many times_ you had a lucid dream in the past year, and not a sum of "lucidity" that you could be actually logging.
- More [data entry formats](https://github.com/mxgrn/geektrackbot?tab=readme-ov-file#data-entry-format).
- More configuration options (currently accessible in the [miniapp](https://github.com/mxgrn/geektrackbot?tab=readme-ov-file#miniapp)).
- More (configurable) notifications - e.g. streak records, a reminder to keep a streak, etc.

### Future work

- API to invite all sorts of integrations and plugins.
- Goals. You could define, say, a monthly goal of 1000 push-ups, then track how close you stay to the plan - weekly or daily.
- Support for the [Elastic Habbits](https://www.amazon.com/Elastic-Habits-Create-Smarter-Adapt-ebook/dp/B08188WBGC) system.

Besides, I have a very long list of other ideas that I would like to implement at some time, but I won't rush into discussing them. For 2 years Geektrack has been growing along my own needs, and I'm only starting, really.

Need a specific feature? [Let me know](https://t.me/geektracktalk).

## Getting started

1. Create a Telegram group with @geektrackbot as another user, name it, e.g. "Jogging, min"
2. Start posting your log entries into that group, e.g. "50"

Create one group per tracker.

![Creating new group](https://github.com/mxgrn/geektrackbot/assets/33935/73aab7e7-7796-46fa-b435-be917a96ae82)

_Creating a new group with the bot_

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

- You may edit an entry by editing on of the previous messages. If the new value isn't parsable, the entry gets deleted.
- To delete an entry, do not simply _delete_ the message in the chat (Telegram bot does not detect that, at least for now), but rather edit the message by replacing the content with a "-" or any other unparsable entry.

## Miniapp

Telegram allows us to implement "miniapps" just are basically authorized webviews. Geektrack takes a full advantage of that. See the "Miniapp" button down in the private chat with the bot (you need to start the bot first), or use the /help command anywhere.

## FAQ

### Is this open source?

Geektrack is not (yet) open source. If you feel like helping me develop it (and maybe get to use Geektrack for free, forever), [reach out](https://x.com/mxgrn), and I may set you up as a contributor in the private repo.

### Why not a native app?

For the purposes of Geektrack, Telegram covers the 2 most important use cases: entering data, and receiving notifications. The idea of entering log data in a chat, as well as getting reminders, feedback, reports, etc from the bot in the same chat, proved to be very simple and intuitive. And when this is not enough, Telegram's support for [miniapps](https://core.telegram.org/bots/webapps) provides freedom to build near-native experience where needed.

Additionally, going with Telegram has the following advantages:

- No need to install yet another app on your phone or computer (given you already use [Telegram](https://telegram.org), arguable the best messenger out there).
- No need for me to go through app store moderation.
- Updates are frequent and instant, as Geektrack is "just" a web service.
- Works on any platform, both from mobile phones and desktops.

## Tips and tricks

- Organize your Telegram tracking groups into folders for easier access and/or use the search. I have - and am actively using - dozens of trackers, with no issues finding my way around.
- Instead of using folders, you may want to name such groups with a prefix, e.g. 'GT jogging', which may simplify the esearch.

## Discussions

Feel free to join our [discussion group](https://t.me/geektracktalk) on Telegram to provide feedback, request features, report issues, and share any other thoughts.

You may also open [issues](https://github.com/mxgrn/geektrackbot/issues) on this repository.

I'm especially interested to hear about various use cases that you might (want to) use Geektrack for.

## Pricing

During the beta period, Geektrack is free to use, no limits. Once out of beta, there will be some generous usage limits for those who choose to keep using it for free. Your data from the beta period will be kept.

Exact price isn't yet known, but it might be a one-time payment. Pre-sale at a discuount is an option, so, stay tuned.

## Easter eggs

Hint: how about competing with friends?

---

(c) 2024 [Max Gorin](https://mxgrn.com)
