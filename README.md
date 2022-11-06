# Transfer learn from English to Romanian!
## How to run
1. Open the notebook in Google Colab (other platforms are untested, so proceed at your own discretion in that case)
2. Set the runtime in Google Colab to GPU (`Runtime > Change runtime type`)
3. Import `clips.zip`, `metadata.txt`, and `alphabet.txt` to the Colab session
4. Run all cells

Script will take a while to run (around 4 hours) so be patient :)

## Goal
The repository I decided to use is Coqui's STT one.

The task is to do transfer learning for STT using English as a source language and Romanian as the target one.

I expect to get a WER between 20-40% given that the languages are not that similar to each other.

## Data format
The audio files, metadata and alphabet files are provided in the repo as well. If you want to use different audio files,
I suggest using the name `clips.zip` and have a folder `clips` inside of it with the audio files. Otherwise, change the paths in the script according to your file structure inside the zip archive.

If you want to change any file, the format needs to stay the same to avoid issues with the converter script
that transforms the files into ones understood by Coqui STT.

The data represents a subset of my recordings in Romanian that I submitted to Common Voice.

All data, including the notebook, can be found in `transfer_learn_RO` folder.

## Results obtained
