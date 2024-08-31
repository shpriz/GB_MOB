# GB_MOB

# python-flask-docker
Итоговый проект курса "Машинное обучение в бизнесе"

Стек:

ML: sklearn, pandas, numpy
API: flask
Данные: с kaggle - https://www.kaggle.com/shivamb/real-or-fake-fake-jobposting-prediction

Задача: предсказать по описанию вакансии является ли она фейком или нет (поле fraudulent). Бинарная классификация

Используемые признаки:

- description (text)
- company_profile (text)
- benefits (text)

Преобразования признаков: tfidf

Модель: logreg

### Создаем и переходим в рабочий каталог, например `GB_homework`

```
$ mkdir GB_homework && cd GB_homework
```

### Клонируем репозиторий и создаем образ
```
$ git clone https://github.com/shpriz/GB_MOB.git
$ docker build -t myprobaserver .
```

### Запускаем контейнер

```
$ docker run -d -p 8180:8180 -p 8181:8181 myprobaserver
```

### Переходим на http://localhost:8181
