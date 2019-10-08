S4D Diarization Toolkit developed by Lium group

Introduction
============

SIDEKIT for diarization (s4d as short name) is an open source package extension of SIDEKIT for Speaker diarization .
It officially developed by LIUM group from France.

URL is aviliable at: https://lium.univ-lemans.fr/s4d/  
URL for SIDEKIT: https://projets-lium.univ-lemans.fr/s4d/  
Official github:  https://git-lium.univ-lemans.fr/Meignier/s4d  

I used their toolkit for doing some diarization experiment using kaldi to extract features

Installation
============

I recommend you use anaconda, and create a new working envrionment by:  

    conda env create -f environment.yml -p <your env path>

Alternatively, install a simple Python virtual environment with:

    virtualenv -p python3.6 .env
    . .env/bin/activate
    pip install -r requirements.txt

Usage
=====

    python gl_bic_ahc_viterbi.py [wavPath] [mfccMethod] [OutputPath]

e.g.

    python gl_bic_ahc_viterbi.py example1.wav s4d ./speakers
