# 4. APIs & Integrações – GPT-XYZ

## 4.1 Credenciais
Armazenar em `.env`:
⚠️ **IMPORTANTE**: NUNCA comitar o arquivo `.env` no controle de versão para proteger suas chaves de API.

```
OPENAI_API_KEY=sk-...
GEMINI_API_KEY=...
```

## 4.2 Endpoints Utilizados
| Serviço | Endpoint | Descrição |
|---------|----------|-----------|
| OpenAI  | /v1/chat/completions | Geração de texto |
| Google  | /v1beta/models/gemini-pro | Fallback |

## 4.3 Rate Limits
| Provedor | RPM | TPM |
|----------|-----|-----|
| OpenAI   | 500 | 80 k |

## 4.4 Tratamento de Erros
- Retry com backoff exponencial
- Log estruturado (JSON)

## 4.5 Segurança
- TLS 1.2+
- Validação de entrada (regex, JSON Schema)
