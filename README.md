# save_webpage (fork by awebmaster)

```
UPD1: Updated packages copatible with Python 3.9.1
UPD2: Stubbed encoding for CSS files (utf-8)
```

## Install and Use

```
1. Download and istall python 3.9.1
2. Clone this repository and navigate to the root
3. Install all packages from file 'requirements' (pip install <package_name>)
4. Run the script: 
python save_webpage.py http://awebmaster.ru --output awebmaster_dist
```

```
usage: save_webpage.py [-h] [-o OUTPUT] [--version] [-q] [--insecure]
                       [--forbidden-urls FORBIDDEN_URLS [FORBIDDEN_URLS ...]]
                       [--follow-links] [-b BASE_URL]
                       [--index-html INDEX_HTML]
                       [--mode {relative,absolute,nochange}]
                       [--config PATH_TO_CONFIG_FILE]
                       list_of_seed_urls [list_of_seed_urls ...]

Save_Webpage Save webpages and all its resources. Apply search and replace of
matched strings.

positional arguments:
  list_of_seed_urls     Seed urls

optional arguments:
  -h, --help            show this help message and exit
  -o OUTPUT, --output OUTPUT
                        Output directory
  --version             show program's version number and exit
  -q, --quite           don't show verbose url get log in stderr
  --insecure            Ignore the certificate
  --forbidden-urls FORBIDDEN_URLS [FORBIDDEN_URLS ...]
                        Forbidden urls
  --follow-links        Follow links
  -b BASE_URL, --base-url BASE_URL
                        Resolves relative links using URL as the point of
                        reference
  --index-html INDEX_HTML
                        Default index file
  --mode {relative,absolute,nochange}
                        Mode of extraction
  --config PATH_TO_CONFIG_FILE
                        Path to configuration file

save_webpage.py: Takes a list of url's and download the websites with all its
internal resource files. Transforms all internal resources so that they link
to local files. Process css files exctracting new resource and converting
url's. Possibility to replace javascript and html files using custom
substitutions. Full Unicode/UTF-8 support.
```
# Скрипт для скачивания веб-страницы со всеми ресурсами (html/css/js/картинки/...)
## Установка и запуск
```
1. Скачать и установить python 3.9.1
2. Склонируйте этот репозиторий и перейдите в корень папки
3. Установите все пакеты из файла 'requirements' (команда для установки пакета: pip install <наимен_пакета>)
4. Запуск скрипта: 
python save_webpage.py http://awebmaster.ru --output awebmaster_dist

В результате рядом со скриптом появится папка awebmaster_dist с содержимым веб-страницы
```
