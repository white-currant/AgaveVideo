# Agave Video

A batch video converter for macOS: drop videos or a folder, pick a format and size, press Convert. ProRes (Proxy to 4444), H.264 and HEVC in MP4 / MOV / M4V, animated GIF, or just the audio track as WAV or M4A. Encoding is done by macOS itself (VideoToolbox), no third-party libraries. *[Русская версия ниже.](#agave-video-1)*

## Install

**One command, nothing else needed:**

```bash
curl -fsSL -o /tmp/AgaveVideo.dmg https://github.com/white-currant/AgaveVideo/releases/latest/download/AgaveVideo.dmg \
  && hdiutil attach -nobrowse -quiet -mountpoint /tmp/AgaveVideo-dmg /tmp/AgaveVideo.dmg \
  && rm -rf "/Applications/Agave Video.app" && cp -R "/tmp/AgaveVideo-dmg/Agave Video.app" /Applications/ ; \
hdiutil detach -quiet /tmp/AgaveVideo-dmg; rm -f /tmp/AgaveVideo.dmg
```

**Or by hand:** download `AgaveVideo.dmg` from [Releases](https://github.com/white-currant/AgaveVideo/releases) and drag Agave Video to Applications. **Or** through [Currant](https://github.com/white-currant/Currant), the white-currant app catalog.

Updates arrive automatically via [Sparkle](https://sparkle-project.org) or from the "Check for Updates…" menu.

Uninstall: delete `/Applications/Agave Video.app`.

---

# Agave Video

Пакетный конвертер видео для macOS. Перетащили видео или папку, выбрали формат и размер, нажали «Конвертировать».

- **ProRes** 422 Proxy, LT, 422, HQ и 4444 — монтажные программы открывают и перематывают его без задержек.
- **H.264** и **HEVC (H.265)** в MP4, MOV или M4V, три уровня качества, «быстрая перемотка» (опорный кадр каждую секунду).
- **GIF** — анимация без звука, 10–25 кадров в секунду.
- **WAV** и **M4A** — только звуковая дорожка.
- Уменьшение кадра (4K … 360p по короткой стороне), смена частоты кадров, звук можно убрать.
- Готовые файлы ложатся рядом с оригиналом в подпапку с названием формата или в выбранную папку.

Кодирует сама macOS, без сторонних библиотек. macOS 14 и новее, Apple Silicon и Intel.

MKV, WebM и AVI система не читает — такие файлы приложение не принимает и сообщает об этом.

## Установка

Скачайте `AgaveVideo.dmg` со страницы [Releases](https://github.com/white-currant/AgaveVideo/releases/latest), откройте и перетащите Agave Video в «Программы». Или через витрину [Currant](https://github.com/white-currant/Currant). Обновления приходят автоматически ([Sparkle](https://sparkle-project.org)); вручную — меню «Проверить обновления…».

Родственное приложение для звука — [Agave Audio](https://github.com/white-currant/Agave).
