# Django
Это веб-фреймворк Python высокого уровня, который способствует быстрой разработке и чистому, прагматичному дизайну. Созданный опытными разработчиками, он берет на себя большую часть хлопот веб-разработки, поэтому вы можете сосредоточиться на написании своего приложения, не изобретая велосипед. Это бесплатно и с открытым исходным кодом. (https://docs.djangoproject.com/)

### Как с этим работать? 
Для начала установим всё необходимое.

- [X] python -m ensurepip             #установщик пакетов или установщик программ, pip устанавливается вместе с Python по умолчанию.
- [X] pip install virtualenv		      #установка виртуальной среды.	
- [X] python -m venv ...  		        #создание виртуальной среды.
- [X] pip install django		          #Установка Django.
- [X] django-admin startproject ...	  # создаём наш проект
> дополнительно если не установлены<br>
- [X] pip install requests             #установит пакет requests, который используется для выполнения HTTP-запросов.
- [X] pip install flask                #установит пакет Flask

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





