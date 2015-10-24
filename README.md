# fftag
all-purpose media file tagger written in bash that lets ffmpeg do the dirty work

## USAGE

fftag [-p] -i \<file\> [\<field1=value1\> ... \<fieldN=valueN\>]

### OPTIONS

`-p`  Prompt before overwriting file

## DESCRIPTION

When an input file is given with no options, the tags in the file are displayed and the program exits. This is useful for finding out the actual names of the tags already in the file, since those are what fftag uses as keys in its dictionary. They are not case-sensitive, but there is a distinction between e.g. "albumartist", "album artist", and "album\_artist", so be aware of that if you dislike redundant tags! 

### TODO
- return values of specified tag field(s), with different verbosity levels (i.e. either show tag name along with value or just value)
