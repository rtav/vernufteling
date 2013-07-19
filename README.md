# What?

*Vernufteling* is my personal attempt to perfect my keyboard layout,
strictly to my own desires.

# Why?

In the *Kulturkreis* where I live, we type azerty. The azerty layout
is inferior, and the same goes for the qwerty layout. I have
extensively tried Colemak and Workman (and Workman Programmer), but
they too have their issues for my hands and habits. I prefer to
stretch and curl my fingers up and down rather than force my index
fingers into the two middle columns (as per Colemak).

I write a lot of
- English
- Dutch
- Python
- Clojure
- LaTeX
- Unix-style commands

I also write some
- Ancient Greek

This keyboard layout strives to be a compromise for those needs.

# How

Actually, there are many ways to change the keyboard layout, so I
figure I should create one more. The vkb (as in __V__irtual
__K__ey __b__oard) syntax for keyboard layouts is a work-in-progress,
and should remain very abstract. The idea is to have it be recompiled
to another syntax for concrete use.

## VKB

I define a vkb file for my own comfort. It should adhere to these rules:
- `Fields` should start with an ampersand character (&).
- Actual ampersand characters should be escaped with a backslash (\&).
- Everything on a line after a hash character (#) is considered a `comment`.
- Actual hash characters should be escaped with a backslash (\#).

The following semantics are valid for `fields`:
- Field 1 should contain the virtual keycode (as per Xkeyboard: TLDE, AE01, AE02, ...)
- All other fields should contain Unicode code points (glyphs and control characters).
- Field 2 holds the basic key input.
- Field 3 holds the shifted key input.
- Field 4 holds the AltGr key input.
- Field 5 holds the shifted AltGr key input.
- An optional field 6 holds the long-press key input.

# By what other name?

I chose the name *vernufteling* in homage to Simon Stevin's proposed
translation for the Dutch/Flemish word for an *engineer*. His proposal
never caught on (we still speak of *ingenieurs*), but his wit stroke
my cord, so to speak.

Also, the Google search space for the term is empty except for Stevin.

# Caveat lector

Licensed per the MIT License (see LICENSE.md). Expect volatility.
