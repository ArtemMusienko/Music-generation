![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

## Music Generation
Ключевыми инструментами в данном коде являются: **MuseScore 3**, **fluidsynth**, **pyfluidsynth**, **Music21** и **pretty_midi**.

Особенность такого подхода в решении задачи в том, что здесь реализована `temperature` - температура модели. Температура модели влияет на генерацию. Более низкие температуры соответствуют более точному предсказанию, а более высокие температуры приводят к более случайной генерации.

Также используются для обучения модели три переменные для представления ноты: `pitch`, `step` и `duration`. Высота звука (`pitch`) - это качество восприятия звука в виде номера ноты в формате **MIDI**. Шаг (`step`) - это время, прошедшее с предыдущей ноты или начала трека. Длительность (`duration`) - это продолжительность воспроизведения ноты в секундах и разница между временем окончания и началом ноты.

[Датасет](https://storage.yandexcloud.net/academy.ai/classical-music-midi.zip) с музыкальными произведениями известных композиторов.
