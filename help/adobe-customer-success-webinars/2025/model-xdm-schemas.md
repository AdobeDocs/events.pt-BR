---
title: Práticas recomendadas e insights para modelagem de esquemas XDM
description: Modelagem de dados mestres no AEP com esquemas XDM, gerenciamento de identidade e práticas recomendadas para personalização e segmentação escaláveis e em tempo real.
topic: Personalization
role: Developer
level: Intermediate
doc-type: Event
duration: 3488
last-substantial-update: 2025-05-08T00:00:00Z
jira: KT-18019
source-git-commit: cfc7b54ae4360779ca2c41f88fc08089bae99165
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---


# Práticas recomendadas e insights para modelagem de esquemas XDM

Nesta sessão, conheça as práticas recomendadas e os atalhos essenciais para criar Adobe Experience Data Models (XDM) escaláveis e de alta qualidade que se alinhem aos padrões do Adobe Experience Platform. Obtenha insights sobre como mapear efetivamente a experiência do cliente e os dados de casos de uso para o XDM, para uma integração perfeita entre o Adobe e as ferramentas externas.

## Pontos de discussão

* Como definir e organizar componentes XDM para garantir modelos de dados escaláveis e flexíveis
* Desafios comuns em design, evolução e manutenção do XDM

>[!VIDEO](https://video.tv.adobe.com/v/3458042/?learn=on&enablevpops)

## Principais pontos

**Modelagem de Dados no Adobe Experience Platform (AEP)**

O esquema XDM é a base para a modelagem de dados no AEP, permitindo a integração e o compartilhamento de dados em diferentes sistemas. Ela define a estrutura e o significado dos dados, como atributos de perfil e ações baseadas em eventos.

**Identity Management**

O gerenciamento adequado de identidades é fundamental para evitar problemas como o colapso de perfis. Hash de dados confidenciais, como email e o uso de identificadores exclusivos, pode ajudar a manter a integridade dos dados. Os mapas de identidade são recomendados para segmentação e personalização em tempo real.

**Práticas recomendadas de design de esquema**

Mantenha os esquemas simples e focados em casos de uso de marketing. Evite sobrecarregar esquemas com atributos desnecessários. Use grupos de campos padronizados e minimize personalizações para escalabilidade e à prova de obsolescência.

**Evento vs. Atributos de Perfil**

Decida se os dados serão modelados como atributos de perfil ou eventos com base em objetivos de marketing. Os atributos do perfil são adequados para o direcionamento em tempo real, enquanto os eventos fornecem insights históricos para segmentação baseada em tempo.

**Manipulando Perfis e Escalabilidade Recolhidos**

Os perfis recolhidos só podem ser corrigidos pelo suporte da Adobe, mas as regras de gráfico de identidade podem impedir futuros recolhimentos. Para reestruturar esquemas existentes, é recomendado extrair os dados necessários e começar do zero com um esquema limpo.
