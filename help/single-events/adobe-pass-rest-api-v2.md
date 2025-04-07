---
title: Adobe Pass - nova API REST v2
description: Essa sessão se concentra na introdução da nova REST API v2 da Adobe e no guia aos usuários por meio de seu processo de migração.
role: Developer
level: Beginner, Intermediate, Experienced
doc-type: Technical Video
duration: 3230
last-substantial-update: 2025-04-07T00:00:00Z
jira: KT-17685
hidefromtoc: true
source-git-commit: 1082d67d49901e151115255b585799a5f57bda4a
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---


# Adobe Pass - nova API REST v2

Essa sessão se concentra na introdução da nova REST API v2 da Adobe e no guia aos usuários por meio de seu processo de migração.

>[!VIDEO](https://video.tv.adobe.com/v/3457461/?learn=on&enablevpops)

## Destaques principais

* **Visão geral e benefícios**

   * A REST API v2 foi projetada para autenticação moderna, flexível e escalável, atendendo a eventos de alta demanda e cenários de vários dispositivos.
   * Os principais aprimoramentos incluem criptografia aprimorada, consistência de sessão, SSO entre dispositivos e informações estendidas de erro para depuração mais rápida.

* **Etapas de migração**

   * Os usuários devem criar novos aplicativos registrados com escopos REST API v2.
   * As configurações existentes, como identificação de dispositivo e mapeamentos do MVPD, podem ser reutilizadas.
   * A migração envolve fases como registro, configuração, autenticação, pré-autorização e autorização.

* **Melhorias funcionais**

   * A API RESTful unificada substitui os SDKs vizinhos de acesso, simplificando a implementação entre plataformas.
   * Suporte para vários perfis de autenticação na mesma sessão e transições simples entre dispositivos.
   * Os fluxos de pré-autorização e autorização permanecem obrigatórios para o acesso ao conteúdo.

* **Linha do tempo**

   * A API REST v1 deixará de receber atualizações até dezembro de 2025 e será totalmente removida até o final de 2026.
   * Os usuários são incentivados a concluir a migração bem antes desses prazos.

* **Recursos e suporte**

   * A documentação, os manuais e as perguntas frequentes estão disponíveis na Adobe Experience League.
   * O Adobe oferece ambientes de sandbox, ingressos do Zendesk e reuniões de migração para suporte.

* **Destaques das Perguntas e Respostas**

   * A REST API v2 requer reautenticação, pois não é compatível com versões anteriores com v1.
   * A pré-autorização é para fins de interface do usuário, enquanto a autorização é necessária para tokens de mídia.
   * O SSO é compatível por meio de um novo token de serviço da Adobe.

