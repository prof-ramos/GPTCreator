# 5. Testes & Métricas – GPT-XYZ

## 5.1 Casos de Teste
| ID | Descrição | Entrada | Saída Esperada | Status |
|----|-----------|---------|----------------|--------|
| T1 | Saudação  | "Oi"    | Cumprimento    | ✅     |

## 5.2 Métricas
- Precisão: 92 %
- Recall: 88 %
- Latência p95: 1.2 s

## 5.3 Avaliação Humana
- Escala 1-5 para relevância, tom, precisão
- 20 avaliadores, 100 amostras

## 5.4 Regressão
- CI/CD: GitHub Actions
- Job: `pytest tests/`
