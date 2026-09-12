# Materiais do Ideathon

O caderno oficial contém seis desafios. Cada pasta separa três origens para evitar confusão:

1. `materiais-recebidos/`: arquivos entregues pela organização ou fontes explicitamente indicadas no caderno.
2. `materiais-encontrados/`: pesquisa externa realizada pela equipe, com catálogo comentado e data de consulta.
3. `resumo-do-desafio.md`: síntese do problema e pergunta orientadora.

## Materiais efetivamente anexados pela organização

- **Curtailment:** cinco bases Parquet tratadas do ONS, baixadas e documentadas.
- **Demanda energética:** PDF de acesso ao ERA5 e notebook de passo a passo, baixados e documentados.

Nos desafios 3 a 6, a pasta pública não trouxe bases anexas. Nesses casos, `materiais-recebidos/` registra apenas as categorias e instituições indicadas pelo caderno. O material localizado depois está em `materiais-encontrados/`.

## Estrutura da pesquisa externa

Cada desafio contém:

- `01-dados/`
- `02-documentos-tecnicos/`
- `03-artigos-e-pesquisa/`
- `04-noticias/`
- `05-casos-e-benchmarking/`

O `README.md` de cada desafio funciona como catálogo principal, com links, finalidade e sugestões de cruzamento.

## Arquivos grandes

Os arquivos `.parquet` e `.mp4` usam Git LFS, configurado em `.gitattributes`. Verifique a cota e o limite do repositório remoto antes do envio ao GitHub.
