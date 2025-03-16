# SCRIBE (Spoken Corpus Recordings In British English), a TIMIT for British English
Data processing and analysis of SCRIBE (Spoken Corpus Recordings In British English)

https://www.phon.ucl.ac.uk/resource/scribe/

TL:DR: You can think of this dataset as a TIMIT for British english. It contains phonetic annotations with time alignments.

The SCRIBE dataset is a small corpus of read speech and spontaneous speech specializing in British English. It consists of 200 phonetically rich sentences and 460 phonetically compact sentences. The phonetically rich sentences are phonetically balanced. The phonetically compact sentences are based on a British version of the MIT compact sentences (as in TIMIT). There are 45 files in the dataset of 30-50 seconds containing 5-10 sentences.

For our experiments in the paper [Text-Independent Phone-to-Audio Alignment Leveraging SSL (TIPAA-SSL) Pre-Trained Model Latent Representation and Knowledge Transfer](https://www.mdpi.com/2624-599X/6/3/42), the audio files and the phoneme annotations needed some processing before we could start using the dataset. The phonemes are in SAMPA form and we needed to convert them to the English Arpabet. Even after the conversion from SAMPA to Arpabet, there were symbols that we could not retrieve so we filtered them out.

The notebook implements this processing. 
I put a copy of the audio files in this repository.

A talk about this work at [ISCA SIG-SLATE](https://sites.google.com/view/sigslate) webinars:

[![Alt text](https://img.youtube.com/vi/7_pQ0aQwg-w/0.jpg)](https://www.youtube.com/watch?v=7_pQ0aQwg-w&ab_channel=ISCASIGSLaTE)



# Citations
```
Tits, N., Bhatnagar, P., & Dutoit, T. (2024). Text-Independent Phone-to-Audio Alignment Leveraging SSL (TIPAA-SSL) Pre-Trained Model Latent Representation and Knowledge Transfer. Acoustics, 6(3), 772-781. https://doi.org/10.3390/acoustics6030042
```

Bibtex:
```
@Article{acoustics6030042,
AUTHOR = {Tits, Noé and Bhatnagar, Prernna and Dutoit, Thierry},
TITLE = {Text-Independent Phone-to-Audio Alignment Leveraging SSL (TIPAA-SSL) Pre-Trained Model Latent Representation and Knowledge Transfer},
JOURNAL = {Acoustics},
VOLUME = {6},
YEAR = {2024},
NUMBER = {3},
PAGES = {772--781},
URL = {https://www.mdpi.com/2624-599X/6/3/42},
ISSN = {2624-599X}
}

```