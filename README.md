# fridge-text


[![make.fun · u-deysumbrella-the-3am-fridge-text-4c3e721d](https://make.fun/badge/u-deysumbrella-the-3am-fridge-text-4c3e721d.svg)](https://make.fun/bounty/u-deysumbrella-the-3am-fridge-text-4c3e721d?utm_source=github&utm_medium=readme&utm_campaign=u-deysumbrella-the-3am-fridge-text-4c3e721d)

[![rank](https://make.fun/badge/u-deysumbrella-the-3am-fridge-text-4c3e721d/nmlyz/fridge-text/rank.svg)](https://make.fun/bounty/u-deysumbrella-the-3am-fridge-text-4c3e721d/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-deysumbrella-the-3am-fridge-text-4c3e721d)

[![reward](https://make.fun/badge/u-deysumbrella-the-3am-fridge-text-4c3e721d/nmlyz/fridge-text/reward.svg)](https://make.fun/bounty/u-deysumbrella-the-3am-fridge-text-4c3e721d?utm_source=github&utm_medium=readme&utm_campaign=u-deysumbrella-the-3am-fridge-text-4c3e721d)


A tiny program that writes the 3am text message of a smart fridge to a

text file. The message is a single line of 87 characters: the fridge

counts its owner's late-night visits and points out that all three

of tonight's visitors were the same person. The program checks the

line before writing it, so the file stays inside the 140-character

limit. It also checks the written bytes after writing: the file must

be exactly the line plus one trailing newline, so what the gate reads

is what was checked.


## The message

> It's 3am. You are the third person to open me tonight, and the other two were also you.

## Run it

```sh
python3 main.py
```

It writes the message to `/output/entry.txt` (`OUTPUT_DIR` overrides
the directory). Running it twice produces byte-identical output, so
the entry is fully reproducible from the source alone.
