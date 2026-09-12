# Materiais encontrados - Confiabilidade e manutenção da transmissão

Catálogo pesquisado em 12/09/2026. Dados de distribuição podem apoiar protótipos, mas devem ser identificados como proxy quando o alvo for transmissão.

## 01 - Dados

- [SIGET - ANEEL](https://dadosabertos.aneel.gov.br/pt_BR/dataset/sistema-de-gestao-da-transmissao-siget): linhas, subestações, equipamentos, contratos, obras e termos; atualização diária informada pelo portal.
- [Catálogo de Dados Abertos ANEEL](https://dadosabertos.aneel.gov.br/dataset/?_tags_limit=0&organization=agencia-nacional-de-energia-eletrica): inclui interrupções de distribuição, SIGET e outros conjuntos úteis.
- [Carga de energia verificada - ONS](https://dados.ons.org.br/dataset/groups/carga-energia-verificada): contexto operacional para ocorrências.
- [BD Queimadas - INPE](https://terrabrasilis.dpi.inpe.br/queimadas/bdqueimadas/): focos e risco ambiental próximos a linhas e faixas de servidão.
- [Dados meteorológicos - INMET](https://bdmep.inmet.gov.br/): vento, precipitação e temperatura para modelos de risco.

## 02 - Documentos técnicos

- [Procedimentos de Rede - ONS](https://www.ons.org.br/paginas/sobre-o-ons/procedimentos-de-rede/vigentes): requisitos operacionais e responsabilidades.
- [RAP da perturbação de 15/08/2023 - ONS](https://www.ons.org.br/AcervoDigitalDocumentosEPublicacoes/RAP%202023.08.15%2008h30min%20vers%c3%a3o%20final%20com%20anexos%20de%20diverg%c3%aancia_Final.pdf): exemplo completo de investigação técnica.
- [PAR/PEL 2024 - ONS](https://www.ons.org.br/paginas/energia-no-futuro/suprimento-eletrico/parpel2024/sumario-executivo/index.html): reforços, desempenho dinâmico e planejamento.
- [ISO 55000 - Asset management](https://www.iso.org/standard/83053.html): referência para gestão de ativos.

## 03 - Artigos e pesquisa aplicada

- [Projeto TAESA de análise automática de ocorrências](https://institucional.taesa.com.br/pesquisa/projeto-0048metodologia-e-ferramenta-para-analise-automatica-de-ocorrencias-utilizando-algoritmos-de-aprendizado-de-maquina/): IA e oscilografias para localizar e classificar faltas.
- [Inspeção inteligente de linhas - TAESA](https://ventures.taesa.com.br/2013/04/03/inspecao-inteligente-de-linhas-com-sistemas-estaticos-e-moveis/): visão computacional e sensores.
- [Planejamento automatizado de faixas de servidão - TAESA](https://institucional.taesa.com.br/pesquisa/planejamento-automatizado-de-limpeza-de-faixas-de-servidao/): dados geoespaciais, queimadas, vegetação, erosão e invasões.

## 04 - Notícias e ocorrências

- [ONS publica RAP da ocorrência de agosto de 2023](https://www.ons.org.br/Paginas/Noticias/20231018_Ocorrencia_de_15_de_agosto_ONS_finaliza_Relatorio_de_Analise_de_Perturbacao_RAP.aspx): caso para estruturar causas, recomendações e responsáveis.
- [Plano de obras de transmissão 2025 - MME](https://www.gov.br/mme/pt-br/assuntos/noticias/mme-abre-consulta-publica-sobre-plano-que-define-novas-obras-da-transmissao-eletrica-para-os-proximos-anos): ampliações e reforços previstos.

## 05 - Casos e benchmarking

- [TAESA Ventures - manutenção preditiva](https://ventures.taesa.com.br/plataforma-de-manutencao-preditiva/): inventário digital, reconhecimento de componentes e priorização.
- [CIGRE](https://www.cigre.org/): publicações e grupos técnicos sobre transmissão e confiabilidade.
- [ENTSO-E Incident Classification Scale](https://www.entsoe.eu/publications/system-operations-reports/): referência europeia para classificação e relatórios de incidentes.

## Ideias de uso

Extrair de relatórios data, ativo, localização, modo de falha, causa, consequência, ação corretiva e recomendação. Combinar busca semântica com classificação de causa e um grafo de ocorrências semelhantes. Separar evidência observada de hipótese do modelo.
