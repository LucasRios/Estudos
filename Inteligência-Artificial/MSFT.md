# **Definir inteligência artificial**

IA como um software que exibe uma ou mais capacidades parecidas com as de humanos, conforme mostrado na tabela a seguir

![]()

![]()

## **Ciência de dados**

A ciência de dados é uma disciplina que se concentra no processamento e na análise de dados, aplicar técnicas estatísticas para descobrir e visualizar relações e padrões nos dados e definir _modelos_ experimentais que ajudam a explorar esses padrões.

## **Aprendizado de máquina**

Machine Learning é um subconjunto de ciência de dados que lida com o treinamento e a validação de modelos de _previsão_. Normalmente, um cientista de dados prepara os dados e, em seguida, usa-os para treinar um modelo com base em um algoritmo que explora as relações entre os _recursos_ nos dados para prever valores para _rótulos_ desconhecidos.

## **Inteligência artificial**

A inteligência artificial geralmente (mas nem sempre) se baseia no aprendizado de máquina para criar um software que emula uma ou mais características da inteligência humana.

## **Treinamento de modelo e inferência**

O processo de treinamento analisa os dados e determina as relações entre os _recursos_ nos dados (os valores de dados que geralmente estarão presentes em novas observações) e o _rótulo_ (o valor que o modelo está sendo treinado para prever).

Depois que o modelo tiver sido treinado, você poderá enviar novos dados que incluem valores de _recursos_ conhecidos e fazer com que o modelo preveja o _rótulo_ mais provável. O uso do modelo para fazer previsões é conhecido como _inferência_.

## **Pontuações de probabilidade e confiança**

Na maioria dos casos, as previsões têm uma _pontuação de confiança_ associada que reflete a probabilidade em que a previsão está sendo feita. Os desenvolvedores de software devem usar valores de pontuação de confiança para avaliar previsões e aplicar limites apropriados para otimizar a confiabilidade do aplicativo e reduzir o risco de previsões, que podem ser feitas com base em probabilidades marginais.

# **Considerações para a IA responsável**

## Imparcialidade, Confiabilidade e segurança, Privacidade e segurança, Inclusão, Transparência, Responsabilidade

# **Entender as funcionalidades do Azure Machine Learning**

![]()

Azure Machine Learning

*   Ingerir e preparar dados.
*   Executar experimentos para explorar dados e treinar modelos de previsão.
*   Implantar e gerenciar modelos treinados como serviços Web.

# **as funcionalidades dos serviços de IA do Azure**

**serviços de IA do Azure** são serviços baseados em nuvem que encapsulam recursos de IA. Em vez de um único produto, você deve pensar nos serviços de IA do Azure como um conjunto de serviços individuais que você pode usar como blocos de construção para compor aplicativos sofisticados e inteligentes.

![]()

# **funcionalidades do Serviço OpenAI do Azure**

modelos de IA que _geram_ conteúdo. O conteúdo que esses modelos geram pode ser na forma de texto, imagens, código ou mais, e de uma forma que quase pareça interagir com uma pessoa real em uma conversa real. Os modelos de IA generativa dependem de _modelos de linguagem grandes_ (LLMs) baseados na arquitetura de transformadores que evoluiu após anos de progresso do aprendizado de máquina.

# **funcionalidades do Azure Cognitive Search**

A **Pesquisa de IA do Azure** é um Serviço de IA Aplicada que permite ingerir e indexar dados de várias fontes e pesquisar o índice para encontrar, filtrar e classificar informações extraídas dos dados de origem.

Além da indexação básica baseada em texto, a Pesquisa de IA do Azure possibilita que você defina um _pipeline de enriquecimento_ que emprega habilidades de IA para aprimorar o índice com insights derivados dos dados de origem, por exemplo, usando a pesquisa visual computacional e os recursos de processamento de linguagem natural, é possível gerar descrições de imagens, extrair textos de documentos digitalizados e determinar frases-chave em documentos grandes que encapsulam seus pontos-chave.

Os serviços de IA do Azure incluem:

*   **IA do Azure para Informação de Documentos**: uma solução de reconhecimento óptico de caracteres (OCR) que pode extrair um significado semântico de formulários, como faturas, recibos e outros.
*   **Leitura Avançada de IA do Azure**: uma solução de leitura que atende a pessoas de todas as idades e níveis de habilidade.
*   **Azure Cognitive Search**: uma solução de pesquisa em escala de nuvem que usa serviços de IA para extrair insights de dados e documentos.
*   **OpenAI do Azure**: um Serviço Cognitivo do Azure que fornece acesso aos recursos do GPT-4 da OpenAI.

