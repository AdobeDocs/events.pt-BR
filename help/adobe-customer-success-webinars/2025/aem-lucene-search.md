---
title: Dicas essenciais e práticas recomendadas para a pesquisa AEM Lucene
description: Aumente o engajamento digital com ferramentas avançadas de pesquisa do AEM, como filtros, facetas, sugestão automática, NGram e verificação ortográfica. Aprenda com demonstrações do mundo real.
solution: Experience Manager
feature: Search
role: Admin, Developer
level: Intermediate, Experienced
doc-type: Event
duration: 3630
last-substantial-update: 2025-11-13T00:00:00Z
jira: KT-19550
source-git-commit: 84c9a126769fa94b0197d12ca594137e13edc510
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---


# Dicas essenciais e práticas recomendadas para a pesquisa AEM Lucene

Descubra como melhorar sua presença digital e o envolvimento do cliente com recursos de pesquisa de última geração, incluindo filtros, facetas, sugestão automática, NGram e verificação ortográfica. Aprenda com demonstrações do mundo real e obtenha insights sobre como otimizar seus recursos de pesquisa com o AEM e o Lucene. Este webinário oferece a oportunidade de elevar sua experiência de pesquisa e manter-se à frente no cenário digital.

>[!VIDEO](https://video.tv.adobe.com/v/3476410/?learn=on&enablevpops)

## Desbloquear pesquisas poderosas no Adobe Experience Manager

O Adobe Experience Manager (AEM) aproveita a pesquisa do Lucene para fornecer resultados rápidos e relevantes em conteúdo, ativos e metadados. Esta sessão explora como os índices Lucene funcionam, como configurá-los e as práticas recomendadas para maximizar o desempenho da pesquisa.

* **A Pesquisa do Lucene está em todos os lugares** O Powers pesquisa no autor, editor e portais do AEM, gerenciando sugestões automáticas, filtros, aspectos e paginação.
* **Desempenho da Unidade das Definições de Índice** A personalização das definições de índice do Oak é fundamental para uma pesquisa direcionada eficiente.
* **As Práticas Recomendadas Importam**. Copie as definições de índice existentes, limite as propriedades indexadas e use os sinalizadores corretos para pesquisas de texto completo e de propriedades.
* **Recursos avançados Aprimorar facetas UX**, sugestão automática, verificação ortográfica, otimização e lematização podem ser habilitados para experiências de pesquisa mais avançadas.

A compreensão desses princípios ajuda a garantir recursos de pesquisa estáveis e de alto valor no AEM, oferecendo suporte a metas técnicas e de negócios.

## Blocos de construção do índice Lucene

As definições de índice AEM Lucene são a base do desempenho e da precisão da pesquisa. Os principais componentes incluem:

* **Tipo** Especifica o tipo de índice (Lucene, propriedade, etc.).
* **Restrição de Tipo de Nó** Segmenta tipos de conteúdo específicos (por exemplo, dam:Asset, cq:Page).
* **Restrição de Caminho** Limita a indexação a caminhos de repositório definidos para eficiência.
* **Regras de Agregação** Controla a profundidade e o escopo do conteúdo indexado, garantindo que as propriedades relevantes sejam pesquisáveis.
* **Regras de índice** Configuração principal; define sinalizadores como nodeScopeIndex (pesquisa ampla de texto completo) e analisado (geração de tokens/normalização).

A configuração cuidadosa desses elementos garante que as consultas de pesquisa sejam rápidas, relevantes e eficientes em recursos.

## Otimizando o desempenho da pesquisa

A otimização eficaz da pesquisa no AEM Lucene envolve a configuração estratégica e a adesão às práticas recomendadas:

* **Iniciar com Índices Existentes** Sempre copiar e modificar definições predefinidas, nunca criar do zero.
* **Limitar Propriedades Indexadas** Inclua apenas as propriedades necessárias para manter os índices enxutos e com desempenho.
* **Use sinalizadores sabiamente:
   * **nodeScopeIndex** true para pesquisa ampla de texto completo
   * **analyse** true para geração de tokens em nível de propriedade
   * **evaluatePathRestriction** true para consultas baseadas em caminho
* **Indexação de propriedade** A restrição de preferência de propriedade procura o melhor desempenho; use somente texto completo quando necessário.
* **Classificação e facetas** Habilite propertyIndex e a ordem de classificação; defina facet** como verdadeiro para filtragem baseada em contagem.

A aplicação dessas estratégias resulta em consultas mais rápidas, uso reduzido de recursos e resultados mais relevantes.

