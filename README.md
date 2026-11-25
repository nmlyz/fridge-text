# fridge-text

[![make.fun · u-deysumbrella-the-3am-fridge-text-4c3e721d](https://make.fun/badge/u-deysumbrella-the-3am-fridge-text-4c3e721d.svg)](https://make.fun/bounty/u-deysumbrella-the-3am-fridge-text-4c3e721d?utm_source=github&utm_medium=readme&utm_campaign=u-deysumbrella-the-3am-fridge-text-4c3e721d)
[![rank](https://make.fun/badge/u-deysumbrella-the-3am-fridge-text-4c3e721d/nmlyz/fridge-text/rank.svg)](https://make.fun/bounty/u-deysumbrella-the-3am-fridge-text-4c3e721d/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-deysumbrella-the-3am-fridge-text-4c3e721d)
[![reward](https://make.fun/badge/u-deysumbrella-the-3am-fridge-text-4c3e721d/nmlyz/fridge-text/reward.svg)](https://make.fun/bounty/u-deysumbrella-the-3am-fridge-text-4c3e721d?utm_source=github&utm_medium=readme&utm_campaign=u-deysumbrella-the-3am-fridge-text-4c3e721d)

A tiny program that writes the 3am text message of a smart fridge to a
text file. The message is a single line of 134 characters: the fridge
has watched its owner eat cereal dry, straight from the box, standing
up at 3am, and finally says what it thinks about that. The program
checks the line before writing it, so the file stays inside the
140-character limit. It also checks the written bytes after writing:
the file must be exactly the line plus one trailing newline, so what
the gate reads is what was checked.

## The message

> I have watched you eat cereal dry, straight from the box, at 3am,
> standing up. I am a fridge. I have no mouth. And yet I am screaming.

## Run it

```sh
python3 main.py
```

It writes the message to `/output/entry.txt` (`OUTPUT_DIR` overrides
the directory). Running it twice produces byte-identical output.
