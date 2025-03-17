---
title: Migração do Marketo para o Adobe Admin Console - (Pré-migração)
description: A Adobe está migrando o Marketo Engage para o Admin Console a fim de melhorar o gerenciamento de usuários. Saiba mais sobre os tipos de automigração e auto-migração, pré-requisitos, alterações pós-migração, práticas recomendadas, armadilhas comuns e suporte. Acesse a gravação da sessão no site do Adobe na Experience League.
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 2280
last-substantial-update: 2025-03-14T00:00:00Z
jira: KT-17483
exl-id: 9c3da83f-9e02-4a2e-9784-10213facf056
source-git-commit: 848fa8fee05b315361781059eabb3b19904c78c2
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Migração do Marketo para o Adobe Admin Console - Pré-migração

Junte-se a nós para uma migração perfeita do Marketo com especialistas da Adobe.

Antecipe-se à migração do Marketo com a Equipe de experiência e identidade do cliente da Adobe neste webinário informativo. Nós o guiaremos pelas principais etapas, práticas recomendadas e desafios comuns para garantir uma transição suave para a Adobe Admin Console.

O que você vai aprender,

* Um roteiro passo a passo para seu processo de pré-migração
* Práticas recomendadas para simplificar sua transição e evitar armadilhas
* Respostas de especialistas a preocupações comuns com a migração

Se você estiver apenas iniciando a migração ou se preparando para as etapas finais, esta sessão fornecerá o conhecimento e as ferramentas para navegar pelo processo com confiança. Não perca esta oportunidade para avançar e facilitar a migração do Marketo.

>[!VIDEO](https://video.tv.adobe.com/v/3449712/?learn=on&enablevpops)

## Principais pontos

### Finalidade da migração e visão geral

A Adobe está migrando o Marketo Engage para o Admin Console a fim de consolidar todos os produtos em um único hub para melhorar o gerenciamento e o acesso dos usuários.  O Admin Console servirá como hub central para gerenciar produtos, funções de usuário, permissões e acesso de suporte da Adobe. Os URLs para acessar o Marketo Engage serão alterados para a plataforma Experience Cloud da Adobe.

### Tipos de migração

* **Migração automática** Para organizações com menos de 75 usuários e sem configuração SSL. O Adobe lida com a migração.
* **Auto Migração** Para organizações com configuração SSL. Os administradores gerenciam o processo de migração usando o Console de migração.

### Pré-requisitos para migração

* Os administradores do sistema devem preencher o email de consentimento.
* O SSL deve ser configurado no Admin Console (não na instância do Marketo).

### Alterações pós-migração

* Os usuários farão logon usando o Adobe ID ou a Federated ID (SSL).
* As funções e permissões de administrador determinarão os níveis de acesso na Admin Console.

### Práticas recomendadas

* Verifique os emails do usuário e resolva as contas bloqueadas antes da migração.
* Verifique se as funções administrativas adequadas foram atribuídas.
* Desative os bloqueadores de anúncios ou use o modo incógnito para evitar problemas de logon.

### Armadilhas comuns

* Permissões de administrador incorretas podem limitar o acesso.
* As extensões do navegador e os bloqueadores de anúncios podem interferir no acesso.
* A lista de permissões de IP ainda não é compatível com o Admin Console, mas está sendo desenvolvida.

### Impacto na funcionalidade

* Emails automatizados, usuários da API e códigos do munchkin não serão afetados pela migração.
* A migração afeta principalmente a autenticação e o gerenciamento de usuários.

### Suporte

* Os usuários com problemas devem abrir um caso de suporte no Atendimento ao cliente da Adobe.
* Inclua a ID da organização IMS em casos de suporte para resolução mais rápida.
