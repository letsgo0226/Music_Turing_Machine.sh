# Music_Turing_Machine.sh

`Music_Turing_Machine.sh` is a 2KB one-line music Turing transducer.

It reads three lines from stdin:

```text
Q = natural-language prompt
T = duration in seconds, blank uses a bounded prompt-derived length
K = seed/key label, blank defaults to 0
```

The machine treats music generation as a Turing-machine process:

```text
Q/T/K input tape -> finite TM trace -> musical AST -> PCM/WAV output tape -> CLCERT
```

The output files are:

```text
Music_Turing_Machine_<K>.wav
Music_Turing_Machine_<K>.clcert
```

The certificate records `M`, `TR`, `QV`, `G`, `R`, `AST`, `WAV`, `STATUS=HALT`, `ZP`, `BUG`, `PCC`, and `ZE`.

This project formalizes a bounded music generator as a Turing transducer. It does not claim to solve every possible aesthetic judgment.
