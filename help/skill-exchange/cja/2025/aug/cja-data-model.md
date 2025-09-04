---
title: A arquitetura da análise - como abordar seu modelo de dados do Customer Journey Analytics
description: Saiba como estruturar modelos de dados do CJA com hierarquias de eventos, atribuição e KPIs para desbloquear insights mais profundos da jornada do cliente.
feature: Attribution
role: User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 0
last-substantial-update: 2025-09-04T00:00:00Z
jira: KT-18813
source-git-commit: 124b52203b98a80dd9202dab1b0dbe575475a52b
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# A arquitetura da análise: como abordar seu modelo de dados do Customer Journey Analytics

Um aspecto crucial da criação de um modelo de dados do CJA é entender a relação hierárquica entre diferentes pontos de contato e interações. Isso forma a base para análises e insights significativos.

As principais considerações incluem:

* Identificação e mapeamento de pontos de interação do cliente em todos os canais
* Estabelecer hierarquias e relacionamentos claros com eventos
* Definição de modelos de atribuição consistentes
* Criação de métricas e KPIs padronizados

Ao estruturar adequadamente esses elementos, as organizações podem rastrear e analisar melhor a jornada completa do cliente, resultando em insights mais acionáveis e melhores recursos de tomada de decisão.

>[!VIDEO](https://video.tv.adobe.com/v/3471111/?learn=on&enablevpops)

## Desbloquear a modelagem de dados para análises poderosas

Descubra como a arquitetura de dados eficiente no Adobe Experience Platform (AEP) e no Customer Journey Analytics (CJA) impulsiona insights e relatórios acionáveis.

* **Questões de Design de Esquema** A escolha entre esquemas simples, matrizes e matrizes de objetos afeta diretamente os recursos de análise e a flexibilidade de relatórios.
* **Processo de transformação** Os dados assimilados na AEP devem ser estruturados cuidadosamente para garantir transformação e usabilidade perfeitas no CJA.
* **Hierarquia do Contêiner** Entender os níveis de evento, sessão e pessoa é fundamental para a análise de vários níveis e para a geração de relatórios precisos.
* **Estratégias práticas** O planejamento antecipado, a governança de esquemas e o aproveitamento dos recursos da plataforma são fundamentais para implementações escaláveis e que não se tornem obsoletas.

Dominar esses conceitos permite que as equipes otimizem seus fluxos de trabalho de análise e desbloqueiem insights de negócios mais profundos.

## Tipos de esquema e seus casos de uso

* **Esquemas Simples** Melhores para relações de dados simples, um para um. Ideal para rastreamento básico de eventos e métricas/dimensões simples.
* **Matrizes** úteis para listas de itens relacionados (por exemplo, categorias de produtos, marcas de conteúdo). Cada elemento de matriz se torna uma dimensão individual para análise.
* **Matrizes de objetos** Projetadas para casos de uso complexos, como compras de produtos, em que cada objeto mantém suas próprias propriedades e relações. Permite a análise detalhada em nível de objeto.
* **Escolhendo de maneira inteligente** Selecione o esquema mais simples que atenda às suas necessidades, mas utilize matrizes e objetos para cenários avançados que exigem preservação de relacionamento.