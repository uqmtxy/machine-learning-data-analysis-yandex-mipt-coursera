# Демонстрация работы алгоритма
Часто оказывается полезно представить результаты вашей работы в виде интерактивной демонстрации, в которую можно будет вводить какие-то данные и получать результат работы вашей модели. В этом задании вам предлагается реализовать такую демонстрацию для вашего алгоритма анализа тональности отзывов на фильмы, используя flask.

Даже если вы никогда не сталкивались с веб-программированием и flask'ом - познакомиться с ним совершенно не сложно. Сделать первые шаги вам поможет прекрасный Викиучебник по Flask: https://ru.wikibooks.org/wiki/Flask

В процессе вы столкнетесь с необходимостью сохранять в файл и загружать питоновский объект - обученный классификатор. Для этого вам пригодится библиотека pickle.

## Структура папок
Всё, что творится внутри этой папки, подвержено своим законам:
* model - папка содержит файл с объектом Pipeline и ноутбук, который преобразует объект Pipeline в файл
* screenshots - папка со снимками экрана работы демонстрации и справки
* templates - папка содержит шаблоны страниц для Flask
* classifier_test.py - проверка работоспособности классификатора отзывов
* demo.py - демонстрация алгоритма
* sentiment_classifier.py - класс классификатора отзывов

## Как запустить
1. Запустить файл demo.py в Visual Studio Code или PyCharm. При таком раскладе запустится сервер, открыть который можно в браузере по этому пути http://localhost:5000/. 
2. Сайт содержит две страницы - http://localhost:5000/demo  с демонстрацией алгоритма и http://localhost:5000/info со справкой.
3. В текстовое поле напишите текст отзыва на англ языке о технике - в ответ получите тональность отзыва. 

P.S. Так как классификатор обучался на малом количестве данных, то возможны ложные предсказания.