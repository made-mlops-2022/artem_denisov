Инструкции по запуску

все скрипты тестировал запуская из папки ml_project

пайплайн по генерации данных

> python3 generate_pipeline.py --n-rows 100 --filepath data

генерирует случайные синтетические данные заданной длины

пайплайн по обучению данных
доступны две конфигурации

 > python3 train_pipeline.py --model-name lr

запускает обучение с моделью логистической регрессии

> python3 train_pipeline.py --model-name knn

запускает обучение с моделью К ближайших соседей

пайплайн predict
> python3 test_pipeline.py --metric accuracy

запускает пайплайн с обучение и выводом в логи метрики accuracy,
вторая доступная метрика f1 f1_score
предсказанные данные записываются в папку data