## **Opções para recursos do Azure**

### **Recurso de vários serviços**

Você pode provisionar um recurso dos **serviços de IA** que dá suporte a vários serviços de IA diferentes.

### **Recurso de serviço único**

Cada serviço de IA pode ser provisionado individualmente

## **Recursos de treinamento e previsão**

Embora a maioria dos serviços de IA possam ser usados por meio de um único recurso do Azure, alguns oferecem (ou requerem) recursos separados para o _treinamento_ e a _previsão_ do modelo

# **Identificar pontos de extremidade e chaves**

Para consumir o serviço por meio do ponto de extremidade, os aplicativos exigem as seguintes informações:

*   **O URI do ponto de extremidade**. Esse é o endereço HTTP no qual a interface REST do serviço pode ser acessada. A maioria dos kits de desenvolvimento de software (SDKs) dos serviços de IA usam o URI do ponto de extremidade para iniciar uma conexão com o ponto de extremidade.
*   **Uma chave de assinatura**. O acesso ao ponto de extremidade é restrito com base em uma chave de assinatura. Os aplicativos cliente devem fornecer uma chave válida para consumir o serviço. Quando você provisiona um recurso de serviços de IA, são criadas duas chaves, e os aplicativos podem utilizar qualquer uma delas. Você também pode regenerar as chaves conforme necessário para controlar o acesso ao recurso.
*   **A localização do recurso**. Ao provisionar um recurso no Azure, você geralmente o atribui a um local, que determina o data center do Azure no qual o recurso é definido. Embora a maioria dos SDKs use o URI do ponto de extremidade para se conectar ao serviço, alguns exigem o local.

# **Considerar a autenticação**

## **Regenerar chaves**

Você deve regenerar as chaves regularmente para proteger contra o risco de que elas sejam compartilhadas ou acessadas por usuários não autorizados. Você pode regenerar chaves usando o portal do Azure ou usando o comando da CLI (interface de linha de comando) do Azure az cognitiveservices account keys regenerate.

## **Proteger chaves com o Azure Key Vault**

O Azure Key Vault é um serviço do Azure no qual você pode armazenar segredos com segurança (como senhas e chaves). O acesso ao cofre de chaves é concedido a _entidades de segurança_, as quais você pode considerar identidades de usuário autenticadas usando o Microsoft Entra ID. Os administradores podem atribuir uma entidade de segurança a um aplicativo (nesse caso, ele é conhecido como uma _entidade de serviço_) a fim de definir uma _identidade gerenciada_ para o aplicativo. O aplicativo pode usar essa identidade para acessar o cofre de chaves e recuperar um segredo ao qual ele tem acesso. Controlar o acesso ao segredo dessa forma minimiza o risco de que ele seja comprometido por ser embutido em código em um aplicativo ou salvo em um arquivo de configuração.

Você pode armazenar as chaves de assinatura para um recurso dos serviços de IA do no Azure Key Vault e atribuir uma identidade gerenciada aos aplicativos cliente que precisam usar o serviço. Os aplicativos podem então recuperar a chave conforme necessário no cofre de chaves, sem o risco de expô-la a usuários não autorizados.

![]()

## **Autenticação baseada em token**

Ao usar a interface REST, alguns serviços de IA dão suporte (ou até mesmo _exigem_) a autenticação baseada em token. Nesses casos, a chave de assinatura é apresentada em uma solicitação inicial para obter um token de autenticação, que tem um período válido de dez minutos. As solicitações subsequentes devem apresentar o token para validar que o chamador foi autenticado.

## **Autenticação do Microsoft Entra ID**

Os serviços de IA do Azure dão suporte à autenticação do Microsoft Entra ID, permitindo que você conceda acesso a entidades de serviço específicas ou identidades gerenciadas para aplicativos e serviços em execução no Azure.

### **Autenticação por meio de entidades de serviço**

#### **Criar um subdomínio personalizado**

Você pode criar um subdomínio personalizado de diferentes maneiras, como por meio do portal do Azure, da CLI do Azure ou do PowerShell.

Por exemplo, você pode criar um subdomínio usando o PowerShell no Azure Cloud Shell. Para fazer isso, selecione sua assinatura usando o seguinte comando:

Set-AzContext -SubscriptionName <Your-Subscription-Name>

