# Migration Issue Map

Identity mapping: destination started empty, so sequential creation preserved the exact original issue numbers 1:1.

| Old issue | New issue | Title | State | Comments |
|-----------|-----------|-------|-------|----------|
| EricRLeao1311/CapiWatt#1 | Hackathon-IA-2026/solucoes-grupo-15#1 | CapiWatt Lens — Caso 1 (Carolina): mapa de decisões | open | 0 |
| EricRLeao1311/CapiWatt#2 | Hackathon-IA-2026/solucoes-grupo-15#2 | Qual é o contrato da interface do serviço vetorial (indexar, buscar, agrupar versões) que isola o Bedrock do resto do backend? | closed | 1 |
| EricRLeao1311/CapiWatt#3 | Hackathon-IA-2026/solucoes-grupo-15#3 | Como uma família de versões de um documento é identificada e agrupada num único objeto, na ingestão e no resultado da busca? | closed | 1 |
| EricRLeao1311/CapiWatt#4 | Hackathon-IA-2026/solucoes-grupo-15#4 | Como as relações entre documentos são representadas (arestas, origem: metadado explícito vs. similaridade) e onde ficam armazenadas? | closed | 1 |
| EricRLeao1311/CapiWatt#5 | Hackathon-IA-2026/solucoes-grupo-15#5 | Como a interface expõe a exploração do grafo de relações e o objeto-documento com versões, a partir dos protótipos juridico_wallace? | closed | 1 |
| EricRLeao1311/CapiWatt#6 | Hackathon-IA-2026/solucoes-grupo-15#6 | O que dispara uma notificação (novo documento? mudança em processo acompanhado?) e o que ela contém na página inicial e no e-mail? | closed | 2 |
| EricRLeao1311/CapiWatt#7 | Hackathon-IA-2026/solucoes-grupo-15#7 | Como a entrega de notificações pelo port Mailer lida com frequência e deduplicação no ambiente do hackathon? | closed | 1 |
| EricRLeao1311/CapiWatt#8 | Hackathon-IA-2026/solucoes-grupo-15#8 | O que roda local e o que roda na AWS no primeiro ciclo, respeitando os serviços e permissões do hackathon? | closed | 3 |
| EricRLeao1311/CapiWatt#9 | Hackathon-IA-2026/solucoes-grupo-15#9 | Como corpus_version, model_version e ranking_version são registrados para reproduzir uma execução? | closed | 1 |
| EricRLeao1311/CapiWatt#10 | Hackathon-IA-2026/solucoes-grupo-15#10 | Quais tipos de documento compõem o caso 1 (autos de infração, processos SEI, decisões, normas correlatas) e quais metadados cada um precisa carregar? | closed | 2 |
| EricRLeao1311/CapiWatt#11 | Hackathon-IA-2026/solucoes-grupo-15#11 | Qual é o gabarito de priorização e como ele é usado para avaliar se os resultados mais relevantes aparecem no topo (métrica, tolerância; não é ranking exato)? | closed | 2 |
| EricRLeao1311/CapiWatt#12 | Hackathon-IA-2026/solucoes-grupo-15#12 | Qual é a pergunta/tarefa concreta do caso 1 e o que Carolina considera resposta útil e erro material? | closed | 1 |
| EricRLeao1311/CapiWatt#13 | Hackathon-IA-2026/solucoes-grupo-15#13 | Que estratégia de chunking e que modelo de embeddings do Bedrock se ajustam aos documentos do caso 1? | open | 3 |
| EricRLeao1311/CapiWatt#14 | Hackathon-IA-2026/solucoes-grupo-15#14 | Carolina entrega o caso 1: detalhamento, documentos e gabarito de priorização | closed | 2 |
| EricRLeao1311/CapiWatt#15 | Hackathon-IA-2026/solucoes-grupo-15#15 | O backend (F3) deve ser dono também do armazenamento documental, junto das arestas, para que grafo e leitura de documentos não atravessem HTTP, dado um corpus da ordem de 100 documentos? | closed | 1 |
| EricRLeao1311/CapiWatt#16 | Hackathon-IA-2026/solucoes-grupo-15#16 | TB1 (Carolina) — scaffold demo/fixtures local: frontend + backend + ai, sem corpus oficial | open | 0 |
| EricRLeao1311/CapiWatt#17 | Hackathon-IA-2026/solucoes-grupo-15#17 | TB1 demo — Ticket 1: Compose scaffold + health check cruzado | closed | 2 |
| EricRLeao1311/CapiWatt#18 | Hackathon-IA-2026/solucoes-grupo-15#18 | TB1 demo — Ticket 2: Ingestão de corpus fixture (famílias/versões declarativas) | closed | 2 |
| EricRLeao1311/CapiWatt#19 | Hackathon-IA-2026/solucoes-grupo-15#19 | TB1 demo — Ticket 3: Busca sobre resultados mapeados por fixture | closed | 2 |
| EricRLeao1311/CapiWatt#20 | Hackathon-IA-2026/solucoes-grupo-15#20 | TB1 demo — Ticket 4: Página de família/documento | closed | 2 |
| EricRLeao1311/CapiWatt#21 | Hackathon-IA-2026/solucoes-grupo-15#21 | TB1 demo — Ticket 5: Relações declarativas + endpoint de grafo + página do processo | closed | 2 |
| EricRLeao1311/CapiWatt#22 | Hackathon-IA-2026/solucoes-grupo-15#22 | TB1 demo — Ticket 6: Sugestões por fixture: fusão + similar_a (aceitar/rejeitar) [opcional] | open | 0 |
| EricRLeao1311/CapiWatt#23 | Hackathon-IA-2026/solucoes-grupo-15#23 | TB1 demo — Ticket 7: Feedback (👍/👎) | closed | 2 |
| EricRLeao1311/CapiWatt#24 | Hackathon-IA-2026/solucoes-grupo-15#24 | TB1 demo — Ticket 8: Notificações + prévia de e-mail (Mailer) + telemetria | closed | 3 |
| EricRLeao1311/CapiWatt#25 | Hackathon-IA-2026/solucoes-grupo-15#25 | TB1 demo — Ticket 9: Reprodutibilidade — replay determinístico de busca fixture registrada | closed | 2 |
| EricRLeao1311/CapiWatt#26 | Hackathon-IA-2026/solucoes-grupo-15#26 | TB1 demo — Redesign do frontend CapiWatt Lens para o protótipo | closed | 2 |
| EricRLeao1311/CapiWatt#27 | Hackathon-IA-2026/solucoes-grupo-15#27 | Qual é o contrato do parecer jurídico conclusivo de uma frase e como ele permanece verificável? | open | 0 |
| EricRLeao1311/CapiWatt#28 | Hackathon-IA-2026/solucoes-grupo-15#28 | Como a busca pagina resultados ordenados por relevância em lotes de 10 sem alterar a ordem entre páginas? | closed | 2 |
| EricRLeao1311/CapiWatt#29 | Hackathon-IA-2026/solucoes-grupo-15#29 | Preparar acesso AWS pessoal para testar o Titan Text Embeddings V2 | closed | 4 |
| EricRLeao1311/CapiWatt#30 | Hackathon-IA-2026/solucoes-grupo-15#30 | Frontend completo do CapiWatt Lens a partir do handoff visual | closed | 6 |
| EricRLeao1311/CapiWatt#31 | Hackathon-IA-2026/solucoes-grupo-15#31 | Aprimorar home inicial, personas e notificações do protótipo | closed | 1 |
| EricRLeao1311/CapiWatt#32 | Hackathon-IA-2026/solucoes-grupo-15#32 | Corrigir queda do backend no primeiro "docker compose up" (corrida com o Postgres) | closed | 0 |
| EricRLeao1311/CapiWatt#33 | Hackathon-IA-2026/solucoes-grupo-15#33 | Integração do produto moderno com o backend demo | open | 1 |
| EricRLeao1311/CapiWatt#34 | Hackathon-IA-2026/solucoes-grupo-15#34 | Integração demo — inicializar corpus automaticamente e expor seu estado | closed | 2 |
| EricRLeao1311/CapiWatt#35 | Hackathon-IA-2026/solucoes-grupo-15#35 | Integração demo — conectar busca, feedback e leitura documental ao produto moderno | closed | 2 |
| EricRLeao1311/CapiWatt#36 | Hackathon-IA-2026/solucoes-grupo-15#36 | Integração demo — conectar processos e relações ao produto moderno | closed | 2 |
| EricRLeao1311/CapiWatt#37 | Hackathon-IA-2026/solucoes-grupo-15#37 | Integração demo — conectar notificações e prévia de e-mail ao produto moderno | closed | 3 |
| EricRLeao1311/CapiWatt#38 | Hackathon-IA-2026/solucoes-grupo-15#38 | Demonstração — resetar interações sem apagar o corpus | closed | 2 |
| EricRLeao1311/CapiWatt#39 | Hackathon-IA-2026/solucoes-grupo-15#39 | Demonstração — publicar temporariamente por túnel HTTPS | open | 0 |
| EricRLeao1311/CapiWatt#40 | Hackathon-IA-2026/solucoes-grupo-15#40 | O que o TB1 demonstra se a recuperação vetorial real não destravar, dado que a geração já responde? | open | 0 |
| EricRLeao1311/CapiWatt#41 | Hackathon-IA-2026/solucoes-grupo-15#41 | Protótipo — baixador terminal de famílias documentais | closed | 2 |
| EricRLeao1311/CapiWatt#42 | Hackathon-IA-2026/solucoes-grupo-15#42 | Baixador — derivar famílias de fontes oficiais SEI/SICNET | closed | 2 |
| EricRLeao1311/CapiWatt#43 | Hackathon-IA-2026/solucoes-grupo-15#43 | Baixador — navegador assistido para SEI/SICNET e lote de 10 famílias | open | 0 |
| EricRLeao1311/CapiWatt#44 | Hackathon-IA-2026/solucoes-grupo-15#44 | Frontend: revisão de acessibilidade (WCAG 2.2) com skill accessibility-audit | open | 2 |
| EricRLeao1311/CapiWatt#45 | Hackathon-IA-2026/solucoes-grupo-15#45 | Baixador — modo família por processo e coleta assistida | closed | 2 |
| EricRLeao1311/CapiWatt#46 | Hackathon-IA-2026/solucoes-grupo-15#46 | Baixador — lote assistido por filtro | closed | 2 |
| EricRLeao1311/CapiWatt#47 | Hackathon-IA-2026/solucoes-grupo-15#47 | Baixador — melhorar wizard do lote assistido | closed | 2 |
| EricRLeao1311/CapiWatt#48 | Hackathon-IA-2026/solucoes-grupo-15#48 | Baixador — tratar arquivo de resultados ausente no lote assistido | closed | 2 |
| EricRLeao1311/CapiWatt#49 | Hackathon-IA-2026/solucoes-grupo-15#49 | Mapa — correções de acessibilidade WCAG 2.2 do frontend (#44) | open | 0 |
| EricRLeao1311/CapiWatt#50 | Hackathon-IA-2026/solucoes-grupo-15#50 | A11y — indicadores de foco visíveis e com contraste (SC 1.4.11, 2.4.7) | closed | 2 |
| EricRLeao1311/CapiWatt#51 | Hackathon-IA-2026/solucoes-grupo-15#51 | A11y — componente de diálogo modal com gerenciamento de foco; menu da conta e popover (SC 2.4.11, 4.1.2) | closed | 2 |
| EricRLeao1311/CapiWatt#52 | Hackathon-IA-2026/solucoes-grupo-15#52 | A11y — estados ARIA em abas, filtros, segmentados, nós do mapa e disclosure (SC 4.1.2) | closed | 2 |
| EricRLeao1311/CapiWatt#53 | Hackathon-IA-2026/solucoes-grupo-15#53 | A11y — tokens de texto secundário com contraste mínimo 4,5:1 (SC 1.4.3) | closed | 2 |
| EricRLeao1311/CapiWatt#54 | Hackathon-IA-2026/solucoes-grupo-15#54 | A11y — layout resistente a texto 200% e tabela semântica em Meus Processos (SC 1.4.4, 1.3.1) | closed | 2 |
| EricRLeao1311/CapiWatt#55 | Hackathon-IA-2026/solucoes-grupo-15#55 | A11y — polimento: rótulos visíveis, nomes únicos, erro por campo, anúncios duplicados (P2 da #44) | closed | 2 |
| EricRLeao1311/CapiWatt#56 | Hackathon-IA-2026/solucoes-grupo-15#56 | Baixador — automatizar lote SEI após CAPTCHA humano | open | 1 |
