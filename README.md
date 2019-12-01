# tongue

Tongue uses speech recognition to get the location of each individual word inside an audio or video file, then compiles these together in any order requested.
This uses google speech recognition for the bulk processing, and then pocketsphinx to check individual words.

### Usage

To view the help for tongue use any of the following commands:
```bash
tongue help
tongue --help
tongue -h
```

First have a folder containing mp3 or mp4 files, ideally only containg the voice you want to mimic.

Then run:
```bash
tongue add <filename>
```
on each of them to generate a .srt file for each, containing the location of each word said. Note that this will take a while to run, often around 10 minutes per hour of audio.

To view a list of the words found, use:
```bash
tongue list
```

To make your subject say a phrase, use any of the following:
```bash
tongue say "The phrase you want them to say"
tongue say The phrase you want them to say
```

To see if all the words for a phrase are available without doing the full speech generation, use any of:
```bash
tongue check "The phrase you want to check"
tongue check The phrase you want to check
```