Em seguida, crie o recurso de serviços de IA do Azure especificando um subdomínio personalizado executando o seguinte:

$account = New-AzCognitiveServicesAccount -ResourceGroupName <your-resource-group-name> -name <your-account-name> -Type <your-account-type> -SkuName <your-sku-type> -Location <your-region> -CustomSubdomainName <your-unique-subdomain-name>

Depois de criado, o nome do subdomínio será retornado na resposta.

#### **Atribuir uma função a uma entidade de serviço**

Você criou um recurso de IA do Azure vinculado a um subdomínio personalizado. Em seguida, atribua uma função a uma entidade de serviço.

Para começar, você precisará registrar um aplicativo. Para isso, execute o comando a seguir:

$SecureStringPassword = ConvertTo-SecureString -String <your-password> -AsPlainText -Force
$app = New-AzureADApplication -DisplayName <your-app-display-name> -IdentifierUris <your-app-uris> -PasswordCredentials $SecureStringPassword

Isso cria o recurso do aplicativo.

Em seguida, use o comando **New-AzADServicePrincipal** para criar uma entidade de serviço e fornecer a ID do aplicativo:

New-AzADServicePrincipal -ApplicationId <app-id>

Por fim, atribua a função **Usuários dos Serviços Cognitivos** à entidade de serviço executando:

New-AzRoleAssignment -ObjectId <your-service-principal-object-id> -Scope <account-id> -RoleDefinitionName "Cognitive Services User"

### **Autenticar usando identidades gerenciadas**

As identidades gerenciadas estão disponíveis em dois tipos:

*   **Identidade gerenciada atribuída pelo sistema**: Uma identidade gerenciada é criada e vinculada a um recurso específico, como uma máquina virtual que precisa acessar os serviços de IA do Azure. Quando o recurso é excluído, a identidade também é excluída.
*   **Identidade gerenciada atribuída pelo usuário**: A identidade gerenciada é criada para ser utilizável por vários recursos em vez de ser vinculada a um. Ela existe independentemente de qualquer recurso único.

# **Implementar segurança de rede**

## **Aplicar restrições de acesso à rede**

Por padrão, os serviços de IA do Azure podem ser acessados de todas as redes. Alguns recursos individuais dos serviços de IA do Azure (como o **serviço de Detecção Facial de IA do Azure**, **Visão de IA do Azure** e outros) podem ser configurados para restringir o acesso a endereços de rede específicos - endereços de Internet públicos ou endereços em redes virtuais.

# **Métricas de exibição**

No caso dos Serviços de IA do Azure, o Azure Monitor coleta métricas relacionadas a solicitações de ponto de extremidade, dados enviados e retornados, erros e outras medições úteis.

## **Criar recursos para o armazenamento de log de diagnóstico**

Para capturar logs de diagnóstico para um recurso dos serviços de IA do Azure, você precisa de um destino para os dados de log. Você pode usar os Hubs de Eventos do Azure como um destino para encaminhar os dados para uma solução de telemetria personalizada e pode se conectar diretamente a algumas soluções de terceiros; mas, na maioria dos casos, você usará um (ou ambos) dos seguintes tipos de recurso em sua assinatura do Azure:

*   **Azure Log Analytics** – Um serviço que permite consultar e visualizar dados de log no portal do Azure.
*   **Armazenamento do Azure** – um armazenamento de dados baseado em nuvem que você pode usar para armazenar arquivos de log (que podem ser exportados para análise em outras ferramentas, conforme necessário).

Você deve criar esses recursos antes de configurar o log de diagnósticos para o recurso dos serviços de IA do Azure. Se você pretende arquivar dados de log no Armazenamento do Microsoft Azure, crie a conta do Armazenamento do Microsoft Azure na mesma região que seu recurso dos serviços de IA do Azure.

## **Entender contêineres**

Os contêineres possibilitam hospedar serviços de IA do Azure localmente ou no Azure. Por exemplo, se o seu aplicativo usa dados confidenciais em um SQL Server local para chamar um serviço dos serviços de IA do Azure, você pode implantar os serviços de IA do Azure em contêineres na mesma rede. Agora, seus dados podem permanecer em sua rede local, sem que sejam transmitidos para a nuvem. A implantação dos serviços de IA do Azure em um contêiner local também diminuirá a latência entre o serviço e os dados locais, o que pode aprimorar o desempenho.

## **O que é um contêiner?**

