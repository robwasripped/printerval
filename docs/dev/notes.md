# Notes

By default the configuration should be set up to work in a logarithmic scale
making more display types for sooner dates. The given system of seconds, hours,
years, etc may solve this dispersion issue.

The tool needs to work in both directions, where by phrases such as "3 minutes
ago" should be used for past events, whereas "in 3 minutes" would be the
equivalent future message. This can work even for "just now" vs "now".

## Configuration options

A vagueness can be specified that gives a range in which to prepend an adverb.
Labels will be marked as to whether they can have an adverb or not. A basic
description such as "5 minutes ago" can have an adverb, whereas "less then 1
minute ago" cannot as it's an absolute and true description. The flag could be
described as "true" labels as the information - regardless of accuracy - is
absolutely true.
* about
* around
* approximately

Options to use named periods. An option to toggle all named periods will be
easier to build. Toggling specific periods will be more difficult as the tool is
internationalised as different periods will be named across languages.
* fortnight
* decade

Options to add target date groups, where the system will check if it could fit
into one of the possibilities. The current date must also meet a given range. If
March were 2 days you would not want to see "last March".:
* last weekend
* Last October


# Relative Unit Groups

| Units     | Example                           |
| --------- | --------------------------------- |
| 0.5 units | Half a *u* ago                    |
| <1 unit   | less than *q* *u* ago             |
| 1 unit    | About *q* *u* ago                 |
|           | Around *q* *u* ago                |
|           | About a *u* ago                   |
|           | *q* *u* ago                       |
| 3-5 units | A few *u* ago                     |
| n unit    | About *q* *u* ago                 |
|           | Around *q* *u* ago                |
|           | *q* *u* ago                       |