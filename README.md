# PrAutoEditorScript

## Описание

Bat скрипт для перетаскивания на него видео (Drag & drop)

---


## Одним

```bash
# Чтоб воспользоватся - переименуй видео файл в 1.mp4
auto-editor "1.mp4" --export premiere --margin 0.2sec
```

---

## Драг

```bash
@echo off

REM Проверяем, был ли указан файл в аргументах командной строки
if "%~1"=="" (
    echo Вы не перетащили файл на скрипт.
    pause
    exit /b
)

REM Проверяем, существует ли указанный файл
if not exist "%~1" (
    echo Файл %~1 не существует.
    pause
    exit /b
)

REM Ваш код с использованием перетащенного файла
auto-editor "%~1" --export premiere --margin 0.2sec

pause

```

---

# Ссылки
| Описание | Ссылка |
| ------ | ------ |
Репо: | [github.com/gitalexhubuser/PrAutoEditorScript](https://github.com/gitalexhubuser/PrAutoEditorScript)
