# ДЗ-2 · Распознавание именованных сущностей

Дообучение [RuBERT-tiny2](https://huggingface.co/cointegrated/rubert-tiny2) для русского NER на [WikiNEuRal](https://huggingface.co/datasets/Babelscape/wikineural). Модель выделяет сущности типов PER, ORG, LOC и MISC.

- [Ноутбук](hw2_nlp.ipynb) содержит код, ответы и выводы полного запуска.
- [Метрики](artifacts/metrics.json) и [отчёт](artifacts/final_report.md) содержат результаты и анализ ошибок.
- Micro-F1 по сущностям на test — **0,8210**, macro-F1 — **0,7784**. На validation micro-F1 модели — **0,8169**, словарного бейзлайна — **0,4677**.

Для воспроизведения откройте ноутбук в Google Colab, выберите GPU T4, положите `artifacts/revisions.json` в `/content/revisions.json` и выполните все ячейки с `FAST_MODE=False`. Зависимости, данные и модели загружаются из ноутбука.

Дополнительные эксперименты 6.2–6.5 выполнены. Для 6.1 требуется отдельная ручная разметка.
