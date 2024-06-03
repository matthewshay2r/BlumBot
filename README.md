[<img width="889" alt="image" src="https://github.com/matthewshay2r/BlumBot/assets/148196025/d8f2f17f-556a-473d-b3dc-fb78bbe1d342">](https://t.me/shay2r)


## Функционал  
| Функционал                                                     | Поддерживается  |
|----------------------------------------------------------------|:---------------:|
| Многопоточность                                                |        ✅        |
| Привязка прокси к сессии                                       |        ✅        |
| Авто-сбор наград                                               |        ✅        |
| Авто-сбор наград за рефиралов                                  |        ✅        |
| Автоматческое прохождение игры                                 |        ✅        |
| Поддержка tdata / pyrogram .session / telethon .session        |        ✅        |


## Настройки
| Настройка                | Описание                                                                                      |
|--------------------------|-----------------------------------------------------------------------------------------------|
| **API_ID / API_HASH**    | Данные платформы, с которой запускать сессию Telegram _(сток - Android)_                      |
| **ACC_DELAY**            | Минимальнае задержка между подключениями к аккаунтам _(напр. [1, 15])_                        |
| **USE_PROXY**            | Использовать-ли прокси из файла `proxy.txt` _(True / False)_                                  |
| **POINTS**               | Сколько поинтов будет получено после игры _(напр. [200, 300])_                                |
| **PlAY_GAME**            | Играть-ли в игру? _(True / False)_                                                            |
| **SLEEP_GAME_TIME**      | Задержка между играми _[50, 100]_                                                             |
| **MINI_SLEEP**           | Задержка между любыми действиями _[3, 7]_                                                     |

## Предварительные условия
Прежде чем начать, убедитесь, что у вас установлено следующее:
- [Python](https://www.python.org/downloads/) версии 3.10 или 3.11.


## Получение API ключей
1. Перейдите на сайт [my.telegram.org](https://my.telegram.org) и войдите в систему, используя свой номер телефона.
2. Выберите **"API development tools"** и заполните форму для регистрации нового приложения.
3. Запишите `API_ID` и `API_HASH` в файле `config.py`, предоставленные после регистрации вашего приложения.


## Установка
Вы можете скачать [**Репозиторий**](https://github.com/matthewshay2r/BlumBot) клонированием на вашу систему и установкой необходимых зависимостей:
```shell
~ >>> git clone https://github.com/matthewshay2r/BlumBot.git
~ >>> cd BlumBot

# Linux/MacOS
~/BlumBot >>> python3 -m venv venv
~/BlumBot >>> source venv/bin/activate
~/BlumBot >>> pip3 install -r requirements.txt
~/BlumBot >>> nano data/config.py # Здесь вы обязательно должны указать ваши API_ID и API_HASH, по желанию другие настройки
~/BlumBot >>> python3 main.py

# Windows
~/BlumBot >>> python -m venv venv
~/BlumBot >>> venv\Scripts\activate
~/BlumBot >>> pip install -r requirements.txt
~/BlumBot >>> редактируем под себя data/config.py # Указываете ваши API_ID и API_HASH, по желанию другие настройки
~/BlumBot >>> python main.py
```
