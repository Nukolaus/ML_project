# Проект МЛ

## Файлы
* Ensemble.ipynb - ансамбль трех бустингов на дескрипторах, эмбедингах ChemBERTa-10M-MLM, числе символов в SMILES
* ml_project_01.ipynb - регрессия (CatboostRegressor, CatboostRegressor + ChemBert), классификация (CatBoostClassifier) и сохранение фото
* ml_project_02.ipynb - классификация по фото Resnet152
* ml_project_03.ipynb - регрессия (LightAutoML)

## Команда

* Александров Николай - БИВТ-21-17
* Мартынов Сергей - БИВТ-21-17

## Метрики
| Model                       | R2         | MSE (log IC50) |
| ----------------------------|------------|----------------|
| CatboostRegressor + BaseLine| 0.382      | 0.803          |
| CatboostRegressor + ChemBert| 0.339      | 0.858          |
| LightAutoML                 | 0.434      | 0.764          |
| CatboostRegressor + Ensemble| 0.370      | 1.269          |

Классификация на 4 класса показала плохие результаты 
* f1-macro 0.48 на табличных данных
* f1-macro 0.35 на картинках
  
Поэтому регрессия не проводилась
