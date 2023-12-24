# Проект 1. Анализ резюме из HeadHunter (PJ)
---
## Оглавление
[1. Описание проекта](https://github.com/OlgaKopaneva/Resume_HH_/blob/main/README.md#Описание-проекта)

[2. Какой кейс решаем](https://github.com/OlgaKopaneva/Resume_HH_/blob/main/README.md#Какой-кейс-решаем)

[3. Краткая информация о данных](https://github.com/OlgaKopaneva/Resume_HH_/blob/main/README.md#Краткая-информация-о-данных)

[4. Этапы работы над проектом](https://github.com/OlgaKopaneva/Resume_HH_/blob/main/README.md#Этапы-работы-над-проектом)

[5. Результат](https://github.com/OlgaKopaneva/Resume_HH_/blob/main/README.md#Результат)

[6. Выводы](https://github.com/OlgaKopaneva/Resume_HH_/blob/main/README.md#Выводы)

---

### Описание проекта
*Проблематика:* часть соискателей не указывает желаемую заработную плату, когда составляет своё резюме  
*Общая цель:* компания HeadHunter хочет построить модель, которая бы автоматически определяла примерный уровень заработной платы, подходящей пользователю, исходя из информации, которую он указал о себе  
*Постановка задачи текущего проекта:* преобразовать, исследовать и очистить данные представленного датасета с резюме 


:arrow_up: [к оглавлению](https://github.com/OlgaKopaneva/Resume_HH_/blob/main/README.md#Оглавление)

---
### Какой кейс решаем
Нужно преобразовать, исследовать и очистить данные представленного датасета с резюме.

**Метрика качества:**  
Отсутствие в итоговом датасете дубликатов, пропущенных значений, выбросов, все категориальные переменные переведены в числовой / логический вид; данные готовы к использованию в построении модели


:arrow_up: [к оглавлению](https://github.com/OlgaKopaneva/Resume_HH_/blob/main/README.md#Оглавление)

---
### Краткая информация о данных
Исходный датасет размещен по ссылке: https://drive.google.com/file/d/1ZfplJnpXWvzv98_4axXdXWyu-IbzBf3d/view?usp=sharing (перед запуском ноутбука его и ноутбук необходимо сохранить локально)

:arrow_up: [к оглавлению](https://github.com/OlgaKopaneva/Resume_HH_/blob/main/README.md#Оглавление)

---
### Этапы работы над проектом
1. Бвзовый анализ структуры данных 
2. Преобразование данных (формирование возможных к дальнейшему использованию признаков из сложных исходных форматов; преобразование категориальных переменных (обобщение, one-hot-encoding), пересчет валюты)
3. Разведывательный анализ данных (построение графиков зависимостей между признаками)
4. Очистка данных (удаление дубликатов, заполнение и удаление пропусков, удаление выбросов)

:arrow_up: [к оглавлению](https://github.com/OlgaKopaneva/Resume_HH_/blob/main/README.md#Оглавление)

---
### Результат
Модель готова к дальнейшему использованию заказчиком для прогнозирования заработной платы

:arrow_up: [к оглавлению](https://github.com/OlgaKopaneva/Resume_HH_/blob/main/README.md#Оглавление)

---
### Выводы
- исходный датасет без преобразования не пригоден для построения моделей (состоит из множества сложно представленных категориальных признаков)  
- в результате работы датасет приведен к состоянию, готовому для дальнейшего использования  
- полученный датасет имеет довольно мало числовых характеристик, что может исказить итоговый прогноз
- по итогам проведенного анализа данных сделаны следующие основные выводы:
    * возраст большинства кандидатов находится в промежутке от 20 до 40 лет, мода распределения - 30 лет (что соответствует ожиданиям)
    * опыт работы большинства кандидатов находится в промежутке от 3-5 до 12-15 лет (мода распределения - 7 лет)
    * зарплатные ожидания большинства кандидатов укладываются в пределы 30 - 100 тыс. руб. (мода распределения - 50 тыс. руб.), но есть и значения за границей 300 тыс. руб.
    * медианный уровень заработной платы зависит от уровня образования для специалистов и служащих (где образование является требованием), для представителей рабочих профессий образование не играет определяющей роли
    * медианная ожидаемая заработная плата наиболее высока в Москве, далее идет второй по величине город РФ - Санкт-Петербург (что ожидаемо), очевидной разницы между городами-миллионниками и прочими городами не отмечено
    * обращает на себя внимание также наибольший разброс зарплат в Москве в сравнении с другими городами (большее расстояние между 1 и 3 квартилью)
    * тепловая карта распределения з/п в зависимости от уровня образования демонстрирует очевидную пользу высшего образования: соискатели с данным уровнем образования претендуют на более высокие зарплаты в течение всей трудовой жизни и, собственно трудовая жизнь у них длится дольше, также из плюсов - наиболее быстрый карьерный рост


:arrow_up: [к оглавлению](https://github.com/OlgaKopaneva/Resume_HH_/blob/main/README.md#Оглавление)
