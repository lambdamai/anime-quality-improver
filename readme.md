[![Телеграмм Канал](https://img.shields.io/badge/Join-Telegram%20Channel-0088cc)](https://t.me/lambdamai)
[![Телеграмм Чат](https://img.shields.io/badge/Join-Telegram%20Chat-0088cc)](https://t.me/joinchat/01_ttlSQj3hjZTg6)
[![Телеграмм Чат](https://img.shields.io/badge/Subscribe-YouTube-FF0000)](https://www.youtube.com/channel/UC8fGhHpoUm-1ZWITOM98N9A)
[![Телеграмм Чат](https://img.shields.io/badge/Follow-Twitch-6441a5)](https://www.twitch.tv/lambdamai)

![One Love](cover.jpg)

# Anime  Quality Improver

Построено на базе [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN). Улучшает качество изображения аниме в разы,
пример ниже это преобразование изображения 420x240 в QHD (2560x1440)

| Оригинал  (420x240)      | Обработанное (2560x1440)          |  
| ------------- |:-------------:|  
| ![Оригинал](example.jpg)      | ![One Love](out.jpg) |  

### Что нужно, что бы запустить?

### 1. Клонировать репозиторий

```bash
 git clone  https://github.com/lambdamai/anime-quality-improver.git
```

### 2. Поставить виртуальное окружение

```bash
virtualenv venv && source venv/bin/activate
```

Для винды

```bash
python -m virtualenv venv && venv\Scripts\activate
```

### 3. Поставить зависимости

```bash
pip install -r requirements.txt
```
### 4. Ставим  Real-ESRGAN

```bash
pip install git+https://github.com/xinntao/Real-ESRGAN.git@772923e207582f4983aaf77e3b55ae1f6974b994
```

### 5. [Скачать](https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.2.4/RealESRGAN_x4plus_anime_6B.pth) модель, создать папку `model` и положить в нее модель 

### 6. Запустить jupyter

```bash
jupyter notebook
```

### P.S.

Дополнительно может понадобиться  `ffmpeg`

```bash
sudo apt-get install ffmpeg 
```

И `libx264` для сохранения видео в лучшем качестве 

```bash
sudo apt-get install  libx264-dev
```
