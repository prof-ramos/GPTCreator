# GPT CREATOR

Repositório centralizado para organizar, versionar e documentar todos os meus projetos de agentes de IA (GPTs, Gemini Gens, Claude Projects, Espaços no Perplexity, etc.).  
Apesar do nome “GPT Creator”, o repositório é agnóstico em relação ao fornecedor: qualquer assistente, chatbot ou agente pode ser armazenado aqui.

---

## 📁 Estrutura de Diretórios

Cada agente possui seu próprio diretório, seguindo o padrão:

```
GPT-XYZ/
├── 1_contexto_index.md        # Visão geral, objetivos e escopo
├── 2_prompts.md             # Prompts de sistema, exemplos de diálogo
├── 3_modelos_padroes.md       # Arquitetura, fluxos, decisões de design
├── 4_apis.md                 # Integrações, endpoints, chaves
├── 5_testes.md               # Casos de teste, métricas, validação
├── 6_exemplos.md             # Conversas reais, saídas geradas
└── 7_referencias.md          # Links, papers, documentação externa
```

> Substitua `XYZ` por um identificador curto e sem espaços (ex.: `GPT-FinTax`, `Gemini-Tradutor`, `Claude-Contratos`).

---

## 🚀 Criando um novo agente

Use o snippet abaixo para gerar a estrutura completa:

```bash
AGENTE="GPT-XYZ"  # Altere para o nome do seu agente
mkdir -p "$AGENTE" && \
touch "$AGENTE"/{1_contexto_index.md,2_prompts.md,3_modelos_padroes.md,4_apis.md,5_testes.md,6_exemplos.md,7_referencias.md}
```

---

## 🧩 Templates

Para facilitar, copie os arquivos da pasta `templates/` para o novo diretório:

```bash
cp templates/* "$AGENTE"/
```

> Os templates já vêm com cabeçalhos e checklists preenchidos — basta adaptar.

---

## 📊 Status dos Projetos

| Agente | Status | Última Atualização | Responsável |
|--------|--------|--------------------|-------------|
| GPT-FinTax | ✅ Produção | 2025-07-23 | Gabriel Ramos |
| Gemini-Tradutor | 🧪 Testes | 2025-07-20 | Gabriel Ramos |
| Claude-Contratos | 🚧 Em construção | 2025-07-22 | Gabriel Ramos |

---

## 🛠️ Boas Práticas

1. **Commits semânticos**: `feat(gpt-xyz): adiciona novo prompt de saudação`.  
2. **Branches por funcionalidade**: `feat/gpt-xyz-ajuste-prompts`.  
3. **Revisão de prompts**: sempre teste variações antes de subir para `main`.  
4. **Documentação viva**: atualize `1_contexto_index.md` sempre que o escopo mudar.  
5. **Segurança**: nunca commite chaves de API; use `.env` e `.gitignore`.

---

## 📚 Recursos Úteis

- [OpenAI Cookbook](https://github.com/openai/openai-cookbook)  
- [Google Gemini Docs](https://ai.google.dev/gemini-api/docs)  
- [Anthropic Claude Prompt Engineering](https://docs.anthropic.com/en/docs/prompt-engineering)  
- [Perplexity Spaces](https://docs.perplexity.ai/guides/spaces)

---

## 🤝 Contribuindo

1. Faça um fork.  
2. Crie um branch (`feat/meu-agente`).  
3. Submeta um PR com descrição clara e prints de testes.

---

## 📄 Licença

MIT © Gabriel Ramos, 2025.