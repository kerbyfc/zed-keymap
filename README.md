# zed-keymap

Сочетания клавиш [Zed](https://zed.dev): vim-режим под раскладку Colemak (перенос colemak.vim),
окна, фолды и копирование пути к файлу по `cmd-shift-c` на macOS и `ctrl-shift-c` на Windows и Linux
(в конфиге — `secondary-shift-c`).

## Установка

### macOS / Linux

Копией:

```sh
cp keymap.json ~/.config/zed/keymap.json
```

Или симлинком, чтобы правки сразу попадали в репозиторий:

```sh
ln -sf "$PWD/keymap.json" ~/.config/zed/keymap.json
```

### Windows

Zed читает `%APPDATA%\Zed\keymap.json`. В PowerShell из папки репозитория — копией:

```powershell
Copy-Item keymap.json "$env:APPDATA\Zed\keymap.json" -Force
```

Или симлинком (нужен режим разработчика в «Параметры → Для разработчиков» либо PowerShell от администратора):

```powershell
New-Item -ItemType SymbolicLink -Path "$env:APPDATA\Zed\keymap.json" -Target "$PWD\keymap.json" -Force
```
