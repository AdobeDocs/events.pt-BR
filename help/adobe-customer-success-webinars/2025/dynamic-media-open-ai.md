---
title: Dominar o Dynamic Media com a API aberta
description: Entenda as principais diferenças entre o Dynamic Media tradicional e o modelo de API aberta e saiba como fazer a transição e implementar com êxito o Dynamic Media Ultimate com API aberta.
solution: Experience Manager as a Cloud Service, Experience Manager Assets
feature-set: Experience Manager Assets
feature: SDK/API
topic: Development, Content Management
role: Admin, Developer, User
level: Beginner, Intermediate
doc-type: Event
duration: 2757
last-substantial-update: 2025-08-08T00:00:00Z
jira: KT-18702
source-git-commit: ef1eacd73c5a4fb9cdfee730d40606ec65bab2a7
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---


# Dominar o Dynamic Media com a API aberta

Este webinário foi projetado para profissionais familiarizados com o Dynamic Media tradicional e que desejam entender e implementar o [Dynamic Media Ultimate](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dm-prime-ultimate) com API aberta.  Exploraremos o funcionamento de alto nível do Dynamic Media Ultimate com a API aberta e o compararemos com o Dynamic Media tradicional. Nosso objetivo é fornecer uma compreensão abrangente das diferenças entre essas duas abordagens, permitindo que os participantes familiarizados com o Dynamic Media se adaptem facilmente ao modelo de API aberta.

>[!VIDEO](https://video.tv.adobe.com/v/3470620/?learn=on&enablevpops)

## Principal comparação de recursos

| Recurso | Mídia dinâmica | Dynamic Media com OpenAPI |
|-----------------------------|------------------------|----------------------------|
| *Disponibilidade* | No local, AMS, Cloud | Somente nuvem |
| *Modificadores* | Conjunto avançado disponível | Limitado, mas em crescimento |
| *Controle de acesso* | Aberto a todos os usuários | Restrito por funções |
| *TTL DO CDN* | ~10 horas | ~10 minutos |
| *Imposição de Aprovação* | Publicado automaticamente | Requer aprovação |
| *Compatível com SEO* | Sim | Sim |

## Cenários de integração

Esses cenários de integração demonstram a flexibilidade e a escalabilidade do Dynamic Media com OpenAPI para diversas necessidades empresariais.

* **Integração do AEM Sites** O Dynamic Media com OpenAPI oferece suporte à integração perfeita com o AEM Sites, permitindo que os ativos sejam buscados diretamente da camada de entrega, sem duplicação.
* **CMS de Terceiros** Habilita a integração com plataformas como Salesforce e Drupal usando APIs ou aplicativos de micro front-end.
* O **Acesso Controlado por API** fornece APIs para pesquisa, recuperação e entrega de representações otimizadas de ativos.
* **Otimização da camada de entrega** O Assets é fornecido pelo Fastly, garantindo uma entrega mais rápida e eficiente.