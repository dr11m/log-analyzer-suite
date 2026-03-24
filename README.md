# Log Analyzer Suite

[English version](README.en.md)

Монорепозиторий трёх инструментов для анализа логов с использованием AI: llm-log-analyzer — standalone Python-модуль с LLM API; log-insight — Claude Code skill с индуктивным анализом через параллельных агентов; log-validate — Claude Code skill с дедуктивной code-aware валидацией через grep.

## Проекты

| Проект | Описание |
|--------|----------|
| [log-insight](log-insight/) | Claude Code skill — AI-анализ логов через чанки и агентов |
| [log-validate](log-validate/) | Claude Code skill — code-aware валидация логов через grep |
| [llm-log-analyzer](llm-log-analyzer/) | Standalone Python-модуль для анализа логов через LLM |

## Краткое сравнение

| | log-insight | log-validate | llm-log-analyzer |
|---|-------------|--------------|------------------|
| Подход | Чанки + агенты | Code-aware grep | Standalone LLM |
| Знание кода | Да (при генерации контекста) | Да (карта логов) | Да |
| Покрытие файла | До 100% (зависит от числа чанков) | 100% | Ограничено контекстом |

## Использование

Каждый сабмодуль независим. Клонируйте с сабмодулями:

```bash
git clone --recursive <repo-url>
```

Или инициализируйте сабмодули отдельно:

```bash
git clone <repo-url>
git submodule update --init --recursive
```
