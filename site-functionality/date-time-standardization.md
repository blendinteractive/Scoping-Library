---
description: >-
  Date formatting should be selected before a project begins and should be
  something to figure out during the planning process.
---

# Date / Time Standardization

Our standard is to show the "actual time" of the current editor. In other words, if an editor's time zone is 11PM Central, the post will show a date/time of 11PM Central.

However, this is a discussion to have during technical scoping. There may be a use case for using the localized Episerver CMS time.

### When Does This Issue Show Up?

This is mostly noticed when we get closer to midnight, since the day will be different, in the U.S. anyway, it would show up more at larger time zone differences, but it’s rare.&#x20;

### Options

To re-itereate the two options:

* **Localized** - This is the Episerver default.
  * Localized example: I create an article with the date 1 am April 2 when in Central time, it will appear as 11 pm April 1 in California, because there’s a 2 hour difference.
* **“Actual Time”** - We can change the code so the date is the actual time that the item was created. Then when that date is seen anywhere in the world it will still be that time.
  * So for example if I create something at 11pm, April 1 Central it will display 11pm, April 1 in California.

