---
title: Reminder
parent: Plugins
nav_order: 5
---

# Reminder (`rm` for remind me...)

The RemindMe Plugin enables users to set reminders effortlessly by typing a date and/or time in natural language followed by a task. This intuitive yet minimalistic plugin
simplifies task management, ensuring you never miss anything important.

<img src="{{ "/assets/images/Plugin_RemindMe.png" | prepend: site.baseurl | prepend: site.url}}"/>

## Setting Reminders
To set a reminder using this plugin, start by specifying the date and time for the reminder using keywords such as "in," "on," and "at." Follow this with the task you want to be reminded of. You can also choose to separate the time and task with the word "to" for clarity. If you don't specify a time, the reminder will notify you at the next startup of the app. When reminders appear, you can choose to snooze them until the next startup or for a specific number of minutes as defined in the settings.

## Supported Time Specifications
- keyword `in`
    - `in 10 mins and 30 seconds`
    - `in an hour`
    - `in 4d 30m 20s`
- keyword `at`
    - `at 20`
    - `at 20:30`
    - `at 8:30 pm`
- time
    - `20:00`
    - `8pm`
    - `8:30pm`
    - does not detect just `20`, use `at 20` instead
- keyword `next`
    - `next month` (first day of next month)
    - `next week` (next monday)
- weekdays
    - `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`,
    - sets date to the next occurrence of that weekday in the future
- tomorrow
    - `tomo`
    - `tomorrow`
- special times (only when time is not provided in another way)
    - `morning`: 8:00
    - `lunch`: 12:00
    - `noon`: 12:00
    - `afternoon`: 14:00
    - `evening`: 17:00
    - `dinner`: 18:00
    - `night`: 20:00
- dates
    - `01.01.1970`
    - `15.4.`
    - `15.4`
    - `15.4.25`
    - `15.4.2025`
    - `15-4-25`
    - `15/4/25`
    - currently not detected: `1 September 22`, `31 Dec 2023`, `2024/12/29`
- task is anything after the keyword `to`, anything left of the time specification (query from start until first occurrence of `to`) after parsing will be prepended to the task

## Windows
Reminders include a GIF to catch your attention. You can customize this by providing your own GIF as `~/.smartclip/plugins/rm/reminder.gif` (.smartclip is usually in your home folder).

## Linux
Reminders won't get automatically snoozed when ignoring the notification, instead they will be removed after they pop up. To snooze the reminders, manually do so via the notification actions.