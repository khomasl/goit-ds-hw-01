# Docker-команда FROM вказує базовий образ контейнера
# Наш базовий образ - це Linux з попередньо встановленим python-3.10
FROM python:3.11

# Встановимо змінну середовища
ENV POETRY_VERSION=2.0.0 \
    POETRY_VIRTUALENVS_CREATE=false \
    POETRY_NO_INTERACTION=1 \
    APP_HOME=/app

RUN pip install "poetry==$POETRY_VERSION"
# Встановимо робочу директорію всередині контейнера
WORKDIR $APP_HOME

# Скопіюємо інші файли в робочу директорію контейнера
COPY pyproject.toml poetry.lock* $APP_HOME/

# Встановимо залежності всередині контейнера
RUN poetry install --no-root

COPY . $APP_HOME
# Позначимо порт, де працює застосунок всередині контейнера
#EXPOSE 5000

# Запустимо наш застосунок всередині контейнера
# CMD ["poetry", "run", "python", "main.py"]
ENTRYPOINT ["poetry", "run", "python", "main.py"]
