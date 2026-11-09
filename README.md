# Лабораторная работа 1. Кто снизил активность и почему

Таболин Владислав Андреевич, вариант S30. Data Science Camp, «Теория DS».

| файл | что это |
|---|---|
| `01_analysis.ipynb` | рабочий ноутбук: загрузка сырых данных, аудит, чистка, журнал, исследование, группы |
| `02_report.ipynb` | отчёт для заказчика (читает результаты первого ноутбука) |
| `report.pdf` | собранный отчёт |
| `cleaning_log.csv` | журнал изменений данных |
| `campaign_list.csv` | итоговый список кампании: `client_id`, `group` |

Как воспроизвести (Python 3.12, [uv](https://docs.astral.sh/uv/)):

```bash
uv sync
uv run jupyter nbconvert --to notebook --execute --inplace 01_analysis.ipynb
uv run jupyter nbconvert --to webpdf --no-input --execute 02_report.ipynb --output report
```

Сырые файлы `clients.csv` и `transactions.csv` лежат в корне репозитория.
