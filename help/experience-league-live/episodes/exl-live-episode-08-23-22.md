---
title: Pergunte aos especialistas - Extensões úteis em tags (Launch) para ajudar a sobrecarregar o SDK da Web
description: Você está pensando em migrar sua implementação para o novo SDK da Web do Adobe?  Vamos executar algumas de nossas extensões favoritas na biblioteca de tags do Adobe, que ajudarão você a elevar o nível da sua coleção de dados.
solution: Data Collection,Experience Platform
kt: 10528
thumbnail: 346610.jpeg
event-start-time: 2022-08-23 09:00-7
event-cta-url: null
event-guests: Rudi Shumpert,Jeff Chasin,Eric Matisoff
exl-id: 5ef987f4-37f5-473f-b9f2-1598b7e655ba
source-git-commit: 17070f55bae19ef0751a2c7c536af7758e31affc
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Pergunte aos especialistas: extensões úteis em tags (Launch) para ajudar a sobrecarregar o SDK da Web

Você está pensando em migrar sua implementação para o novo SDK da Web do Adobe?  Vamos executar algumas de nossas extensões favoritas na biblioteca de tags do Adobe, que ajudarão você a elevar o nível da sua coleção de dados.

>[!VIDEO](https://video.tv.adobe.com/v/346610/?quality=12&learn=on)

## Perguntas e comentários do programa

### Extensão do Assistente de elemento de dados do Evolytics

<br> 
**Pergunta:** Do ponto de vista da segurança de dados, o Evolytics é seguro para uso, pois é uma extensão de terceiros?

**Resposta:** Sim. Você pode revisar o código de extensão se desejar. Além disso, ele não salva a data e faz apenas uma transformação.

<br> 

**Pergunta:** Isso também captura o Adobe ECID?

**Resposta:** O ECID do Adobe não é capturado nessa extensão. Essa extensão se destina à criação de identificadores adicionais e anônimos (entre outras coisas).

**Resposta:** A Adobe ECID pode ser capturada de outras maneiras. Compartilharemos isso por meio das notas do ExL e do Twitter, já que não é possível compartilhar links no bate-papo aqui.

<br> 

**Pergunta:** A funcionalidade de hash oferece várias técnicas de hash como SHA-256 e fornece chaves públicas e privadas?

**Resposta:** Sim! SHA-256 é o padrão

<br> 

### Perguntas gerais e comentários:

<br> 

**Pergunta:** Em que clicamos para baixar os arquivos de origem das extensões? Isso está no &quot;menu de 3 pontos&quot;?

**Resposta:** Sim! Os 3 pontos e, em seguida, Baixar origem (na exibição do catálogo)

<br> 

**Comentário:** Uma das coisas que eu realmente gosto de usar com extensões é o aspecto de economia de tempo delas. Muitos deles fazem coisas que você *poderia* faça com algum código personalizado, mas com uma extensão, você não precisa gravar esse código.

**Responder:** Diretamente. E é repetível sem ter que recriar a roda a cada vez.

<br> 

**Pergunta:** Como os plug-ins do Analytics serão compatíveis ou substituídos por implementações do SDK da Web?

**Resposta:** Muitos plug-ins do Analytics são desnecessários hoje em dia, graças à maior flexibilidade das tags do Workspace e do Adobe. No entanto, aqueles que não estão, estão sendo migrados ativamente para uso pelo SDK da Web.

<br> 

**Pergunta:** Algum desenvolvimento no rastreamento do Activity Map usando o SDK da Web?

**Resposta:** Tenho o prazer de informar que o Activity Map está sendo ativamente trabalhado também para suporte no SDK da Web

<br> 

**Pergunta:** Poderíamos ter acesso à rede Adobe Edge para gerenciar eventos antes de transferi-los para os destinos finais? Entendo que também podemos fazer isso no Launch, mas no futuro também seria possível fazer isso no servidor?

**Resposta:** Sim! Isso é possível por meio do recurso de encaminhamento de eventos, que os clientes podem comprar por meio de qualquer um dos nossos produtos da Real-Time CDP (Real-Time CDP Connections, Prime ou Ultimate).

**Resposta:** As Conexões RTCDP (Encaminhamento de eventos) oferecem a capacidade de ter mais controle antes de enviá-las para destinos que não sejam da Adobe.

**Resposta:** Confira alguns de nossos outros vídeos ExL Live para saber mais sobre isso (como [este](exl-live-episode-06-23-22.md)).

<br> 

**Comentário:** Chamada rápida para uma de minhas extensões favoritas: há uma extensão de tabela de mapeamento em que você pode ler uma tabela para um elemento de dados que &quot;se esse valor for esse, defina-o dessa maneira&quot;.

**Responder:** A flexibilidade que eles proporcionam é impressionante. Além disso, observe que as empresas também podem criar suas próprias extensões privadas, se desejarem.

<br> 

**Pergunta:** Você mostrou os dados individuais do CRM, como cidade e clima, então onde estamos armazenando a resposta individual?

**Resposta:** As respostas são armazenadas em cada evento único que aciona uma regra em uma propriedade de encaminhamento de eventos e são usadas somente nesse evento específico.

<br> 

Prossiga a discussão sobre este tópico no [Discussão da comunidade do Experience League](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-platform/experience-league-live-post-session-discussion-useful-extensions/m-p/542620#M240).
<br> 

## Sessões Experience League LIVE adicionais desta série de coleta de dados

* [Pergunte aos especialistas - Noções básicas do SDK da Web](exl-live-episode-05-26-22.md)
* [Pergunte aos especialistas - RTCDP Connections](exl-live-episode-06-23-22.md)
* [Pergunte aos especialistas - Datastreams e preparação de dados](exl-live-episode-07-21-22.md)
