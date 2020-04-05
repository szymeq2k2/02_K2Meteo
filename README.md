# Program K2-Meteo

## Recording and display current weather and forecast on K2 mountain. 

### Task description:
>Do wyprawy na K2 przygotowuje się grupa nieokrzesanych śmiałków, oczywiście jak na prawdziwych profesjonalistów przystało o sprawdzeniu pogody przypomniało im się na 3 dni przed wylotem do Islamabadu.
>Grupa koniecznie musi monitorować aktualne dane pogodowe oraz prognozę na najbliższe 5 dni.
>Jesteś ich ostatnią nadzieją. Musisz przygotować prosty skrypt, który spełnia następujące założenia:
>
>1. Jest dostępny na GitHub'ie.
>2. Napisany w Python.
>4. Pełna historia commitów w języku angielskim.
>5. Wszystkie zewnętrzne biblioteki zapisane w pliku requirements.txt.
>6. Dane powinny być zapisywane do bazy danych SQLite w czasie rzeczywistym.
>7. Prognoza pogody dostępna na wykresie.
>8. Możliwość pobrania z bazy danych min, max, avg. dla temperatury z całego okresu składowania danych.
>9. Prosta dokumentacja użycia.
>
>Dane pobieramy ze strony:
>https://openweathermap.org/api
>
>Należy założyć darmowe konto oraz poczekać na aktywację klucza, który należy następnie użyć podczas pobierania danych.
>
>Pozycja K2 = {"lat": "35.88", "lon": "76.51"}
>
## Table of contents

2. [Technologies](#technologies)
4. [Status](#status)
5. [Contact](#contact)

## Technologies

- Python v3.7
- SQLite

## Status
Project is: _in progress_

To do:
 - [ ] Main Branch
    - [x] SQLite
        - [x] Create database
        - [x] Add data do database
        - [x] Read max value from database
    - [x] OpenWeatherMap
        - [x] Read current weather data and forecast
        - [x] Recording current weather data   
        - [x] Reading forecast 
    - [x] Graph
        - [X] Generate graph and save to file
    - [x] UI 
        - [x] Command structure
    - [x] Register data in Real-Time
 - [ ] Readme
    - [ ] Instruction
   
#### Database table

##### Table 1. current_weather

| DataId | DateTime         | Temp | TempMin | TempMax |
| :---:  |:---:             |:---: |:---:    |:---:    |
| 1      | 2020-04-04 12:00 | 24.5 |  20.5   | 24.5    |
| 2      | 2020-04-04 12:00 | 24.4 |  20.5   | 24.5    |
| ..     | ...              | ...  |  ...    | ...     |
   
#### Graph

After each plot graph it will be saved on this path:
      
      K2Meteo -> Data
 
Example graph:

![](img/Graph_example.png)
 
## Contact
Created by [pjuszcze@gmail.com](mailto:pjuszcze@gmail.com)