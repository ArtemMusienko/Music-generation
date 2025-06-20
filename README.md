## Music Generation
Ключевыми инструментами в данном коде являются **MuseScore 3**, **fluidsynth**, **pyfluidsynth**, **Music21** и **pretty_midi**.

Особенность такого подхода в решении задачи в том, что здесь реализована `temperature` - температура модели. Температура модели влияет на генерацию. Более низкие температуры соответствуют более точному предсказанию, а более высокие температуры приводят к более случайной генерации.

Также используются для обучения модели три переменные для представления ноты: `pitch`, `step` и `duration`. Высота звука (`pitch`) - это качество восприятия звука в виде номера ноты в формате **MIDI**. Шаг (`step`) - это время, прошедшее с предыдущей ноты или начала трека. Длительность (`duration`) - это продолжительность воспроизведения ноты в секундах и разница между временем окончания и началом ноты.

[Датасет](https://storage.yandexcloud.net/academy.ai/classical-music-midi.zip) с музыкальными произведениями известных композиторов.