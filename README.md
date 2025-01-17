# 🎤 Voice Synthesis Project
Проект для синтеза речи с использованием модели fish-speech/xtts.
Позволяет преобразовывать текст в речи с клонированием голоса.

## 🎧 Демонстрация

### Образец 
<audio src="./voice_samples/anya.wav" controls></audio>

### Результат синтеза
<audio src="./output/output.wav" controls></audio>

## ✨ Особенности

- Клоинрование голоса из WAV-файла
- Поддержка русского языка
- Высокое качество синтеза
- Простой API

## 🔧 Требования

- Python 3.11 - 3.11.9
- Библиотека TTS
- Образец голоса (WAV, 16kHz, moho)
- Минимум 4GB RAM

## ⚙️ Установка

### Клонирование репозитория

1. Клонируйте проект:
    ```bash
    git clone git@github.com:5ekastanx/Voice-Synthesis.git
    cd Voice-Synthesis
    ```

## Обновление Python до версии 3.11

Если у вас установлена другая версия Python, выполните следующие
шаги:

1. Деактивируйте текущее виртуальное окружение (если есть):
    ```bash
    deactivate
    ```

2. Активируйте окружение:
    ```bash
    new_venv/bin/activate
    ```

3. Установите TTS:
    ```bash
    pip install TTS
    ```

## 📁 Структура проекта

```
Voice-Synthesis/
├── main.py              # Основной скрипт
├── voice_samples/       # Образцы голоса
│   └── aliya.wav       # Пример образца
└── output/             # Выходные файлы
    └── output.wav
```


## 🚀 Использование

1. Поместите WAV-файл с образцом голоса в `voice_samples/`

2. Запустите синтез:
    ```bash
    text = "Ваш текст для синтеза"
    synthesize(
        text=text,
        speaker_wav=speaker_wav
    )
    ```

3. Запустите скрипт:
    ```bash
    python main.py
    ```


## ❗ Устранение проблем

- **CUDA out of memory**: Уменьшите размер текста
- **Искажение голоса**: Проверьте частоту дискретизации (16kHz)
- **FileNotFoundError**: Проверьте пути к файлам