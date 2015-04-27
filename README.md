# anki-silence-sound
Snips large sections of silence from front and end of mp3 files.

I am currently learning Portuguese and finding Anki cards to be helpful. I frequently record audio, synchronize my anki deck to my phone and then practice. I have noticed that waiting for the sound to start in a deck is quite an irritation. This little program uses the pydub library to simply remove silence from the start and end of mp3 files and can be run on unzipped Anki apkg files (which have no filename extension to identify them) or the collection.media folder on the Desktop version of Anki (which does have a filename extension).

It's written partly as a learning opportunity for Python and git.

I've test playing the files by first:
(a) identifying audio files (file *)
(b) playing with sox (sox -t mp3 [filename])
(c) comparing before and after.

I can export and import .apkg files and unzip and rezip them (just using e.g. zip Fluenz_Portuguese\ 1__Session\ 6.apkg *) without obviously causing problems for Anki.

I can also take my home Anki folder and run this script on it periodically:

./silence_sounds.py '/home/mulhollandd/Documents/Anki/User 1/collection.media/'

After I do a 'Check Database' and 'Check Media' a resynchronize of Anki and other devices ensures they are up-to-date.

Multiple runs of this should not cause any problems audio files.




