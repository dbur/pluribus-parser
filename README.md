# Parser for Pluribus Poker AI Hands
[Data Source](https://science.sciencemag.org/content/early/2019/07/10/science.aay2400)

Takes this:

`STATE:11:ffffcc/cr230c/cr530c/cc:4hAc|Ah6s|4cKh|2s4s|2c9c|4dKc/5d6h2h/3h/Js:530|-530|0|0|0|0:Pluribus|MrBlue|MrBlonde|MrWhite|MrPink|MrBrown`

And turns it into this:

```
PREFLOP:

MrBlonde (4cKh) FOLDS
MrWhite (2s4s) FOLDS
MrPink (2c9c) FOLDS
MrBrown (4dKc) FOLDS
Pluribus (4hAc) CHECKS
MrBlue (Ah6s) CHECKS

FLOP: 5d6h2h

Pluribus (4hAc) CHECKS
MrBlue (Ah6s) RAISES 230
Pluribus (4hAc) CALLS

TURN: 3h

Pluribus (4hAc) CHECKS
MrBlue (Ah6s) RAISES 530
Pluribus (4hAc) CALLS

RIVER:Js

Pluribus (4hAc) CHECKS
MrBlue (Ah6s) CHECKS

RESULTS:
Pluribus 530
MrBlue -530
MrBlonde 0
MrWhite 0
MrPink 0
MrBrown 0
```

# TODO:
- Read paper
- Check if stack sizes change or if each game starts with 10k
- Clean up parser results
- Get HUD-like stats on each player


# References

```
Superhuman AI for multiplayer poker
BY NOAM BROWN, TUOMAS SANDHOLM

PUBLISHED ONLINE11 JUL 2019

DOI: 10.1126/science.aay2400
```
