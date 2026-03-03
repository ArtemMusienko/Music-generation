![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)

## Music Generation

[![ru](https://img.shields.io/badge/README_на_русском-2A2C39?style=for-the-badge&logo=github&logoColor=white)](README.ru.md)  

The key tools in this code are: **MuseScore 3**, **fluidsynth**, **pyfluidsynth**, **Music21**, and **pretty_midi**.

The peculiarity of this approach to solving the problem is that here is implemented `temperature` - the temperature of the model. The temperature of the model affects the generation. Lower temperatures correspond to a more accurate prediction, and higher temperatures lead to a more random generation.

Three variables are also used to train the model to represent a note: `pitch`, `step`, and `duration`. The pitch (`pitch`) is the quality of the sound as a note number in the **MIDI** format. The step (`step`) is the time elapsed since the previous note or the beginning of the track. The duration (`duration`) is the length of the note in seconds and the difference between the end and start times of the note.

The model's architecture is based on recurrent layers (**RNN**).

[Dataset](https://storage.yandexcloud.net/academy.ai/classical-music-midi.zip) with musical works by famous composers.

> To run this code, I recommend using a **graphics accelerator**
>  **T4** or better!