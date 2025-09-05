---
title: Sessões técnicas - Subdomínio do Adobe Campaign e gerenciamento de SSL no Painel de controle do Campaign
description: Saiba como delegar e configurar subdomínios no Painel de controle do Adobe Campaign, configurar certificados SSL e monitorar a configuração para garantir a capacidade de entrega segura de emails.
solution: Campaign
feature: Subdomains and Certificates
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3409
last-substantial-update: 2025-09-05T00:00:00Z
jira: KT-18866
source-git-commit: 18ce421793d97372198151afc92b24f3bed053a8
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Sessões técnicas: Subdomínio do Adobe Campaign e gerenciamento de SSL no Painel de controle do Campaign

Nesta sessão, exploramos os conceitos de delegação e configuração de subdomínio no Adobe Campaign, incluindo a instalação de certificados SSL para proteger subdomínios.

Saiba o que é um subdomínio, suas finalidades e os métodos de delegação que permitem que o Adobe o use com eficiência. A sessão também aborda os princípios de proteção de um subdomínio por meio de certificados SSL e as práticas recomendadas para manter um ambiente seguro.

Fornecemos orientação passo a passo sobre como configurar subdomínios usando o Painel de controle do Self-Service, destacando possíveis obstáculos e como resolvê-los. Os participantes obtêm conhecimento prático para garantir uma configuração perfeita e um gerenciamento seguro de seus subdomínios.

Seja você um administrador, desenvolvedor ou proprietário de plataforma, esta sessão oferece as habilidades para configurar e proteger subdomínios com confiança no Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3471391/?learn=on&enablevpops)

## Especialização em gerenciamento de subdomínio no Adobe Campaign

Desbloqueie os conceitos básicos de delegação, configuração e segurança de subdomínio para as comunicações por email do Adobe Campaign:

* **Delegação de subdomínio** Escolha entre delegação CNAME ou completa para controlar como o Adobe gerencia sua capacidade de entrega de DNS e email.
* **Configuração de DNS e SSL** A configuração adequada dos certificados MX, SPF, DKIM, DMARC e SSL é fundamental para o envio seguro e confiável de emails.
* **Painel de Controle** Use a ferramenta de autoatendimento da Adobe para simplificar a configuração de subdomínios, monitorar registros e gerenciar certificados SSL.
* **Armadilhas comuns** Evite atrasos e erros entendendo as linhas do tempo de auditoria, os requisitos de registro e as etapas de solução de problemas.

Dominar esses processos garante que suas campanhas estejam seguras, sejam entregues e mantenham a reputação da sua marca.

## Métodos de delegação** completos vs. CNAME

* A **Delegação completa** do Adobe gerencia todos os registros DNS para o subdomínio, garantindo uma capacidade de entrega e segurança ideais. Recomendado para a maioria dos usuários.
* **Delegação CNAME** O cliente e a Adobe compartilham responsabilidades de DNS. O cliente cria registros CNAME que apontam para recursos gerenciados pela Adobe.
* **Principais diferenças:
* **Total** o Adobe tem autoridade total; menos manutenção de clientes.
* **CNAME** Responsabilidade compartilhada; mais etapas manuais para o cliente.
* **Dica** Nunca delegue seu domínio raiz (somente subdomínios) para evitar perder o controle sobre seu domínio principal.
