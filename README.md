# automator

Are you afflicted by a runaway aslmanager and a massive file collection in /var/log/asl/*? If so, this might do just what you need.

## Summary

I got tired of running `sudo launchctl stop com.apple.syslogd; sudo launchctl stop com.apple.aslmanager; sudo rm -rf /var/log/asl*; sudo launchctl start com.apple.syslog`. It was getting ridiculous having to get to a terminal every 30 minutes to make the fan spin stop. So I automated it with Automator.

## How It Works

Just clone this repo out. You might need to save it to Applications. I didn't have to, mine lives in `~/gitrepos/automator` and Mac OSX just knows how to find it. I just type `Cmd+space Fix` and it autofills the rest. A password prompt pops up and moments later the aslmanager CPU spin stops and the /var/log/asl directory is blissfully empty.
