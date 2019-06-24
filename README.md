# Introduction
These are lists of the CC numbers of specific MIDI equipment, in a format
intended for TidalCycles.  These are meant to be easily copied from and pasted
into tidal code.

The filenames indicate the equipment the CCs control. The text was copied
directly from the relevant pages of the user manuals of each, then cleaned up. 

**None of this is standalone TidalCycles code**. You will get an error if you
try to run any of it alone. But it should be easy to integrate. 

# Format
```
ccv 0 # ccn {{ CC number }}, -- {{ description }}
```

# Usage
Open the file and copy the lines for the parameter(s) you want to control. Paste
into your TidalCycles code.

Due to the trailing commas, these are best used within an array, which is
typically the input of e.g. `cat` or `stack`. I prefer this over use within
their own pattern.

Typically you will want to edit the `ccv` parameter, but you might not need to
edit anything else.
