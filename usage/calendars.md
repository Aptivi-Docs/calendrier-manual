---
description: We need calendars!
icon: calendar
metaLinks:
  alternates:
    - https://app.gitbook.com/s/BdESDsiuTO9fbDXLJ8HV/usage/color-sequences
---

# Calendars

Calendrier provides some of the calendar management APIs to make access to them easier than before. You can now get the calendar straight from the calendar type or its name using the `GetCalendar()` function from the `CalendarTools` class.

{% hint style="info" %}
Additionally, you can use the variant calendar, which uses your culture to define a calendar culture. This can be accessed by calling `GetCalendar()` with `CalendarTypes.Variant` as a type.
{% endhint %}

Additionally, the time and date renderers can be used with the base calendar class instance obtained from the above function. The following calendars can be used:

* `Chinese`: `zh-CN`
* `Gregorian`: `en-US`
* `Hijri`: `ar`
* `Japanese`: `ja-JP`
* `Persian`: `fa`
* `SaudiHijri`: `ar-SA`
* `Taiwanese`: `zh-TW`
* `ThaiBuddhist`: `th-TH`
* `Variant`: Your system culture

{% hint style="warning" %}
Some systems, especially when using Mono, return the Um Al-Qura calendar when using the Hijri calendar. Similarly, Persian calendars might be returned as Gregorian calendar in such systems. Mono, for some reason, considers the regular Hijri calendar in all Arabic cultures to be invalid.
{% endhint %}
