# Django
Свободный фреймворк для веб-приложений на языке Python, использующий шаблон проектирования MVC. Проект поддерживается организацией Django Software Foundation.Сайт на Django строится из одного или нескольких приложений, которые рекомендуется делать отчуждаемыми и подключаемыми. (https://docs.djangoproject.com/) <br>
Архитектура Django похожа на «Модель-Представление-Контроллер» (MVC). Контроллер классической модели MVC примерно соответствует уровню, который в Django называется Представление(View), а презентационная логика Представления реализуется в Django уровнем Шаблонов (Template). Из-за этого уровневую архитектуру Django часто называют «Модель-Шаблон-Представление» (MTV) <br>
Данный фреймворк имеет ряд преимуществ: <br>
- встроенный интерфейс администратора с возможностью перевода на многие языки; o диспетчер URL на основе регулярных выражений; <br> 
- расширяемая система шаблонов с тегами и наследованием; o авторизация и аутентификация пользователей; <br>
- система фильтров для построения дополнительных обработчиков запросов; <br>
- система тегов для вывода информации в шаблон; <br>
> Модули(приложения) – это базовые строительные блоки для создания приложений на фреймворке Django.<br>
Чтобы проект был изолированным от других Django-проектов, нужно создать виртуальное окружение с помощью команды python -m virtualenv '<name virtualenviroment>' и активировать его, зайдя в папку Scripts, и вызвать скрипт activate.<br>
Приложение состоит из основных управляемых файлов: models.py , views.py , urls.py.<br>
Для подключения модуля необходимо в файле настроек проекта (settings.py) в массиве INSTALLED_APPS подключить приложение.<br>
Для создания нового модуля необходимо выполнить команду в консоли :python manage.py startapp '<name application>'.<br>
Для того, чтобы запустить приложение, нужно выполнить команду : python manage.py runserver.<br>


### Как с этим работать? 
Для начала установим всё необходимое.

- [X] python -m ensurepip&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;#установщик пакетов или установщик программ, pip устанавливается вместе с Python по умолчанию.
- [X] pip install virtualenv&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;#установка виртуальной среды.	
- [X] python -m venv ...&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;#создание виртуальной среды.
- [X] pip install django&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;#установка Django.
- [X] django-admin startproject ...&nbsp;&nbsp;&nbsp;&nbsp;#создаём наш проект.

> дополнительно если не установлены, пакеты которые нам понадобятся<br>

- [X] pip install requests&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;#установит пакет requests, который используется для выполнения HTTP-запросов.
- [X] pip install flask&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;#установит пакет Flask

![image](https://github.com/tvgVita69/Django/assets/98489171/cfd80a6f-ed6f-4667-b383-51441295b670)

### 1. Установка менеджера пакетов pip.
Как уже было в комментарии, пакет pip устанавливается вместе с Python по умолчанию. Только в старых версиях его ставили отдельно.<br>
Как проверить, установлен он или нет? И какая версия?<br>
Введём команду<br>
``pip -V`` или ``python -m pip --version`` или ``python3 -m pip --version``
<br>Если пакет не установлен, значит устанавливаем, вводим команду<br>
``python -m ensurepip``
<br>Если пакет установлен, значит продолжим далее устанавливать необходимые пакеты.<br>
Конечно можно обновить устаревшую версию pip командой ``python.exe -m pip install --upgrade pip``, <br>
но при дальнейшей установке пакетов будет предложено обновить пакет pip если они устарели. См. ниже. <br>

### 2. Установка виртуальной среды.	
``pip install virtualenv``

```
(venv) PS D:\Python And Data Analysis> pip install virtualenv
Collecting virtualenv
  Downloading virtualenv-20.25.0-py3-none-any.whl.metadata (4.5 kB)
  Using cached filelock-3.13.1-py3-none-any.whl.metadata (2.8 kB)
Requirement already satisfied: platformdirs<5,>=3.9.1 in d:\python and data analysis\venv\lib\site-packages (from virtualenv) (4.1.0)
Downloading virtualenv-20.25.0-py3-none-any.whl (3.8 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.8/3.8 MB 9.3 MB/s eta 0:00:00
Downloading distlib-0.3.8-py2.py3-none-any.whl (468 kB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 468.9/468.9 kB 9.8 MB/s eta 0:00:00
Using cached filelock-3.13.1-py3-none-any.whl (11 kB)
[notice] A new release of pip is available: 23.3.1 -> 24.0
[notice] To update, run: python.exe -m pip install --upgrade pip
```
![image](https://github.com/tvgVita69/Django/assets/98489171/64d370ae-ab82-4ac3-b9d7-b253232fb999)

### 3. Создаём виртуальную среду и активируем её.
``python -m venv имя ``

> например: ``python -m venv django``

![image](https://github.com/tvgVita69/Django/assets/98489171/e96c67b0-0ed0-40fc-88e1-f6a1ff65ef4f)

> Далее перейдём в папку Scripts и активируем виртуальную среду.
- cd django
  - cd Scripts
    - ``activate``

![image](https://github.com/tvgVita69/Django/assets/98489171/c14df737-adc3-4a40-b044-9e789e0eae6c)

### 4. Установка Django.

> Перейдём в папку django
- cd ..
- ``pip install django``

![image](https://github.com/tvgVita69/Django/assets/98489171/8167c2fd-97d7-4155-add5-3913f6196e2c)

### 5. Создаём наш проект.
``django-admin startproject имя_проекта``

> например: ``django-admin startproject  project_01``

![image](https://github.com/tvgVita69/Django/assets/98489171/6da8ac03-b7d3-4fb9-bd77-2d3fae717faf)

Появилась папка с файлами и названием нашего проекта.

![image](https://github.com/tvgVita69/Django/assets/98489171/91903193-bc6c-4ecd-83c6-1fb5b07c458b)










