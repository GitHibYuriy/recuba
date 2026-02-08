# recuba
Recuba is a desktop tool for regression modeling and optimization. It supports linear, logarithmic, and logistic models with strict domain validation (no data-distorting protections), automatic and custom term selection, and extremum search. Designed for engineering and scientific analysis.
Recuba — настольный инструмент для регрессионного моделирования и оптимизации.
Поддерживает линейные, логарифмические и логистические модели с жёсткой проверкой доменов (без искажения данных), auto/custom отбор термов и поиск экстремумов. Для инженерных и научных задач.
# Recuba (v20)
The core idea of Recuba is explicit separation of model spaces:
linear space (Y),
logarithmic space (log Y),
logistic space (logit Y),
with strict domain validation instead of data-distorting numerical “protections”.
Ключевая идея Recuba — жесткое разделение пространств моделирования:
линейное пространство (Y),
логарифмическое пространство (log Y),
логистическое пространство (logit Y),
с обязательной проверкой доменов, вместо искажающих данные численных «защит».
# Recuba supports:
linear regression (OLS),
models with logarithmic and logistic transformations,
automatic and manual (custom) term selection on a polynomial basis,
numerical optimization and extremum search in a specified factor domain.
The package is designed for engineering, scientific, and applied modeling tasks, where model correctness and interpretability are more important than blind metric optimization.
# Recuba поддерживает:
линейную регрессию (МНК),
модели с логарифмическими и логистическими преобразованиями,
автоматическую и ручную (custom) идентификацию термов на полиномиальном базисе,
численную оптимизацию и поиск экстремумов в заданной области факторов.
Пакет ориентирован на инженерные, научные и прикладные задачи, где корректность модели и интерпретируемость важнее формальной оптимизации метрик.
# Key Features 
- Linear regression (OLS) on polynomial basis with interaction terms.
- Logarithmic and logistic models with **strict domain validation**.
- Automatic and manual (custom) term selection.
- Consistent model space handling (linear / log / logit).
- Export of results and metrics to Excel.
- Numerical optimization and extremum search in factor space.
# Основные возможности
- Линейная регрессия (МНК) на полиномиальном базисе с взаимодействиями.
- Логарифмические и логистические модели с **жёсткой проверкой доменов**.
- Автоматический и ручной (custom) отбор термов.
- Строгое разделение пространств моделей (linear / log / logit).
- Экспорт результатов и метрик в Excel.
# Domain Rules (LOG / LOGIT)  
Recuba applies **strict domain rules** for transformed models.
If a domain condition is violated, the calculation is blocked and no data is modified.
- **LOG model** is allowed only if: `y > 0` for all used data points.
- **LOGIT model** is allowed only if: `0 < y < 1` for all used data points.
- No artificial clipping, shifting, or data correction is applied.
- Domain violations are detected during pre-analysis.
# Правила доменов (LOG / LOGIT)
Recuba использует **жёсткие правила доменов** для моделей с преобразованием отклика.
При нарушении домена расчёт блокируется, данные не искажаются.
- **LOG-модель** допускается только при условии: `y > 0` для всех используемых точек.
- **LOGIT-модель** допускается только при условии: `0 < y < 1` для всех используемых точек.
- Искусственное клиппирование или сдвиг данных не применяется.
- Нарушения домена выявляются на этапе предварительного анализа.
#  Quick Start
1. Download the release archive from **GitHub → Releases**.
2. Run `recuba_tk_app_v20.exe`.
3. Load your Excel file, select factors and responses, and start the calculation.
# Быстрый старт
1. Скачайте архив релиза в разделе **GitHub → Releases**.
2. Запустите `recuba_tk_app_v20.exe`.
3. Загрузите Excel-файл с данными, выберите факторы и отклики и запустите расчёт.
# Limitations
- LOG and LOGIT models require strict compliance with domain conditions.
- Extremely large ranges in exponential models may lead to numerical instability.
- The package is intended for structured experimental or simulation data.
# Ограничения
- Модели LOG и LOGIT требуют строгого соблюдения доменных условий.
- Слишком большие диапазоны в экспоненциальных моделях могут приводить к численной неустойчивости.
- Пакет ориентирован на структурированные экспериментальные или расчетные данные.
  
Author: **Yuriy Zarubin**  
License: **MIT**
