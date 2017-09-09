No Zapier, você pode usar o WebHooks ou o Code

## Code

```js
fetch('$URL')
  .then(function(res) {
    return res.json();
  })
  .then(function(json) {
    callback(null, json);
  })
  .catch(callback);
  
```

## Webhooks



http://mapa.cultura.ce.gov.br/api/event/find?@select=id,createTimestamp,user.name,name,shortDescription,project,registrationInfo,telefonePublico,preco,site,facebook,twitter,instagram&@limit=100

http://mapa.cultura.ce.gov.br/api/event/find?

@select=id,createTimestamp,user.name,name,shortDescription,project,registrationInfo,telefonePublico,preco,site,facebook,twitter,instagram&@limit=100

# Entidades

## Evento

http://mapa.cultura.ce.gov.br/api/event/find?

### Descrição - http://mapa.cultura.ce.gov.br/api/event/describe

```json
{
"id": { 
        "isMetadata":false,
        "isEntityRelation":false,
        "required":true,
        "type":"integer",
        "length":null,
        "label":"Id"
      },
"_type":{"isMetadata":false,"isEntityRelation":false,"required":true,"type":"smallint","length":null,"label":"","@select":"type"},"name":{"isMetadata":false,"isEntityRelation":false,"required":true,"type":"string","length":255,"label":"Nome"},"shortDescription":{"isMetadata":false,"isEntityRelation":false,"required":true,"type":"text","length":null,"label":"Descri\u00e7\u00e3o Curta"},"longDescription":{"isMetadata":false,"isEntityRelation":false,"required":false,"type":"text","length":null,"label":"Descri\u00e7\u00e3o Longa"},"rules":{"isMetadata":false,"isEntityRelation":false,"required":false,"type":"text","length":null,"label":""},"createTimestamp":{"isMetadata":false,"isEntityRelation":false,"required":true,"type":"datetime","length":null,"label":"Data de Cria\u00e7\u00e3o"},"status":{"isMetadata":false,"isEntityRelation":false,"required":true,"type":"smallint","length":null,"label":"Status"},"updateTimestamp":{"isMetadata":false,"isEntityRelation":false,"required":false,"type":"datetime","length":null,"label":"Data de Atualiza\u00e7\u00e3o"},"occurrences":{"isMetadata":false,"isEntityRelation":true,"targetEntity":"EventOccurrence","isOwningSide":false,"label":""},"owner":{"isMetadata":false,"isEntityRelation":true,"targetEntity":"Agent","isOwningSide":true,"label":""},"project":{"isMetadata":false,"isEntityRelation":true,"targetEntity":"Project","isOwningSide":true,"label":""},"__metadata":{"isMetadata":false,"isEntityRelation":true,"targetEntity":"EventMeta","isOwningSide":false,"label":""},"__files":{"isMetadata":false,"isEntityRelation":true,"targetEntity":"EventFile","isOwningSide":false,"label":""},"__agentRelations":{"isMetadata":false,"isEntityRelation":true,"targetEntity":"EventAgentRelation","isOwningSide":false,"label":""},"__termRelations":{"isMetadata":false,"isEntityRelation":true,"targetEntity":"EventTermRelation","isOwningSide":false,"label":""},"__sealRelations":{"isMetadata":false,"isEntityRelation":true,"targetEntity":"EventSealRelation","isOwningSide":false,"label":""},"__permissionsCache":{"isMetadata":false,"isEntityRelation":true,"targetEntity":"EventPermissionCache","isOwningSide":false,"label":""},"subsite":{"isMetadata":false,"isEntityRelation":true,"targetEntity":"Subsite","isOwningSide":true,"label":""},"subTitle":{"required":false,"type":"text","length":null,"private":false,"label":"Sub-T\u00edtulo","isMetadata":true,"isEntityRelation":false},"registrationInfo":{"required":false,"type":"text","length":null,"private":false,"label":"Inscri\u00e7\u00f5es","isMetadata":true,"isEntityRelation":false},"classificacaoEtaria":{"required":true,"type":"select","length":null,"private":false,"options":{"Livre":"Livre","18 anos":"18 anos","16 anos":"16 anos","14 anos":"14 anos","12 anos":"12 anos","10 anos":"10 anos"},"optionsOrder":["Livre","18 anos","16 anos","14 anos","12 anos","10 anos"],"label":"Classifica\u00e7\u00e3o Et\u00e1ria","isMetadata":true,"isEntityRelation":false},"telefonePublico":{"required":false,"type":"string","length":null,"private":false,"label":"Mais Informa\u00e7\u00f5es","isMetadata":true,"isEntityRelation":false},"preco":{"required":false,"type":"string","length":null,"private":false,"label":"Pre\u00e7o","isMetadata":true,"isEntityRelation":false},"traducaoLibras":{"required":false,"type":"select","length":null,"private":false,"options":{"":"N\u00e3o Informado","Sim":"Sim","N\u00e3o":"N\u00e3o"},"optionsOrder":["","Sim","N\u00e3o"],"label":"Tradu\u00e7\u00e3o para LIBRAS","isMetadata":true,"isEntityRelation":false},"descricaoSonora":{"required":false,"type":"select","length":null,"private":false,"options":{"":"N\u00e3o Informado","Sim":"Sim","N\u00e3o":"N\u00e3o"},"optionsOrder":["","Sim","N\u00e3o"],"label":"\u00c1udio descri\u00e7\u00e3o","isMetadata":true,"isEntityRelation":false},"site":{"required":false,"type":"string","length":null,"private":false,"label":"Site","isMetadata":true,"isEntityRelation":false},"facebook":{"required":false,"type":"string","length":null,"private":false,"label":"Facebook","isMetadata":true,"isEntityRelation":false},"twitter":{"required":false,"type":"string","length":null,"private":false,"label":"Twitter","isMetadata":true,"isEntityRelation":false},"googleplus":{"required":false,"type":"string","length":null,"private":false,"label":"Google+","isMetadata":true,"isEntityRelation":false},"instagram":{"required":false,"type":"string","length":null,"private":false,"label":"Instagram","isMetadata":true,"isEntityRelation":false}}

```
