# Customer Churn Prediction

Аналитический проект по прогнозированию оттока клиентов телеком-компании на публичном датасете IBM Telco Customer Churn.

## Что внутри

- `Churn_Prediction.ipynb` — оформленный ноутбук с EDA, моделированием, интерпретацией факторов оттока и бизнес-рекомендациями.
- `telco_customer_churn.csv` — исходный датасет.
- `requirements.txt` — минимальные зависимости для повторного запуска.

## Основные выводы

- Отток клиентов в датасете: около 26.5%.
- Самые рискованные сегменты: новые клиенты, month-to-month контракты, Fiber optic, Electronic check, отсутствие TechSupport и OnlineSecurity.
- Лучшая модель по ROC AUC: Gradient Boosting, ROC AUC около 0.846 на holdout-выборке.
- Для retention-сценария важен не только стандартный порог 0.5, но и отдельный бизнес-порог, который повышает recall и помогает находить больше клиентов с риском ухода.

## Как запустить

```bash
python3 -m pip install -r requirements.txt
jupyter notebook Churn_Prediction.ipynb
```

## Источник данных

Датасет известен как IBM Telco Customer Churn / `WA_Fn-UseC_-Telco-Customer-Churn.csv`.

