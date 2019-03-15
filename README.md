# Disclaimer 

This is an awesome script made by https://github.com/williballenthin
Taken from this repo: https://github.com/williballenthin/idawilli/tree/master/scripts/yara_fn

I didn't made a fork because I just want this script with a few changes... But the awesome and dificult work has been made by him :)

The diference with this script and the original are:
### Now it drops the .yar file directly at the Desktop folder (I got tired of copy pasting it from the IDA Output window)
### I deleted the yara-python check, as I don't want it and makes me sad to see the alert every time


# yara_fn

IDAPython script that generates a YARA rule to match against the
basic blocks of the current function. It masks out relocation bytes
and ignores jump instructions (given that we're already trying to
match compiler-specific bytes, this is of arguable benefit).

If python-yara is installed, the IDAPython script also validates that
the generated rule matches at least one segment in the current file.

## installation

none

## usage

invoke the script via `File->Script file...`. review the text written to the output pane.


