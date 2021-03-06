# Проект по предсказанию цен на квартиры в Москве
<p align="center">
  <img src="app/static/images/moscow.jpg" width="1000" title="hover text">
</p>

# Как запустить сервер(linux)?
> 1. ``` sh ./instal_venv.sh ```
> 2. ``` source venv/bin/activate ```
> 3. ``` python3 app/run_server.py ```

# Как запустить парсер
> 1. ``` sh ./instal_venv.sh ```
> 2. ``` source venv/bin/activate ```
> 3. ``` scrapy crawl m2 ```

# Структура moscow_estate.csv
  - **okrug** - Округ
  - **metro** - Ближайшая станция метро 
  - **distance_from_center** - Расстояние от центра Москвы (в км) 
  - **route_time** - Время пути до станции метро пешком
  - **total_area** - Общая площадь квартиры
  - **rooms** - Кол-во комнат
  - **price** - Цена
  
> Пропуски в данных отсутствуют 

## Файлы и папки проекта
1. app - Директория для приложения
    - **data** - Директория с данными для обучения модели
     
    - **model** - Директория с файлами обучения модели и сохраннеными весами модели
     
    - **templates** - Директория с шаблонами для сайта
     
    - **static** - Директория с стилями для сайта
     
    - **run_server.py** - Скрипт запускающий flask сервер
2. parser - Директория со Scrapy проектом парсинга m2.ru
3. requirements.txt - список используемых библиотек
4. install_venv.sh - скрипт установки виртуального окружения и библиотек




