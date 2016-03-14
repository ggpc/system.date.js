# system.date.js
Date utility. Creates formatted date string.

# Methods:
date_formatted([format String], [date Date], [language String]);
set_date_language(lang String);
set_date_format(format String)

# Date Format Variables
  %d   Day of the month, 2 digits with leading zeros   01 to 31
  %D   A textual representation of a day, three letters    Mon through Sun
  %j   Day of the month without leading zeros  1 to 31
  %l (lowercase 'L')   A full textual representation of the day of the week    Sunday through Saturday
  %N   numeric representation of the day of the week 1 (for Monday) through 7 (for Sunday)
  %S   English ordinal suffix for the day of the month, 2 characters   st, nd, rd or th. Works well with j
  %w   Numeric representation of the day of the week   0 (for Sunday) through 6 (for Saturday)
  %F   A full textual representation of a month, such as January or March  January through December
  %m   Numeric representation of a month, with leading zeros   01 through 12
  %M   A short textual representation of a month, three letters    Jan through Dec
  %n   Numeric representation of a month, without leading zeros    1 through 12
  %Y   A full numeric representation of a year, 4 digits   Examples: 1999 or 2003
  %y   A two digit representation of a year    Examples: 99 or 03
  %a   Lowercase Ante meridiem and Post meridiem   am or pm
  %A   Uppercase Ante meridiem and Post meridiem   AM or PM
  %g   12-hour format of an hour without leading zeros     1 through 12
  %G   24-hour format of an hour without leading zeros     0 through 23
  %h   12-hour format of an hour with leading zeros    01 through 12
  %H   24-hour format of an hour with leading zeros    00 through 23
  %i   Minutes with leading zeros  00 to 59
  %s   Seconds, with leading zeros     00 through 59

# Languages
  en // English
  ru // Russian
  ua // Ukrainian
  
# Examples
date_format(); // 14:42:55 14.03.2016
date_format('%H:%i:%s'); // 14:42:55
date_format('%H:%i:%s', new Date()); // 14:42:55
date_format('%H:%i:%s %F', new Date(), 'en'); // 14:42:55 March

