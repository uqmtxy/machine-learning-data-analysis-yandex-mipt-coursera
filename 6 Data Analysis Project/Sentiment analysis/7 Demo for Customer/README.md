# Демонстрация алгоритма для заказчика
На этой неделе вы в некотором смысле поведете итог вашей работы над проектом - реализуете демонстрацию для алгоритма, который не просто решает задачу анализа тональности отзывов, а еще и обучен на собранной лично вами выборке, а также прошел тест на небольшом наборе примеров от заказчика.

Адаптируйте вашу демонстрацию из предыдущих недель под новый алгоритм и подготовьте несколько новых примеров (теперь уже с ним).

## Структура папок
Всё, что творится внутри этой папки, подвержено своим законам:
* model - папка содержит файл с объектом Pipeline
* screenshots - папка со снимками экрана работы демонстрации и справки
* templates - папка содержит шаблоны страниц для Flask
* classifier_test.py - проверка работоспособности классификатора отзывов
* demo.py - демонстрация алгоритма
* sentiment_classifier.py - класс классификатора отзывов

## Как запустить
1. Запустить файл demo.py в Visual Studio Code или PyCharm. При таком раскладе запустится сервер, открыть который можно в браузере по этому пути http://localhost:5000/. 
2. Сайт содержит две страницы - http://localhost:5000/demo  с демонстрацией алгоритма и http://localhost:5000/info со справкой.
3. В текстовое поле напишите текст отзыва на русском языке о смартфоне - в ответ получите тональность отзыва. 