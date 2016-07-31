# lnav-ruby-logger-format

Ruby Logger format for [http://lnav.org](lnav). View Ruby logs and easily find critical information.

This format matches the default Ruby stdlib Logger output. If you use a custom formatter with Logger, you'll need to edit the Regexp in the format file to account for your custom formatting.

Timestamps are set up so lnav can correctly navigate the logs in a time-like manner, and alert-level is set up so lnav can navigate from error to error (or warning to warning, etc).

In addition, the following captures can be used with lnav's SQL search:

* pid
* alert_level
* body

## Installation

Clone this repo into your lnav formats directory (usually ~/.lnav/formats). Lnav should find the new format the next time you run it.