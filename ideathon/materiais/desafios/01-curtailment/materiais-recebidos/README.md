# Materiais recebidos - Curtailment

Esta pasta contém os cinco arquivos Parquet entregues pela organização do Hackathon, obtidos da pasta pública **Dados - ONS** indicada no Caderno de Desafios e Dados.

## Arquivos baixados

| Arquivo | Conteúdo | Período informado no caderno | Registros |
|---|---|---:|---:|
| `constrained_off_eolica_tm.parquet` | Base principal eólica | 01/10/2023 a 31/08/2026 | 7.951.920 |
| `constrained_off_fotovoltaica_tm.parquet` | Base principal fotovoltaica | 01/04/2024 a 31/08/2026 | 2.854.800 |
| `constrained_off_eolica_fotovoltaica_tm.parquet` | Base principal integrada | 01/04/2024 a 31/08/2026 | 9.441.168 |
| `constrained_off_eolica_detail.parquet` | Detalhamento eólico | 01/01/2023 a 31/08/2026 | 63.429.221 |
| `constrained_off_fotovoltaica_detail.parquet` | Detalhamento fotovoltaico | 01/04/2024 a 31/08/2026 | 19.061.960 |

Local dos arquivos: `dados-ons/Dados - ONS/`.

## Origem

- [Pasta pública fornecida pelo Hackathon](https://drive.google.com/drive/folders/1nAHsGQ3S7IGXq3ZI1p7lTqk5dwT0Vg0a)
- [Base eólica oficial do ONS](https://dados.ons.org.br/dataset/restricao_coff_eolica_usi)
- [Base fotovoltaica oficial do ONS](https://dados.ons.org.br/dataset/restricao_coff_fotovoltaica)
- [FAQ de Curtailment do ONS](https://www.ons.org.br/Paginas/faq_curtailment.aspx)

## Cuidados de uso

O caderno informa intervalos de 30 minutos, valores nulos preservados e ausência de imputação ou remoção de outliers. Na base integrada, use `fonte` junto com `id_ons`, pois `id_ons` não é globalmente único entre eólica e fotovoltaica.
