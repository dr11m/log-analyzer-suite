# Log Analyzer Suite

A monorepo of three log analysis tools exploring complementary approaches to AI-powered log analysis: llm-log-analyzer is a standalone Python module using LLM APIs; log-insight is a Claude Code skill using inductive analysis via parallel agents; log-validate is a Claude Code skill using deductive code-aware validation with full file coverage via grep.

## Projects

| Project | Description |
|---------|-------------|
| [log-insight](log-insight/) | Claude Code skill — AI log analysis via chunking and agents |
| [log-validate](log-validate/) | Claude Code skill — code-aware log validation via grep |
| [llm-log-analyzer](llm-log-analyzer/) | Standalone LLM-powered log analyzer module |

## Quick Reference

| | log-insight | log-validate | llm-log-analyzer |
|---|---|---|---|
| Approach | Chunks + agents | Code-aware grep | Standalone LLM |
| Code knowledge | No | Yes (logger map) | Yes |
| File coverage | 5-30% | 100% | Context-limited |

## Usage

Each subrepository is independent. Clone with submodules:

```bash
git clone --recursive <repo-url>
```

Or initialize submodules separately:

```bash
git clone <repo-url>
git submodule update --init --recursive
```
