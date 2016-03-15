# system.date.js

Date utility. Creates formatted date string.

# Methods

date_formatted([format String], [date Date], [language String]);

set_date_language(lang String);

set_date_format(format String)

# Date Format Variables

  __%d__ -  Day of the month, 2 digits with leading zeros   01 to 31

  __%D__ - A textual representation of a day, three letters    Mon through Sun

  __%j__ - Day of the month without leading zeros  1 to 31

  __%l__ (lowercase 'L') - A full textual representation of the day of the week    Sunday through Saturday

  __%N__ - numeric representation of the day of the week 1 (for Monday) through 7 (for Sunday)

  __%S__ - English ordinal suffix for the day of the month, 2 characters   st, nd, rd or th. Works well with j

  __%w__ - Numeric representation of the day of the week   0 (for Sunday) through 6 (for Saturday)

  __%F__  - A full textual representation of a month, such as January or March  January through December

  __%m__  - Numeric representation of a month, with leading zeros   01 through 12

  __%M__  - A short textual representation of a month, three letters    Jan through Dec

  __%n__  - Numeric representation of a month, without leading zeros    1 through 12

  __%Y__  - A full numeric representation of a year, 4 digits   Examples: 1999 or 2003

  __%y__  - A two digit representation of a year    Examples: 99 or 03

  __%a__  - Lowercase Ante meridiem and Post meridiem   am or pm

  __%A__  - Uppercase Ante meridiem and Post meridiem   AM or PM

  __%g__  - 12-hour format of an hour without leading zeros     1 through 12

  __%G__  - 24-hour format of an hour without leading zeros     0 through 23

  __%h__  - 12-hour format of an hour with leading zeros    01 through 12

  __%H__  - 24-hour format of an hour with leading zeros    00 through 23

  __%i__  - Minutes with leading zeros  00 to 59

  __%s__  - Seconds, with leading zeros     00 through 59

# Languages
  >  English
  __en__  
  
> Russian
  __ru__ 

  > Ukrainian
  __ua__ 
  
# Examples

```javascript
date_formatted(); // 14:42:55 14.03.2016

date_formatted('%H:%i:%s'); // 14:42:55

date_formatted('%H:%i:%s', new Date()); // 14:42:55

date_formatted('%H:%i:%s %F', new Date(), 'en'); // 14:42:55 March
```
