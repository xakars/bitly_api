# Файл main.py

Скрипт умеет сокращать длинные ссылки используя сервис https://app.bitly.com. 
Если же передать уже ранее созданую сокращенную ссылку то покажет статистику переходов по этой ссылке.

Команда для установки зависимостей:
``` 
pip install -r requirements.txt
``` 
Чтобы пользоваться скрипотом Вам понадобится токен сгенерированный в сервисе https://app.bitly.com. 
Задайте BITLY_TOKEN в файле .env

Например:
```
BITLY_TOKEN=bebc2fcb8bfe1defd43d654d1930c06f48fbbe67
```
Запустите скрипт командой:
```
python main.py {Ссылка которую надо сократить || Битлинк}
```
Пример использования:
```console
$ python main.py https://climate.mit.edu/
Битлинк: https://bit.ly/3z15YY8
```
```console
$ python main.py https://bit.ly/3z15YY8
По вашей ссылке прошли: 3 раз(а)
```
