# Проект МЛ

## Файлы
* Ensemble.ipynb - ансамбль трех бустингов на дескрипторах, эмбедингах ChemBERTa-10M-MLM, числе символов в SMILES
* ml_project_01.ipynb - регрессия (CatboostRegressor, CatboostRegressor + ChemBert), классификация (CatBoostClassifier) и сохранение фото
* ml_project_02.ipynb - классификация по фото Resnet152

## Команда

* Александров Николай - БИВТ-21-17
* Мартынов Сергей - БИВТ-21-17

## Метрики
| Model                       | R2         | MSE (log IC50) |
| ----------------------------|------------|----------------|
| CatboostRegressor + BaseLine| 0.382      | 0.803          |
| CatboostRegressor + ChemBert| 0.339      | 0.858          |
| LIghtAutoML                 | -          | -              |
