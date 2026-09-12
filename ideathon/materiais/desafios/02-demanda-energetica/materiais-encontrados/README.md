# Materiais encontrados - Demanda energética

Catálogo pesquisado em 12/09/2026. Use as subpastas numeradas para downloads e notas locais.

## 01 - Dados

- [Carga de energia verificada - ONS](https://dados.ons.org.br/dataset/groups/carga-energia-verificada): séries oficiais para modelar carga por período e subsistema.
- [Dados de consumo - EPE](https://www.epe.gov.br/pt/publicacoes-dados-abertos/publicacoes/consumo-de-energia-eletrica): resenhas mensais e séries por classe e região.
- [Anuário Estatístico de Energia Elétrica 2026 - EPE](https://www.epe.gov.br/pt/imprensa/noticias/epe-publica-o-anuario-estatistico-de-energia-eletrica-2026-ano-base-2025-): consumo, demanda, carga, preços e tarifas.
- [BDMEP - INMET](https://bdmep.inmet.gov.br/): observações de estações meteorológicas brasileiras.
- [ERA5](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels): reanálise horária global desde 1940.
- [Calendário de feriados nacionais](https://www.gov.br/gestao/pt-br/assuntos/noticias/): criar variáveis de calendário; validar anualmente a portaria oficial.

## 02 - Documentos técnicos

- [Impactos das mudanças climáticas na demanda - EPE](https://www.epe.gov.br/sites-pt/publicacoes-dados-abertos/publicacoes/PublicacoesArquivos/publicacao-852/topico-736/Demanda%20e%20Mudan%C3%A7as%20Clim%C3%A1ticas.pdf): riscos climáticos e planejamento.
- [Previsão de carga para o planejamento anual - ONS/EPE/CCEE](https://www.ons.org.br/AcervoDigitalDocumentosEPublicacoes/Nota%20T%C3%A9cnica%20-%20Previs%C3%A3o%20de%20carga%20para%20o%20Planejamento%20Anual%20da%20Opera%C3%A7%C3%A3o%20Energ%C3%A9tica%20do%20SIN%20-%202024-2028.pdf): método e premissas institucionais.
- [PEN 2025 em notícia técnica - Agência Brasil](https://agenciabrasil.ebc.com.br/economia/noticia/2025-07/ons-brasil-precisara-de-termicas-e-da-volta-do-horario-de-verao): riscos no pico noturno e alternativas operacionais.

## 03 - Artigos e pesquisa

- [IEA - Electricity 2026](https://www.iea.org/reports/electricity-2026): tendências de demanda, eletrificação e flexibilidade.
- [Open Power System Data - Time series](https://data.open-power-system-data.org/time_series/): referência de organização e documentação de séries elétricas.

## 04 - Notícias

- [Consumo cresceu 3,7% em julho de 2026 - EPE](https://www.epe.gov.br/pt/imprensa/noticias/consumo-de-eletricidade-continua-a-crescer-em-julho-de-2026-residencias-e-comercio-lideram-alta): exemplo recente para testar explicações do modelo.
- [Fact sheet sobre clima e demanda - EPE](https://www.epe.gov.br/pt/imprensa/noticias/epe-publica-fact-sheet-sobre-impactos-das-mudancas-climaticas-na-demanda-de-energia-eletrica): contexto oficial.
- [Recorde de consumo durante onda de calor - CNN Brasil](https://www.cnnbrasil.com.br/economia/macroeconomia/calor-faz-demanda-por-energia-atingir-o-maior-patamar-da-historia-no-brasil/): evento extremo para estudo de caso.

## 05 - Casos e benchmarking

- [ENTSO-E Transparency Platform](https://transparency.entsoe.eu/): demanda e operação europeias.
- [Electricity Maps](https://www.electricitymaps.com/data-portal): referência de visualização e combinação de dados elétricos e carbono.

## Ideias de cruzamento

Modelar por subsistema e horizonte. Criar variáveis de hora, dia da semana, feriado, temperatura aparente, ondas de calor e tendência. Comparar um baseline simples com modelos de IA e medir erro especialmente nos picos.
