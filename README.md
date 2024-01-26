# Описание
Модель, который добавляет в текст недостающие пунктуационные знаки и удаляет лишние слова ради лаконичности, используя для этого ChatGPT

# Установка
`pip install deco_text`

# Начало
.. code-block:: python
  # Импортируем модуль
  import deco_text
  
  # Вызываем инициализацию
  # По умалчанию, когда в функцию предаётся None, она берёт OpenAI API токен из переменной окружения с именем OPENAI_API_KEY. Если изначально её нет, то происходит попытка загрузить .env файл в папке с проектом.
  deco_text.init()
  
  # Функция для обработки "сырого" текста, как пргумента, которая возвращает строку с уже украшенным текстом
  deco_text.decorate_text("короче забыл чё хотел сказать ну в общем как у тебя дела")
