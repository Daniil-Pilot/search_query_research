# Query NLP Pipeline

[![Python 3.10+](https://img.shields.io/badge/python-3.10%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HuggingFace](https://img.shields.io/badge/🤗-Datasets-orange.svg)](https://huggingface.co/datasets/nyuuzyou/wb-products)

Гибридный NLP-пайплайн для извлечения структурированных атрибутов из поисковых запросов маркетплейса Wildberries. Решение разработано в рамках тестового задания.

## Ключевые результаты


| Метрика | Значение | Интерпретация |
|---------|----------|---------------|
| **Accuracy** | 66.7% | Доля верных предсказаний |
| **Precision** | **80.4%** | Модель редко галлюцинирует |
| **Recall** | 66.7% | Модель осторожничает на сложных кейсах |
| **F1-score** | 72.3% | Баланс precision/recall |

## Архитектура

Трехуровневый гибридный пайплайн, сочетающий скорость rule-based подходов с гибкостью ML:



### Установка

#### 1. Клонировать репозиторий

```bash
git clone https://github.com/Daniil-Pilot/search_query_research.git
cd search_query_research
```

#### 2. Создать виртуальное окружение

**Linux / macOS:**
```bash
python -m venv venv
source venv/bin/activate
```

**Windows (PowerShell):**
```powershell
python -m venv venv
venv\Scripts\Activate.ps1
```

**Windows (cmd):**
```cmd
python -m venv venv
venv\Scripts\activate.bat
```

#### 3. Установить зависимости

```bash
pip install --upgrade pip
pip install -r requirements.txt
```
