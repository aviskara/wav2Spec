# wav2Spec
Create multiple spectrograms snippets from random snippets of wav files.


## Generating a spectrogram
To begin with the program 3 files must be created in the directory that the program is located in:
* music
* images
* splitMusic 

Place the desired wav files in the music folder and run though the entirety of the program and the desired spectrogram will appear

## Changing the interval of snippets
The function that controls the length and location of snippets is the `split_wav.multiple_split` function. There are a couple of parameters to play with.
1. sec_per_split
   * Contols the the length of each split in seconds
2. start_sec
   * Controls the minimum start location of the snippet. Intended to be used to skip intros.
3. end_bef
   * Controls the maximum start location of the snippet. Intended to be used to skip outros.
4. rand_amount
   * Controls the total number of snipets that will be made. The number of snipets = number of spectrograms.

## Other changes to be made
1. The function `plot_spectrogram` has a parameter y_axis that controls the display of the frequency type that can be read [here](https://librosa.org/doc/main/generated/librosa.display.specshow.html).
2. The file names and locations can be changed by changing their respective strings with the path of the desired folder.

## Current Issues/ Things to Imporve
1. Space inefficient as the function requires WAV files to be able to work and stores WAV snippets in folder
2. Make the whole program be able to be called with a single function with supporting arguments/ parameters

## Thanks to the following people 
https://stackoverflow.com/a/62872679 - code to split the wav file
https://www.youtube.com/channel/UCZPFjMe1uRSirmSpznqvJfQ - idea for this whole thing
