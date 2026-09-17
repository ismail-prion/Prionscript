# Prionscript

A complete programming language interpreter. Written in C++17. Built solo, on a phone, in Syria.

**Status: FOR SALE** — full source code, documentation, and ownership transfer.
Asking: $4,000 – $5,000 (negotiable)
Contact: ismail998213@gmail.com

Live showcase page (features, stats, live output demo): *[https://youtube.com/shorts/AmdriDFzKgE?si=9JE_urHSiQd6mL7S]*



## What is Prionscript?

Prionscript is a dynamic scripting language with a full lexer, parser, AST, and
tree-walking interpreter — all in a single ~4,050-line C++17 file, with zero
external dependencies beyond optional SDL2 and OpenSSL.

## Quick Stats

| | |
|---|---|
| Lines of C++17 | ~4,050 |
| SecurityRadars | 6 |
| Permission flags | 10 |
| Platforms | Linux, Windows, Android |
| External dependencies | 0 (SDL2 / OpenSSL optional) |

## Core Language

- Full lexer with line tracking + escape sequences
- Parser: complete AST, operator precedence
- Tree-walking interpreter
- 7 value types: null, int, float, string, bool, list, dict
- Dynamic typing
- Functions with recursion (capped at 2000 depth)
- Labeled while-loops (`loop:label!(cond)`)
- Dream blocks (background threads, isolated snapshots)
- Memoization via `.learn()`
- Living Memory: `x.history`
- Empathy heuristic: `user.frustrated`

## Security

- **6 SecurityRadars** — step radar (busy-loop kill switch), recursion-depth
  radar, container-growth radar, injection radar, privilege-probe radar,
  bounds radar
- **OS-level sandbox** — CPU time limit, address space limit, wall-clock
  limit, child-process limit, via Linux rlimits and Windows Job Objects
- **10-flag permission system** — every sensitive capability (filesystem,
  network, eval, threading, hardware, crypto, audio, process info) is off by
  default and must be explicitly enabled per run

## Built-in Libraries

Math (trig, statistics, matrices, linear regression) · Networking (raw sockets
+ JSON-RPC) · Blockchain (Ethereum, contracts, DEX) · Crypto (Kyber,
Dilithium, Argon2id, scrypt) · AI (Anthropic + Groq integration) · Neural
networks (from-scratch sigmoid MLP) · Regex · Hardware I/O (GPIO, serial,
battery, thermal) · Terminal (ANSI, instant key read)

## Sample (verified output)

This is real Prionscript source, and the output below is the actual result
captured from running it through the interpreter:

```
func:factorial!(n) {
    if (n <= 1) { return 1; }
    return n * factorial(n - 1);
}

console:main!() {
    output("factorial(6) = " + to_string(factorial(6)));

    nums = [5, 3, 8, 1, 9];
    output("unsorted: " + to_string(nums));
    output("sorted:   " + to_string(sort(nums)));

    d = { name: "Prion", version: 1 };
    output("dict.name = " + d.name);
}
```

Output:

```
factorial(6) = 720
unsorted: [5, 3, 8, 1, 9, ]
sorted:   [1, 3, 5, 8, 9, ]
dict.name = Prion
```

## Why It's For Sale

I'm a solo developer moving on to a new project. Prionscript is complete,
tested, and documented — a new owner can rename it, rebrand it, and ship it
as their own from day one.

## Full Source

The full `prionscript.cpp` source and complete language specification are
provided directly to serious buyers on request — not published in this
repository.

**Contact:** ismail998213@gmail.com

Built in 20 days using AI-assisted development.
