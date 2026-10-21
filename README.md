# Gabriel de Assis

**Engenharia de dados e analytics engineering.** Venho de BI e inteligência comercial: passei anos do lado de quem consome o dado e sabe o custo de um número errado. Hoje construo o lado de baixo: ingestão, modelagem em camadas, regras de qualidade testáveis e pipelines que provam que funcionam.

O que guia meus projetos:

- **Qualidade medida, não declarada.** Se o pipeline diz que deduplica, o CI mostra precisão e recall contra um gabarito.
- **Regra de negócio fora do código.** Regras em YAML ou SQL documentado, para quem não programa conseguir ler e mudar.
- **Dado público só sintético ou aberto.** Nenhum projeto aqui usa dado de empresa.

## Projetos

### [Framework de Qualidade e Deduplicação de CRM](https://github.com/GabrAssis/framework-qualidade-crm)

Audita e deduplica o export de qualquer CRM: regras de qualidade em YAML, nota por campo e por registro, deduplicação com blocagem, similaridade e golden record, e um plano de merge revisável. Um gerador sintético cria uma base suja com defeitos conhecidos, e o CI mede precisão, recall e F1 da deduplicação contra esse gabarito.

Python · YAML · RapidFuzz · Jinja2 · pytest · GitHub Actions · GitHub Pages · **[relatório ao vivo →](https://gabrassis.github.io/framework-qualidade-crm/)**

### [Livraria Inteligente](https://github.com/GabrAssis/projeto-livraria-ia)

Pipeline em arquitetura medalhão sobre um catálogo coletado por scraping: bronze em JSONB com rastreio da ingestão, prata com tipagem e deduplicação determinística por função de janela, ouro com métricas por livro e categoria. Por cima, um agente que responde perguntas em português gerando SQL e mostra a consulta e o resultado.

Python · PostgreSQL · Supabase · SQL · BeautifulSoup · Streamlit · LLM

### [Assistente de Documentos com IA](https://github.com/GabrAssis/projeto-documentos-ia)

RAG sem banco de dados: ingestão de PDF, TXT e Markdown, chunking com sobreposição, embeddings multilíngues locais, busca por similaridade de cosseno e respostas que citam os trechos de origem. Inclui rotina de avaliação com perguntas de referência e um caso fora da base.

Python · Sentence Transformers · NumPy · Streamlit · LLM

### [Análise de vendas semanais](https://github.com/GabrAssis/projeto-analise-vendas-melhores-compras)

Projeto acadêmico: comparação de modelos de regressão para vendas semanais, com os resultados apresentados em Power BI.

Python · pandas · scikit-learn · XGBoost · Power BI

## Stack

- **Dados:** Python · SQL · PostgreSQL · pandas · modelagem em camadas (bronze/prata/ouro)
- **Qualidade e engenharia:** testes com pytest · CI no GitHub Actions · regras declarativas
- **Análise e BI:** Power BI · estatística aplicada · visualização para público não técnico
- **IA aplicada a dados:** RAG · text-to-SQL · embeddings

## Estudos

Anotações e exercícios da pós em Engenharia de Dados: [Pos-Engenharia-Dados](https://github.com/GabrAssis/Pos-Engenharia-Dados).
