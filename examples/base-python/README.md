Пример решения Классик AI
=========================

Решение реализует необходимый интерфейс:
- отвечает положительно на запрос `/ready/`
- на запрос генерации `/generate/` всегда отвечает одним и тем же стихотворением
- стихотворение в общем случае не отвечает ни одному из критериев качества (получит минимальную оценку), тем не менее оно удовлетворяет ограничениям по формату и будет принято к проверке

Решение реализовано на Python 3 с ипользованием библиотеки [Flask](http://flask.pocoo.org) для запуска веб-сервера.

В `metadata.json` записано окружение и команда запуска:

```json
{
    "image": "sberbank/python",
    "entry_point": "python generator_server.py"
}
```

