# Соревнование: [WSDM Cup - Multilingual Chatbot Arena](https://www.kaggle.com/competitions/wsdm-cup-multilingual-chatbot-arena/overview)


## Оглавление

1. [Аннотация соревнования](#аннотация-соревнования)
2. [Работа с выделением текста](#описание-данных)
3. [Таймлайн проекта](#таймлайн-проекта)
4. [Активная разборатка решений](#notebooks)
5. [Защита проекта](#reports)


## Аннотация соревнования
This competition challenges you to predict which responses users will prefer in a head-to-head battle between chatbots powered by large language models (LLMs). You'll be given a dataset of conversations from the Chatbot Arena, where different LLMs generate answers to user prompts. By developing a winning machine learning model, you'll help improve how chatbots interact with humans and ensure they better align with human preferences.

## Описание данных
**train.parquet**

* `id` - A unique string identifier for the row.
* `prompt` - The prompt that was given as an input to both models.
* `response_[a/b]` - The response from model_[a/b] to the given prompt.
* `winner` - The judge's selection. The ground truth target column.
* `model_[a/b]` - The identity of model_[a/b]. Only included in train.parquet.
* `language` - The language used in the prompt. Only included in train.parquet.

**test.parquet**

* `id` - A unique integer identifier for the row.
* `prompt`
* `response_[a/b]`
* `scored` - Whether or not the row is currently scored. During the model training phase this will be true for rows used for the public leaderboard; during the forecasting phase this will be true for rows used for the private leaderboard.

**sample_submission.csv**

* `id`
* `winner`

## Таймлайн проекта
* **29 ноября 2024**: Выбор соревнования для участия.
* **23 декабря 2024**: Дедлайн выбор соревнования.
* **16 января 2025**: Создание репозитория и начало работы.
* **20 января 2025**: Командный брейншторминг. ([Результаты](brainstorming.md))
* **02 февраля 2025**: Дедлайн отчёта по соревнованию. ([Отчёты](reports/))

* **TBA марта 2025**: Дедлайн защиты проекта. ([Отчёты](final_presentation/))
