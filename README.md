# boletim-am-assets

Assets públicos do **Boletim AM** (newsletter semanal da [Análise Macro](https://analisemacro.com.br)),
servidos via **GitHub Pages**. Aqui ficam apenas os arquivos *publicados* — o código do pipeline
permanece nos repositórios privados (`Boletim_AM`, `newsletters-digest`).

## Estrutura

```
digests/    # PDFs de resumo e aprofundamento por edição (resumo-AAAA-MM-DD.pdf, aprofundamento-...)
podcasts/   # mp3 do Audio Overview (NotebookLM) por edição (boletim-<N>.mp3)
index.html  # landing page com os materiais da edição corrente
```

## URLs públicas

Base: `https://vitorwilher.github.io/boletim-am-assets/`

- Resumo: `…/digests/resumo-AAAA-MM-DD.pdf`
- Aprofundamento: `…/digests/aprofundamento-AAAA-MM-DD-<slug>.pdf`
- Podcast: `…/podcasts/boletim-<N>.mp3`

## Como publicar uma edição

1. Copiar os PDFs da semana (de `newsletters-digest/digests/`) para `digests/`.
2. Baixar o Audio Overview do NotebookLM e salvar em `podcasts/boletim-<N>.mp3`.
3. Atualizar `index.html` com os links da edição.
4. `git add . && git commit && git push` — o GitHub Pages atualiza em ~1 min.

> Os links são embutidos no rodapé "📎 Material da semana" de cada edição do boletim
> (gerado por `scripts/generate_draft.py` no repo `Boletim_AM`).