Um contêiner consiste em um aplicativo ou serviço e nos componentes de runtime necessários para executá-lo, ao mesmo tempo que abstrai o sistema operacional subjacente e o hardware. Na prática, essa abstração resulta em dois benefícios significativos:

*   Os contêineres são portáveis entre hosts, que podem estar executando sistemas operacionais diferentes ou usar hardware diferente – tornando mais fácil mover um aplicativo e todas as suas dependências.
*   Um único host de contêiner pode dar suporte a vários contêineres isolados, cada um com sua própria configuração de runtime específica – facilitando a consolidação de vários aplicativos com diferentes requisitos de configuração.

Um contêiner é encapsulado em uma _imagem de contêiner_ que define o software e a configuração a que ele deve dar suporte. As imagens podem ser armazenadas em um registro central, como o _Docker Hub_, ou você pode manter um conjunto de imagens em seu próprio registro.

Para usar um contêiner, você normalmente extrai a imagem de contêiner de um registro e a implanta em um host do contêiner, especificando quaisquer definições de configuração necessárias. O host do contêiner pode estar na nuvem, em uma rede privada ou em seu computador local. Por exemplo:

*   Um servidor do _Docker_\*.
*   Uma ACI (Instância de Contêiner do Azure).
*   Um cluster do AKS (Serviço de Kubernetes do Azure).

# **Usar contêineres dos serviços de IA do Azure**

## **Imagens de contêiner dos serviços de IA do Azure**

Cada contêiner fornece um subconjunto de funcionalidades dos serviços de IA do Azure. Por exemplo, nem todos os recursos do serviço de Linguagem de IA do Azure estão em um único contêiner. Detecção de idioma, tradução e análise de sentimentos são imagens de contêiner separadas. No entanto, as etapas de configuração são semelhantes para cada contêiner.

![]()

![]()

![]()

![]()

# **Visão geral da moderação de texto**

Ao usar a moderação de conteúdo assistida por computador, você bloqueia, aprova ou examina o conteúdo com base nas políticas e nos limites. Use a assistência de computador para aumentar a moderação humana de ambientes em que parceiros, funcionários e consumidores geram conteúdo de texto. Esses locais incluem:

*   Salas de chat
*   Quadros de discussão
*   Chatbots
*   Catálogos de comércio eletrônico
*   Documentos

A resposta da API de Moderação de Texto inclui as seguintes informações:

*   Uma lista de palavras potencialmente indesejadas encontradas no texto.
*   Quais tipos de palavras potencialmente indesejadas foram encontrados.
*   Possíveis dados pessoais encontrados no texto.

## **Conteúdo ofensivo**

Quando você passa o texto para a API, os termos potencialmente ofensivos no texto são identificados e retornados em uma resposta JSON. O item ofensivo é retornado como um Term na resposta JSON, junto com um valor de índice mostrando a localização do termo no texto fornecido.

Você também pode usar listas de termos personalizados com essa API. Nesse caso, se um termo ofensivo é identificado no texto, um ListId também é retornado para identificar a lista de termos personalizada que foi usada. A combinação do ListID e do Term identifica a palavra personalizada específica que foi encontrada. Uma resposta JSON de exemplo é mostrada aqui:

