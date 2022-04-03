<img src="https://storage.googleapis.com/golden-wind/experts-club/capa-github.svg" />

# Publicando uma aplicação react.js estática no Azure Blob Storage

Ao final teremos uma aplicação React.js estática publicada no Azure Storage de maneira profissional e atrás de uma CDN, custando centavos mensalmente. Apresentado por [Wilson Neto][1].

## Sobre este template
Este é o template "React Material UI Devias Kit", um template gratuito feito pela agência Devias, utilizado aqui apenas como exenplo de uma aplicação React.js totalmente estática (https://material-ui.com/store/items/devias-kit/).

## Instalação

1. Basta baixar usando <br />`git clone https://github.com/wilsonneto-dev/ExpertsClub_001_StaticAppToAzBlobStorage.git`
3. Basta executar <br />`npm start`

## Sobre a Aula

Nesta aula vou te mostrar o passso sobre como publicar suas aplicações SPAs/estáticas com o menor custo possível utilizando o Azure Blob Storage. Além de implmentarmos o fluxo completo e automatizado de continous deployment com Github Actions.

Atualmente com as aplicações SPAs e os frameworks modernos dominando o cenário do desenvolvimento frontent demanda cada vez maior é a necessidade de publicarmos aplicações 100% estáticas que irão consumir API que estarão em outros servidores. Já vi muitos projetos utilizando servidores PaaS, containers ou mesmo máquinas virtuais para hospedarem SPAs, que poderiam estar em hospedagens estáticas como Azure Blob Storage ou AWS S3, e a publicação destas aplicações sem ser em hospedagens estáticas acarreta em custos muito maiores e desnecessários.

## Link e informações de apoio

- Comando para criar o token AZURE_CREDENTIALS de permissionamento que utilizamos no Github Actions:<br />
Bast abrir o "Cloud Shell" e digitar: <br />`az ad sp create-for-rbac --name "GHActionsPipelineEC" --role contributor --scopes /subscriptions/<subscription uuid>/resourceGroups/<resource group name> --sdk-auth`<br /> 
(substitua o subscription id e o sresource group conforme fizemos no vídeo)

- Em caso de solicitação para registrar o serviço da CDN:<br />
Em algumas contas novas ao tentar criar uma CDN irá aparecer uma mensagem solicitando que verifique se o serviço de CDN está registrado em sua conta, para estes casos acessar o terminal "Cloud Shell" no próprio portal da Azure e digitar: <br />`Register-AzResourceProvider -ProviderNamespace Microsoft.Cdn`<br /> Assim o serviço de CDN será registrado em sua conta para que você possa criar recursos de CDN.

- Link Azure:<br />
https://portal.azure.com/

- Links tema utilizado no exemplo:<br />
https://material-ui.com/store/items/devias-kit/

## Expert

| [<img src="https://github.com/wilsonneto-dev.png" width="75px;"/>][1] |
| :-: |
|[Creator][1]|


[1]: https://seusite.com.br
