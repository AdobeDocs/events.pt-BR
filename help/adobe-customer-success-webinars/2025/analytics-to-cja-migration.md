---
title: Práticas recomendadas para migrar do Adobe Analytics para o Adobe Customer Journey Analytics
description: Saiba mais sobre as etapas essenciais e as práticas recomendadas para migrar do Adobe Analytics para o Customer Journey Analytics (CJA), incluindo o design de esquema XDM, o mapeamento de dados e a configuração da visualização de dados.
solution: Analytics, Customer Journey Analytics
topic: Migration
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 3654
last-substantial-update: 2025-07-16T00:00:00Z
jira: KT-18535
source-git-commit: 90eb4a9d2cf445c58fde776092fb047f820fa207
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Práticas recomendadas para migrar do Adobe Analytics para o Adobe Customer Journey Analytics

Saiba mais sobre a migração do Adobe Analytics para o Customer Journey Analytics (CJA). Apresentada por Nicolina Picone e Maurizio Corò da equipe do Ultimate Success da Adobe, a sessão fornece uma visão geral detalhada do CJA, seus recursos e práticas recomendadas para migração.

## Principais tópicos discutidos

* diferenças entre o Analytics e o CJA
* a importância de identificadores de identidade fortes, alinhamento de estruturas de dados e criação de visualizações de dados personalizáveis
* A aborda estratégias para importar dados históricos, gerenciar a atribuição de canais de marketing e aproveitar a flexibilidade do CJA para relatórios personalizados

>[!VIDEO](https://video.tv.adobe.com/v/3464911/?learn=on&enablevpops)

## Principais práticas

* **Visão geral do Customer Journey Analytics (CJA)** O CJA é uma evolução do Adobe Analytics, com foco na jornada completa do cliente em vários pontos de contato (por exemplo, dispositivos móveis, Web, CRM, call centers) em vez de eventos de rastreamento único. Ele permite o processamento e a manipulação de dados em tempo real.

* **Disponibilidade para migração** As principais etapas para migrar do Adobe Analytics para o CJA incluem garantir um identificador de identidade forte (por exemplo, ID de pessoa), alinhar variáveis e dimensões e mapear dados para o esquema XDM. Os dados históricos podem ser importados com etapas de validação.

* **Visualizações de Dados e Flexibilidade** O CJA permite a criação de visualizações de dados personalizáveis com durações de sessão ajustáveis, filtros de segmentação e configurações de atribuição. Essa flexibilidade permite relatórios e análises personalizados.

* **Práticas recomendadas para migração de dados históricos** Valide dados do CJA comparando-os com dados do Adobe Analytics dentro de um intervalo aceitável (por exemplo, 10% de diferença). Comece com uma janela de preenchimento retroativo curta (por exemplo, um mês) e aumente a escala gradualmente.

* **Atribuição de canal de marketing** A CJA oferece recursos aprimorados para atribuição de canal de marketing, eliminando limitações como a função de &quot;primeira página da visita&quot; e permitindo configurações de sessão mais dinâmicas.