"Terms": \[

{

"Index": 118,

"OriginalIndex": 118,

"ListId": 0,

"Term": "crap"

}

## **Classificação**

Esse recurso da API pode colocar o texto em categorias específicas com base nas seguintes especificações:

Quando a resposta JSON é retornada, ela fornece um valor booliano para uma revisão recomendada do texto. Se ela for true, você deverá examinar o conteúdo manualmente para determinar o potencial de algum problema.

Cada categoria também é retornada com uma pontuação entre 0 e 1 para indicar a categoria prevista para o texto avaliado. Quanto maior a pontuação, mais provável é que a categoria possa ser aplicável. Esta é uma resposta JSON de exemplo:

"Classification": {

"ReviewRecommended": true,

"Category1": {

"Score": 0.99756889843889822

},

"Category2": {

"Score": 0.12747249007225037

},

"Category3": {

"Score": 0.98799997568130493

}

}

## **Dados pessoais**

Os dados pessoais são de importância crítica em muitos aplicativos. Esse recurso da API pode ajudar você a detectar se algum valor no texto pode ser considerado um dado pessoal antes de torná-lo público.

"PII": {

"Email": \[{

"Detected": "abcdef@abcd.com",

"SubType": "Regular",

"Text": "abcdef@abcd.com",

"Index": 32

}\],

"IPA": \[{

"SubType": "IPV4",

"Text": "255.255.255.255",

"Index": 72

}\],

"Phone": \[{

"CountryCode": "US",

"Text": "5557789887",

"Index": 56

}, {

"CountryCode": "UK",

"Text": "+44 123 456 7890",

"Index": 208

}\],

"Address": \[{

"Text": "1 Microsoft Way, Redmond, WA 98052",

"Index": 89

}\],

"SSN": \[{

"Text": "999-99-9999",

"Index": 267

}\]

}

# **Provisionar um recurso da Visão de IA do Azure**

![]()Os recursos visuais disponíveis estão contidos na enumeração VisualFeatures:

*   VisualFeatures.Tags: Identifica marcas sobre a imagem, incluindo objetos, cenário, configuração e ações
*   VisualFeatures.Objects: Retorna a caixa delimitadora para cada objeto detectado
*   VisualFeatures.Caption: Gera uma legenda da imagem em linguagem natural
*   VisualFeatures.DenseCaptions: Gera legendas mais detalhadas para os objetos detectados
*   VisualFeatures.People: Retorna a caixa delimitadora para pessoas detectadas
*   VisualFeatures.SmartCrops: Retorna a caixa delimitadora da taxa de proporção especificada para a área de interesse
*   VisualFeatures.Read: Extrai texto legível

A resposta JSON para análise de imagem é semelhante a este exemplo, dependendo dos recursos solicitados:

{

"apim-request-id": "abcde-1234-5678-9012-f1g2h3i4j5k6",

"modelVersion": "<version>",

"denseCaptionsResult": {

"values": \[

{

"text": "a house in the woods",

"confidence": 0.7055229544639587,

"boundingBox": {

"x": 0,

"y": 0,

"w": 640,

"h": 640

}

},

{

"text": "a trailer with a door and windows",

"confidence": 0.6675070524215698,

"boundingBox": {

"x": 214,

"y": 434,

"w": 154,

"h": 108

}

}

\]

},

"metadata": {

"width": 640,

"height": 640

}

}

## **Classificação de imagens**

Os modelos podem ser treinados para classificação multiclasse (em que há várias classes, mas cada imagem pode pertencer a apenas uma classe) ou classificação multirrótulo (em que uma imagem pode ser associada a vários rótulos).

## **Componentes de um projeto de Visão personalizada**

O primeiro componente de um projeto personalizado é o _conjunto de dados_. Esse conjunto é a sua coleção de imagens para treinar o modelo, junto com o _arquivo COCO_ que define as informações dos rótulos dessas imagens. Seu conjunto de dados fica armazenado em um contêiner de armazenamento de blobs do Azure, e vamos falar mais sobre o arquivo COCO nesta unidade.

Depois de definir suas imagens e rótulos de classe, você poderá treinar seu modelo personalizado. Durante o treinamento, você escolhe o tipo de modelo a treinar, qual conjunto de dados usar e seu orçamento para o treinamento (em quantidade de tempo). Quando o treinamento do modelo terminar, você poderá verificar o desempenho e usar o modelo para fazer previsões.

Na maioria dos casos, você vai seguir estas etapas:

1.  Criar seu contêiner de armazenamento de blobs e carregar apenas as imagens de treinamento.
2.  Criar o conjunto de dados para seu projeto e conectá-lo ao contêiner de armazenamento de blobs. Ao criar seu conjunto de dados, você define o tipo de projeto: classificação de imagem, detecção de objetos ou reconhecimento de produto.
3.  Rotular os dados em seu Projeto de Rotulagem de Dados do Azure Machine Learning, o que gera o arquivo COCO no contêiner de armazenamento de blobs.
4.  Conectar o arquivo COCO concluído das imagens rotuladas ao seu conjunto de dados.
5.  Treinar seu modelo personalizado no conjunto de dados e rótulos criados.
6.  Verificar o desempenho e iterar caso o desempenho treinado não atenda às expectativas.

Uma vez que o desempenho atender às expectativas, o modelo pode ser utilizado no Vision Studio ou em seu próprio aplicativo.

### **Arquivos COCO**

Um arquivo COCO é um arquivo JSON com um formato específico que define:

*   **imagens**: define o local da imagem no armazenamento de blobs, nome, largura, altura e ID.
*   **anotações**: define as classificações (ou objetos), incluindo em qual categoria a imagem está classificada, a área e a caixa delimitadora (se estiver rotulando para detecção de objetos).
*   **categorias**: define a ID da classe de rótulo nomeada.

Normalmente, os arquivos COCO são criados ao rotular suas imagens de treinamento em um Projeto de Rotulagem de Dados do Azure Machine Learning.

{

"images": \[

{

"id": 1,

"width": 1024,

"height": 768,

"file\_name": "abc.jpg",

"coco\_url": "AmlDatastore://fruit/abc.jpg",

"absolute\_url": "https://myBlobStorage.blob.core.windows.net/fruit/abc.jpg",

"date\_captured": "<date>"

},

{

"id": 2,

"width": 1024,

"height": 768,

"file\_name": "xyz.jpg",

"coco\_url": "AmlDatastore://fruit/xyz.jpg",

"absolute\_url": "https://myBlobStorage.blob.core.windows.net/fruit/xyz.jpg",

"date\_captured": "<date>"

},

<...>

\],

"annotations": \[

{

"id": 1,

"category\_id": 1,

"image\_id": 1,

"area": 0.0

},

{

"id": 2,

"category\_id": 1,

"image\_id": 2,

"area": 0.0

},

<...>

\],

"categories": \[

{

"id": 1,

"name": "apple"

},

{

"id": 2,

"name": "orange"

},

{

"id": 3,

"name": "banana"

}

\]

}

Se você estiver rotulando um conjunto de dados de detecção de objetos, cada anotação no arquivo COCO também contém uma matriz de caixa delimitadora com os valores na matriz sendo _Esquerda_, _Topo_, _Largura_ e _Altura_.

"bbox": \[

0.11803319477782331,

0.41586723392402375,

0.7765206955096307,

0.3483334397217212

\]

# **Rotular e treinar um modelo personalizado**

A rotulagem de suas imagens de treinamento é feita no Estúdio do Azure Machine Learning, usando o Projeto de Rotulagem de Dados. Ter etiquetas completas e precisas para suas imagens de treinamento melhora muito o desempenho do seu modelo treinado. Ao rotular suas imagens, certifique-se de atribuir rótulos com precisão e rotular completamente todas as instâncias de cada classe.

![]()

![]()Há ferramentas com o Azure Machine Learning para ajudar na rotulagem, como a _rotulagem assistida por ML_, que pega alguns rótulos que você fornece para um subconjunto das imagens e tenta rotular as imagens restantes para você. Se estiver usando esses recursos, é importante revisar os rótulos para garantir que eles sejam precisos. Se não forem precisos, o desempenho do modelo treinado diminui.

Quando a rotulagem for concluída e todas as imagens de treinamento forem classificadas ou rotuladas corretamente, você poderá adicionar seu arquivo COCO ao conjunto de dados diretamente do workspace do Azure Machine Learning.

## **Treinar seu modelo**

Com todas as imagens de treinamento rotuladas, o próximo passo é treinar seu modelo. Ao treinar um modelo, selecione o tipo de modelo, especifique o conjunto de dados que deseja usar como dados de treinamento e indique o orçamento de treinamento. O orçamento de treinamento é um limite superior de tempo para execução do treinamento. O tempo real utilizado para o treinamento geralmente é menor do que o orçamento especificado.

Quando o modelo for treinado, selecioná-lo permite que você visualize o desempenho da execução da avaliação. Se um conjunto de dados de avaliação não for fornecido durante o treinamento do modelo, ele usará a execução de avaliação padrão. A execução de avaliação padrão retira um pequeno conjunto das imagens rotuladas do conjunto de treinamento, usa o modelo treinado para previsões nesse subconjunto e compara as previsões com os rótulos fornecidos.

Na página do modelo treinado, você pode disparar novas execuções de avaliação em um conjunto diferente de imagens ou experimentar seus próprios testes no Vision Studio selecionando a guia na parte superior da página.

**Identificar opções de detecção, análise e identificação faciais**

![]()Ao criar uma solução que usa dados faciais, as considerações incluem (mas não se limitam a):

*   **Dados, privacidade e segurança**. Os dados faciais são de identificação pessoal e devem ser considerados confidenciais e particulares. Você deve garantir que dispõe de proteção adequada para dados faciais usados para treinamento e inferência de modelos.
*   **Transparência**. Garanta que os usuários sejam informados sobre como seus dados faciais são usados e quem terá acesso a eles.
*   **Imparcialidade e inclusividade**. Garanta que o seu sistema baseado em reconhecimento facial não possa ser usado de maneira prejudicial às pessoas com base na sua aparência ou para atingi-las injustamente.

Para detectar e analisar rostos com o serviço de Visão de IA do Azure, chame a função REST de **Análise de Imagem** (SDK ou o método REST equivalente), especificando **Pessoas** como uma dos recursos visuais a serem retornados.

{

"modelVersion": "2023-10-01",

"metadata": {

"width": 400,

"height": 600

},

"peopleResult": {

"values": \[

{

"boundingBox": {

"x": 0,

"y": 56,

"w": 101,

"h": 189

},

"confidence": 0.9474349617958069

},

{

"boundingBox": {

"x": 402,

"y": 96,

"w": 124,

"h": 156

},

"confidence": 0.9310565276194865

},

...

\]

}

}

![]()

O serviço de Detecção Facial fornece funcionalidade que você pode usar para:

*   _Detecção facial_ – Para cada rosto detectado, os resultados incluem uma ID que identifica o rosto e as coordenadas da caixa delimitadora indicando a localização na imagem.
*   _Análise de atributo facial_ – Você pode retornar uma grande variedade de atributos faciais, entre eles:
    *   Posição da cabeça (orientação de _inclinação_, _rotação_ e _guinada_ no espaço 3D)
    *   Óculos (_sem óculos_, _óculos de leitura_, _óculos de sol_ ou _óculos de natação_)
    *   Desfoque (_baixo_, _médio_ ou _alto_)
    *   Exposição (_subexposição_, _boa exposição_ou _superexposição_)
    *   Ruído (ruído visual na imagem)
    *   Oclusão (objetos que obscurecem o rosto)
    *   Acessórios (óculos, chapéu, máscara)
    *   QualityForRecognition (_baixo_, _médio_ou _alto_)
*   _Localização do ponto de referência facial_ – Coordenadas para os principais pontos de referência em relação às características faciais (por exemplo, cantos de olho, pupilas, ponta do nariz e assim por diante)
*   _Comparação facial_ – Você pode comparar os rostos em várias imagens em busca de semelhanças (para encontrar indivíduos com características faciais semelhantes) e para verificação (a fim de determinar que um rosto em uma imagem é a mesma pessoa que um rosto em outra imagem)
*   _Reconhecimento do rosto_ – Você pode treinar um modelo com uma coleção de rostos que pertencem a indivíduos específicos e usar o modelo para identificar essas pessoas em novas imagens.
*   _Vivacidade facial_: a vivacidade pode ser usada para determinar se o vídeo de entrada é um fluxo real ou falso para impedir que indivíduos mal intencionados falsifiquem o sistema de reconhecimento.

Para treinar um modelo de reconhecimento do rosto com o serviço de Detecção Facial:

1.  Crie um **Grupo de pessoas** que defina o conjunto de indivíduos que você deseja identificar (por exemplo, _funcionários_).
2.  Adicione uma **Pessoa** ao **Grupo de pessoas** para cada indivíduo que você deseja identificar.
3.  Adicione rostos detectados de várias imagens a cada **pessoa**, preferencialmente em várias posições. As IDs desses rostos não expiram mais após 24 horas (portanto, agora são conhecidos como rostos _persistentes_).
4.  Treinar o modelo.

![]()

OCR (reconhecimento óptico de caracteres). O OCR permite extrair texto de imagens, como fotos de placas de rua e produtos, bem como de documentos — como manuscritos ou não estruturados.

*   **Análise de Imagem** OCR (reconhecimento óptico de caracteres):
    *   Use esse recurso para documentos gerais não estruturados com menor quantidade de texto ou imagens que contenham texto.
    *   Os resultados são retornados imediatamente (síncronos) de uma só chamada à API.
    *   Tem funcionalidade para analisar imagens além da extração de texto, incluindo a detecção de objetos, a descrição ou categorização de uma imagem, a geração de miniaturas recortadas inteligentes e muito mais.
    *   Os exemplos incluem: placas de rua, anotações manuscritas e placas de loja.
*   **Informação de Documentos**:
    *   Use esse serviço para ler grandes volumes de texto em imagens e documentos em PDF.
    *   Este serviço usa o contexto e a estrutura do documento para melhorar a precisão.
    *   A chamada de função inicial retorna uma ID de operação assíncrona, que deve ser usada em uma chamada subsequente para recuperar os resultados.
    *   Os exemplos incluem: recibos, artigos e faturas.

**Usar a API de Leitura**

Para usar o recurso OCR de Leitura, chame a função **ImageAnalysis** (API REST ou método de SDK equivalente), passando a URL da imagem ou os dados binários e, opcionalmente, especificando uma legenda com neutralidade de gênero ou o idioma em que o texto está escrito (com um valor padrão de **en** para inglês).

Para fazer uma solicitação de OCR para **ImageAnalysis**, especifique o recurso visual como READ.

ImageAnalysisResult result = client.Analyze(

<image-to-analyze>,

VisualFeatures.Read);

{

"metadata":

{

"width": 500,

"height": 430

},

"readResult":

{

"blocks":

\[

{

"lines":

\[

{

"text": "Hello World!",

"boundingPolygon":

\[

{"x":251,"y":265},

{"x":673,"y":260},

{"x":674,"y":308},

{"x":252,"y":318}

\],

"words":

\[

{

"text":"Hello",

"boundingPolygon":

\[

{"x":252,"y":267},

{"x":307,"y":265},

{"x":307,"y":318},

{"x":253,"y":318}

\],

"confidence":0.996

},

{

"text":"World!",

"boundingPolygon":

\[

{"x":318,"y":264},

{"x":386,"y":263},

{"x":387,"y":316},

{"x":319,"y":318}

\],

"confidence":0.99

}

\]

},

\]

}

\]

}

}

O serviço **Azure Video Indexer** foi projetado para ajudar você a extrair informações de vídeos. Ele fornece a funcionalidade que você pode usar para:

*   _Reconhecimento facial_ – detecção da presença de pessoas individuais na imagem. Isso exige a aprovação [Acesso Limitado](https://aka.ms/cog-services-limited-access).
*   _Reconhecimento óptico de caracteres_ – leitura de texto no vídeo.
*   _Transcrição de fala_ – criação de uma transcrição de texto do diálogo do vídeo.
*   _Tópicos_ – identificação dos principais tópicos discutidos no vídeo.
*   _Sentimento_ – análise de quão positivos ou negativos são os segmentos no vídeo.
*   _Rótulos_ – marcas de rótulo que identificam objetos ou temas chave em todo o vídeo.
*   _Moderação de conteúdo_ – detecção de temas adultos ou violentos no vídeo.
*   _Segmentação de cena_ – um detalhamento do vídeo quanto às cenas integrantes.

O serviço Analisador de Vídeo fornece um site do portal que pode ser usado para carregar, exibir e analisar vídeos interativamente.

Você pode estender os recursos de reconhecimento do Analisador de Vídeo ao criar modelos personalizados para:

*   **Pessoas**. Adicione imagens dos rostos de pessoas que você deseja que sejam reconhecidas em vídeos e treine um modelo. O Video Indexer reconhecerá essas pessoas em todos os seus vídeos.
*   **Idioma**. Se sua organização usa uma terminologia específica que pode não ser de uso comum, você pode treinar um modelo personalizado para detectá-la e transcrevê-la.
*   **Marcas**. Você pode treinar um modelo para reconhecer nomes específicos como marcas para identificar produtos, projetos ou empresas relevantes para sua empresa.
*   **Widgets do Azure Video Indexer**
*   Os widgets usados no portal do Azure Video Indexer para reproduzir, analisar e editar vídeos podem ser inseridos em suas próprias interfaces HTML personalizadas. Você pode usar essa técnica para compartilhar insights de vídeos específicos com outras pessoas sem conceder a elas o acesso completo à sua conta no portal do Azure Video Indexer.
*   **API do Azure Video Indexer**
*   O Azure Video Indexer fornece uma API REST que você pode usar para obter informações sobre sua conta, incluindo um token de acesso.
*   HTTPCopiar
*   https://api.videoindexer.ai/Auth/<location>/Accounts/<accountId>/AccessToken
*   Em seguida, você pode usar seu token para consumir a API REST e automatizar tarefas de indexação de vídeo, criando projetos, recuperando insights e criando ou excluindo modelos personalizados.
*   Por exemplo, uma chamada GET para o ponto de extremidade REST https://api.videoindexer.ai/<location>/Accounts/<accountId>/Customization/CustomLogos/Logos/<logoId>?<accessToken> retorna o logotipo especificado. Em outro exemplo, você pode enviar uma solicitação GET para https://api.videoindexer.ai/<location>/Accounts/<accountId>/Videos?<accessToken>, que retorna detalhes de vídeos em sua conta,
