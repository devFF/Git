# Git
## Установка git
Ubuntu 
```bash
sudo apt update # на всякий случай смотрим новые версии
sudo apt install git-all
```
Windows - GitHub Desktop (CLI + GUI)

## Настройка git
```bash
git config --global user.name "<имя фамилия>"
git config --global user.email "<ваш емейл>"
```

## Аккаунт на github
```bash
# Создание ssh-ключей
ssh-keygen -t ed25519  -C "your_email@example.com"
# Дальше будет несколько вопросов. На все вопросы нужно нажимать Enter.

# Запуск агента ssh, который следит за ключами - для windows не надо
eval "$(ssh-agent -s)"

# Добавления нового ssh-ключа в агент - для windows не надо
ssh-add ~/.ssh/id_ed25519
```

Затем нужно открыть настройки аккаунта на github и перейти в раздел SSH и GPG keys - [ссылка](https://github.com/settings/keys). Нажать на кнопку New SSH key. Скопировать содержимое файла *~/.ssh/id_ed25519.pub* (Linux) или *%userprofile%\ssh\id_ed25519.pub* в Windows.


