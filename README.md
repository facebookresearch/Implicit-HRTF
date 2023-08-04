<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/80x15.png" /></a> This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

# Implicit HRTF Modeling Using TCN
[Link to the ICASSP 2021 Paper.](https://ieeexplore.ieee.org/document/9414750)

This is an open-source dataset release for the paper published in ICASSP 2021 conference: "Implicit HRTF Modeling Using Temporal Convolutional Networks". This paper presents a data-driven approach to learn HRTFs implicitly with a neural network that achieves state of the art results compared to traditional approaches but relies on a much simpler data capture that can be performed in arbitrary, non-anechoic rooms.


# Dataset
There are eight white-noise sequences in the dataset folder. Each sequence contains audio files: the paired mono and the binaural audio signals, as well as the 6DoF tracking data for the mono source. The audio is recorded at 48kHz, and the tracking data at 240fps. The tracking data and audio samples are in sync. The paper provides additional information regarding the dataset collection setup and process.
```
├── seq%04d
│   ├── audio
│   |   ├── mono.wav # the transmitted/playedback white-noise signal
│   |   ├── binaural.wav # the binaural recorded signal
│   ├── tracking
│   |   ├── tx.txt # 6DoF tracking data of the moving mono source [x,y,z,qx,qy,qz,qw]
│   |   ├── rx.txt # 6DoF of listener which is static and always at the center
|   ├── topview.mp4 # topview plot with binaural audio
```


## License
This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>, as found in the LICENSE file.

## Citation
If you find this repository useful in your research, please consider giving a star ⭐ and cite our ICASSP 2023 paper by using the following BibTeX entrys.
```
@inproceedings{gebru2021implicit,
  title={Implicit hrtf modeling using temporal convolutional networks},
  author={Gebru, Israel D and Markovi{\'c}, Dejan and Richard, Alexander and Krenn, Steven and Butler, Gladstone A and De la Torre, Fernando and Sheikh, Yaser},
  booktitle={ICASSP 2021-2021 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
  pages={3385--3389},
  year={2021},
  organization={IEEE}
}
```
