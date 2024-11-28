---
title: Blueprint de migração do Assets
description: Saiba como migrar um DAM herdado para o Adobe Experience Manager Assets com insights de Achim Koch, que abrangem análise das partes interessadas, planejamento de recursos, transformação de dados e práticas recomendadas como usar arquivos CSV para manipulação de dados.
feature: Migration
topic: Migration
solution: Experience Manager, Experience Manager Assets
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1690
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16576
exl-id: f588055b-05c7-44df-be67-799a0e3ee1ed
source-git-commit: 946d7cd484e8c5d4358d4099b3518705cab8d4a3
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Blueprint de migração do Assets

Junte-se a Achim Koch, arquiteto técnico principal da Adobe, para saber como migrar um DAM herdado para o Adobe Experience Manager Assets. Obtenha insights sobre a análise das partes interessadas, o planejamento de recursos, a transformação de dados e as práticas recomendadas, como o uso de arquivos CSV para o manuseio de dados. Crie um roteiro para seus próprios projetos de migração do Adobe Experience Manager.

>[!VIDEO](https://video.tv.adobe.com/v/3440403/?learn=on&enablevpops)

## Discussão da comunidade

Continue a conversa na [discussão](https://adobe.ly/4hKHpnF) da Comunidade do Adobe Developers Live.

## Principais pontos

* **Nenhuma ferramenta pronta para uso para migração** Não há uma única ferramenta que possa migrar de vários sistemas herdados para o Adobe Experience Manager (AEM) devido à diversidade de produtos e soluções personalizadas.

* **Cinco estágios de migração**

   * Planejamento do Projeto
   * Planejamento de implementação
   * Implementação do AEM
   * Implementação do script de migração
   * Execução de migração

* **Envolvimento das partes interessadas** É fundamental identificar e envolver partes interessadas, como patrocinadores, usuários empresariais, administradores de sistemas de TI e suporte a sistemas herdados.

* **Planejamento de Recursos e Linha do Tempo** Verifique se os recursos estão disponíveis e planeje feriados, horários de pico e janelas fora do limite.

* **Planejamento técnico** Inclui análise de requisitos, transformação de dados e planejamento de infraestrutura.

* A Migração de **Processo Iterativo** envolve várias iterações de execução, análise, feedback e adaptação de scripts.

* **Uso de arquivos CSV** Os arquivos CSV são preferidos por sua facilidade de uso e legibilidade durante o processo de migração.

* A **Linguagem de Script** do Node.js é recomendada por seu suporte a CSV, AWS e HTTP e por ser uma boa oportunidade de aprender JavaScript.

* **Qualidade e repetibilidade** Garanta uma migração de dados de alta qualidade, mantenha os dados originais e arquivos CSV para referência e torne o processo repetível.

* **Congelamento de conteúdo** Declare um congelamento de conteúdo durante a migração para impedir que novos dados sejam adicionados depois que o instantâneo for tirado.

* **Ferramentas e dicas** Use ferramentas como o VS Code com a extensão Rainbow CSV e considere o marcador de ordem de bytes (BOM) para arquivos de texto UTF-8.

* **Aprovação da empresa** Reserve tempo para testar e obter aprovação oficial da empresa após a migração para levantar o congelamento do conteúdo.
