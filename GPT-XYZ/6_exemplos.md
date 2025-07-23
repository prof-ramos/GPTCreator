# 6. Exemplos de Conversa – GPT-XYZ

## 6.1 Exemplo 1 – Consulta Simples
**Usuário:** Como funciona o parcelamento de ICMS?  
**Assistente:** O parcelamento pode ser feito em até 60 meses…

## 6.2 Exemplo 2 – Multiturno
```
Usuário: Preciso abrir uma empresa.
Assistente: Qual o ramo?
Usuário: Tecnologia.
Assistente: ...
```

## 6.3 Exemplo 3 – JSON Mode
**Prompt:** Retorne um JSON com CNPJ e regime tributário.  
**Saída:**
```json
{"cnpj": "12.345.678/0001-00", "regime": "Simples Nacional"}
```

## 6.4 Exemplo 4 – Falha e Recuperação
Mostra como o agente lida com ambiguidade.
