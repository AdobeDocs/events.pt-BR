---
title: Otimização da entrega de conteúdo - Desbloqueando o poder dos serviços da Edge
description: O ATM Edge Delivery Services (EDS) aprimora os recursos do ATM com serviços de composição, ciclos rápidos de desenvolvimento e altas pontuações máximas, oferecendo suporte à criação baseada em documentos e no WYSIWYG, arquitetura sem servidor, criação rápida de sites e amplas opções de personalização.
solution: Experience Manager, Experience Manager as a Cloud Service
feature: Edge Delivery Services
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3589
last-substantial-update: 2024-12-06T00:00:00Z
jira: KT-16631
source-git-commit: 47ae42d06ed311e60ebce194e0683bb95e8e5b69
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---


# Otimização da entrega de conteúdo: explorar o potencial dos serviços da Edge

Nesta sessão, forneceremos uma visão geral do Edge Delivery Services (EDS) e sua arquitetura. Vamos analisar como a EDS se integra à criação baseada em documentos e à criação baseada em AEM por meio do Editor universal. Uma demonstração ao vivo mostrará a EDS em ação, seguida por recursos para exploração adicional e uma sessão de perguntas e respostas.

>[!VIDEO](https://video.tv.adobe.com/v/3440938/?learn=on&enablevpops)

## Principais pontos

### Introdução ao EDS

* A EDS é um conjunto de serviços de composição projetados para aprimorar as capacidades do ATM &#x200B;.
* O objetivo é fornecer experiências excepcionais que impulsionam o engajamento e as conversões com ciclos de desenvolvimento rápidos e uma pontuação mínima de 100%. &#x200B;

### Opções de criação

* A **Criação baseada em documentos** usa ferramentas familiares, como o Microsoft Word ou o Google Docs, para a criação de conteúdo, permitindo a criação rápida de conteúdo sem um treinamento extensivo. &#x200B;
* **Editor Universal** Fornece uma interface de WYSIWYG semelhante aos sites ATM tradicionais, permitindo a criação de conteúdo mais detalhado e visual. &#x200B;

### Arquitetura

* A EDS integra-se à estrutura Cloud Service Amazon. &#x200B;
* Ela é compatível com a implementação sem servidor e pode funcionar sem um autor tradicional ou instância de editor. &#x200B;
* É possível implementar dois níveis de armazenamento em cache: no nível da infraestrutura do cliente e no nível da EDS. &#x200B;

### Gerenciamento de conteúdo

* A criação baseada em documentos requer uma conta GitHub, o Google Drive ou o Microsoft SharePoint, um plug-in sidekick e uma ferramenta de sincronização de código. &#x200B;
* O EDS com criação IAM requer uma conta GitHub, uma licença IAM as a Cloud Service e uma ferramenta de sincronização de código.

### Desenvolvimento e implantação

* O processo de criação de um site com EDS é rápido, geralmente leva menos de um dia. &#x200B;
* O desenvolvimento local pode ser feito usando o comando aem up para criar uma versão local do site.
* As alterações podem ser enviadas às ramificações de recursos para teste antes de mesclar com a ramificação principal. &#x200B;

### Personalização e extensibilidade

* Componentes personalizados podem ser criados usando CSS e JavaScript simples. &#x200B;
* A arquitetura permite integrações de terceiros e fontes de criação personalizadas.

### Práticas recomendadas

* É recomendável usar JavaScript baunilha e CSS para manter altas pontuações de farol.
* Qualquer introdução a bibliotecas como o React deve ser cuidadosamente considerada e testada para evitar degradação de desempenho.

### Suporte e documentação

* Uma documentação abrangente está disponível para orientar os usuários durante o processo de configuração e personalização. &#x200B;
* Os usuários são incentivados a entrar em contato com o suporte do Adobe para resolver qualquer problema não resolvido. &#x200B;