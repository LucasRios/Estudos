# **O que é Aprendizado de Máquina?**

## **Definição Geral**

Aprendizado de máquina (machine learning) é um campo da Inteligência Artificial que permite que computadores **aprendam padrões a partir de dados**, sem a necessidade de serem programados explicitamente para cada tarefa.

Essa definição é atribuída a **Arthur Samuel**, uma das figuras mais importantes na história da área. Para ele, aprendizado de máquina é:

"O campo de estudo que dá aos computadores a capacidade de aprender sem serem explicitamente programados."

Essa definição destaca o elemento central do aprendizado de máquina:
**o computador melhora sua performance com experiência.**

# **O Exemplo Clássico: O Programa de Damas de Arthur Samuel**

## **Contexto Histórico**

Na década de 1950, Arthur Samuel desenvolveu um dos primeiros programas capazes de **aprender**. Ele criou um sistema para jogar damas, mesmo **não sendo um jogador habilidoso**.

## **Como o Programa Aprendeu**

Samuel instruiu o computador a:

*   Jogar contra si mesmo **dezenas de milhares de vezes**.
*   Registrar quais **posições de tabuleiro** normalmente levavam à vitória.
*   Registrar quais posições levavam a derrota.
*   Ajustar sua estratégia para buscar boas posições e evitar as ruins.

Com o tempo:

*   O programa acumulou mais experiência do que qualquer humano seria capaz.
*   Aprendeu padrões que Samuel não saberia descrever manualmente.
*   Tornou-se **melhor jogador de damas do que o próprio Samuel**.

Esse exemplo é importante porque ilustra:

*   Aprendizado baseado em dados e experiência.
*   Escalabilidade: o computador suporta volumes enormes de prática.
*   A essência do machine learning moderno.

## A Importância de Muitos Exemplos

Durante o vídeo, há um mini-questionário perguntando:

**“O que aconteceria se o computador tivesse jogado muito menos partidas?”**

A resposta correta é:

→ Ele teria um desempenho pior.

Esse ponto é fundamental:

*   Quanto mais dados ou experiências um algoritmo tem,
    **melhor sua capacidade de identificar padrões.**
*   Isso vale para jogos, classificação de imagens, previsões de vendas, detecção de spam etc.

O vídeo reforça que o objetivo desses quizzes não é acertar de primeira, mas **fixar os conceitos**.

# **Tipos Principais de Aprendizado de Máquina**

O curso apresenta três categorias principais:

## **1\. Aprendizado Supervisionado**

*   O modelo aprende a partir de exemplos **rotulados**.
*   Cada instância nos dados tem uma resposta correta.
*   O objetivo é prever o rótulo de novos dados nunca vistos.

Exemplos:

*   Prever preço de casas.
*   Classificar imagens como “gato” ou “cachorro”.
*   Identificar e-mails como “spam” ou “não spam”.

Este será o foco dos primeiros dois cursos da especialização.

## **2\. Aprendizado Não Supervisionado**

*   Os dados **não têm rótulos**.
*   O modelo tenta encontrar padrões, agrupamentos e estruturas escondidas.

Exemplos:

*   Agrupar clientes com comportamentos semelhantes.
*   Encontrar padrões em dados de sensores.
*   Reduzir dimensionalidade de dados para visualização.

Será explorado mais profundamente no terceiro curso.

## **3\. Sistemas de Recomendação e Aprendizado por Reforço**

*   Sistemas de recomendação: recomendam filmes, produtos, músicas etc.
*   Aprendizado por reforço: o agente aprende por tentativa e erro, recebendo recompensas.

O terceiro curso da especialização incluirá esses temas.

## Algoritmos São Apenas Ferramentas: O Valor Está na Aplicação

O instrutor enfatiza um ponto essencial:

Conhecer algoritmos é importante, mas saber **como aplicá-los corretamente** é ainda mais importante.

Comparação utilizada no vídeo:

*   Aprender algoritmos é como receber um conjunto de ferramentas (martelo, furadeira etc.).
*   Mas apenas entregar boas ferramentas não faz alguém construir uma casa.
*   O valor real está no **uso correto**, **decisões de projeto**, **boas práticas** e **conhecimento aplicado**.

## **Erros comuns em equipes reais**

O instrutor relata ter visitado grandes empresas e observado equipes experientes que:

*   Trabalharam por meses com um algoritmo inadequado.
*   Tentaram resolver um problema com a técnica errada.
*   Poderiam ter economizado meses de esforço com orientação correta desde o início.

# **Aprendizado Supervisionado – Parte 1**

## **Visão Geral**

O aprendizado supervisionado é responsável por **cerca de 99% do valor econômico gerado pelo machine learning atualmente**. É a categoria mais madura, mais aplicada e a que concentra a maior parte das soluções práticas no mercado.

O conceito central é simples:
O algoritmo aprende uma função que **mapeia entradas (x) para saídas (y)**.
Para isso, ele recebe exemplos onde você fornece:

*   A **entrada x**
*   A **resposta correta y** (o rótulo)

Após ver muitos exemplos, o modelo aprende a prever y para **novas entradas**, mesmo quando nunca as viu antes.

# **Como Funciona o Aprendizado Supervisionado**

## **A Ideia de “Exemplos Rotulados”**

A característica essencial do aprendizado supervisionado é que o algoritmo treina com um conjunto de dados onde:

*   Cada entrada **x** possui um rótulo correto **y**.
*   O modelo aprende padrões que relacionam x → y.
*   Depois do treinamento, ele consegue prever y apenas a partir de x.

## **Estrutura Geral**

1.  **Treinamento:** você fornece pares corretos ⟨x, y⟩.
2.  **Aprendizado:** o algoritmo identifica a relação entre x e y.
3.  **Predição:** inserindo apenas x, ele produz uma estimativa de y.

Essa estrutura aparece em praticamente todos os casos de uso reais.

# **Exemplos de Aplicações de Aprendizado Supervisionado**

## **1\. Filtro de Spam**

*   **Entrada (x):** texto e metadados do e-mail.
*   **Saída (y):** spam / não spam.
    O modelo aprende com milhares de exemplos de e-mails rotulados.

## **2\. Reconhecimento de Fala**

*   **Entrada:** áudio.
*   **Saída:** texto transcrito.
    O algoritmo aprende a mapear padrões acústicos para palavras.

## **3\. Tradução Automática**

*   **Entrada:** frase em um idioma.
*   **Saída:** frase traduzida em outra língua.
    Modelos treinam com bilhões de pares de sentenças paralelas.

## **4\. Publicidade Online (uma das aplicações mais lucrativas)**

*   **Entrada:** características do anúncio + dados do usuário.
*   **Saída:** probabilidade de clique (CTR).

Cada clique gera receita; logo:

*   Prever cliques corretamente tem valor econômico direto.
*   Plataformas inteiras dependem de modelos supervisionados para isso.

## **5\. Carros Autônomos**

*   **Entrada:** imagens + sensores (radar, LIDAR, etc.).
*   **Saída:** localização de carros, pedestres, faixas, sinais.
    O aprendizado supervisionado permite interpretar a cena e dirigir de forma segura.

## **6\. Inspeção Visual em Manufatura**

*   **Entrada:** imagem do produto recém-fabricado.
*   **Saída:** “defeituoso” ou “sem defeito”.
    Ajuda fábricas a reduzir retrabalho e aumentar a qualidade.

# **Processo: Treinar com Exemplos, Prever em Novos Casos**

Em todos os exemplos acima:

*   Primeiro o modelo vê muitos pares x → y.
*   Depois, consegue prever y para novos x nunca vistos.

# **Exemplo Prático: Previsão de Preço de Casas**

## **O Problema**

Você quer prever o preço de uma casa baseado no seu tamanho (em m² ou ft²).

### **Dados:**

*   Eixo horizontal: tamanho da casa.
*   Eixo vertical: preço da casa.

Depois de plotar os dados, surge uma tendência clara.

## **Predição Simples: Ajuste de Linha Reta**

Um algoritmo pode:

1.  Traçar uma linha que melhor se ajusta aos pontos.
2.  Usar a linha para prever o preço de uma casa de, por exemplo, **750 ft²**.
3.  A linha pode sugerir um valor aproximado, como **US$ 150.000**.

## **Modelo Mais Complexo: Ajuste de Curva**

Uma linha reta nem sempre é suficiente.
Outro modelo pode ajustar:

*   Uma **curva** mais flexível.
*   Uma função **não linear**.

Ao fazer isso, a previsão para 750 ft² pode mudar para algo como **US$ 200.000**.

O curso ensinará como escolher sistematicamente entre uma linha reta, uma curva mais complexa ou até funções mais sofisticadas.

Não se escolhe o modelo pela resposta mais conveniente, e sim pela **capacidade real de generalizar bem**.

# **Por Que Isso é Aprendizado Supervisionado?**

Porque em cada ponto do conjunto de dados:

*   Temos o tamanho da casa (**x**)
*   E temos o preço correto (**y**)

O algoritmo aprende com as respostas corretas e passa a prever novos casos.

# **Subtipos de Aprendizado Supervisionado**

## **1\. Regressão**

Usada quando o objetivo é **prever um número contínuo**, como:

*   Preço de casas
*   Temperatura
*   Valor de vendas
*   Probabilidades

O espaço de possíveis valores é **infinito** (ex.: qualquer valor entre 0 e 300.000).

O exemplo do preço da casa é um tipo clássico de regressão.

## **2\. Classificação**

Outro tipo importante, apresentado no próximo vídeo:

*   A tarefa é prever **categorias**.
*   Exemplos:
    *   spam / não spam
    *   defeito / sem defeito
    *   doença A / doença B / saudável

A classificação será aprofundada na próxima parte.

![]()

# **Aprendizado Supervisionado – Parte 2**

## **Relembrando o Conceito**

No aprendizado supervisionado, o objetivo do algoritmo é aprender um **mapeamento entre entrada (x) e saída (y)**.
No vídeo anterior, você viu a **regressão**, onde o modelo prevê um número contínuo — por exemplo, o preço de uma casa.

Agora entramos no segundo grande grupo dentro do aprendizado supervisionado: **classificação**.

# **Classificação: O Que é?**

## **Definição**

Classificação é um tipo de algoritmo supervisionado que:

*   Não tenta prever um número contínuo.
*   Em vez disso, prevê **categorias** (também chamadas de _classes_).

As categorias representam um **conjunto finito de possíveis resultados**, como:

*   “benigno” ou “maligno”
*   “gato”, “cachorro”, “pássaro”
*   “spam” ou “não spam”

Esse conjunto é limitado e discreto, ao contrário da regressão, onde valores podem ser infinitos.

# **Exemplo Real: Detecção de Câncer de Mama**

## **Objetivo do Sistema**

Construir um modelo que ajude médicos a:

*   Avaliar se um tumor é **benigno (classe 0)**
    ou
*   **Maligno (classe 1)**.

Esse tipo de diagnóstico é essencial, pois o câncer detectado precocemente pode salvar vidas.

## **Estrutura dos Dados**

Cada tumor no conjunto de dados tem:

*   **Tamanho do tumor (entrada x)**
*   **Classificação benigna (0) ou maligna (1) (rótulo y)**

Podemos plotar isso em um gráfico:

*   Eixo horizontal: **tamanho do tumor**
*   Eixo vertical: **classe** (0 ou 1)

Esse gráfico mostra que:

*   Há apenas **duas saídas possíveis**, em vez de infinitas possibilidades.

Isso caracteriza um problema de **classificação binária**.

# **Representação Visual em Classificação**

O vídeo exemplifica usando símbolos:

*   **Círculo (O):** tumor benigno
*   **Cruz (X):** tumor maligno

Com essa visualização, ao analisar um novo paciente, o algoritmo deve responder:

Dado o tamanho do tumor, ele deve ser classificado como benigno ou maligno?

# **Classificação com Múltiplas Categorias**

Nem sempre são apenas duas categorias.
Exemplos:

*   Diferentes **tipos de câncer** (tipo 1, tipo 2 etc.)
*   Diferentes **espécies de animais**
*   Diferentes **níveis de severidade** de uma doença

Nesse caso, o espaço de saída pode ser:

*   {0, 1, 2}, ou qualquer conjunto finito de classes.

Observação importante:

*   Mesmo que as classes sejam representadas por números, esses números não são valores contínuos.
*   Eles representam **categorias**, não quantidades.

# **Diferença Principal Entre Regressão e Classificação**

### **Regressão:**

*   Saída é um **número contínuo**, podendo assumir infinitos valores.
*   Ex.: 72.5, 150000, 0.43 etc.

### **Classificação:**

*   Saída é uma **categoria**, escolhida dentro de um conjunto finito.
*   Ex.: 0 ou 1; ou 0, 1, 2.

# **Usando Mais de Uma Entrada (Multidimensional)**

O exemplo anterior usava apenas **uma** entrada: o tamanho do tumor.
Mas sistemas reais costumam usar várias entradas simultaneamente.

## **Exemplo com Duas Entradas:**

*   **Idade do paciente**
*   **Tamanho do tumor**

Agora, cada ponto no gráfico é bidimensional, representando:

*   (idade, tamanho) → classe

O algoritmo agora deve encontrar um **limite de decisão** que separe tumores benignos dos malignos.

Esse limite pode ser:

*   uma linha,
*   uma curva,
*   ou uma fronteira mais complexa.

Esse limite é o que permite **classificar novos pacientes**.

# **Modelos com Muitas Entradas**

Na prática, modelos de detecção de câncer usam dezenas de variáveis, como:

*   Espessura do tecido tumoral
*   Uniformidade do tamanho das células
*   Uniformidade da forma celular
*   Textura
*   Densidade de massa
*   entre outras características clínicas

Com múltiplos atributos, o espaço deixa de ser bidimensional e passa a ter muitas dimensões — algo natural para algoritmos modernos.

# **Aprendizado Não Supervisionado – Parte 1**

## **Introdução ao Aprendizado Não Supervisionado**

Depois do aprendizado supervisionado, o **aprendizado não supervisionado** é o segundo tipo mais usado de machine learning.
Apesar do nome sugerir algo “menos estruturado”, essa categoria é extremamente poderosa e útil em diversos contextos reais.

No aprendizado **supervisionado**, cada exemplo de treinamento inclui:

*   uma entrada **x**
*   um rótulo correto **y**

No aprendizado **não supervisionado**, isso desaparece:

*   você recebe apenas as entradas **x**
*   **não** existem rótulos
*   nada indica previamente qual é a “resposta certa”

O algoritmo, portanto, precisa **descobrir sozinho** padrões, estruturas internas ou relações interessantes dentro dos dados.

# **Diferença Essencial: Supervisionado vs. Não Supervisionado**

## **Supervisionado**

*   O modelo aprende com pares ⟨entrada, rótulo⟩.
*   Ex.: tumor benigno (0) vs. maligno (1).

## **Não supervisionado**

*   Recebemos apenas as entradas.
*   Não existe rótulo “benigno” ou “maligno”.
*   A tarefa é **descobrir padrões** sem orientação.

Exemplo citado:

*   Dados contendo **idade do paciente** e **tamanho do tumor**, mas **sem indicar se é benigno ou maligno**.

Visualmente, isso significa um gráfico apenas com pontos dispersos, sem categorias prévias.

# **Objetivo do Aprendizado Não Supervisionado**

O algoritmo tenta encontrar:

*   Estruturas ocultas
*   Padrões naturais
*   Divisões internas
*   Agrupamentos
*   Similaridades e diferenças

Ou, de forma geral:

“Descobrir o que há de interessante nos dados.”

Não existe “resposta certa” para ensinar.
O algoritmo tem liberdade para explorar e identificar as estruturas mais coerentes.

# **Algoritmo de Agrupamento (Clustering)**

O tipo mais clássico e mais usado de aprendizado não supervisionado é o **clustering**.

### **O que ele faz?**

Agrupa dados similares entre si e separa dados diferentes entre si.

### **Exemplo simples:**

Com os dados de idade e tamanho do tumor, o algoritmo pode encontrar que:

*   Existe um **grupo 1** com tumores pequenos e pacientes jovens.
*   Existe um **grupo 2** com tumores maiores ou pacientes mais velhos.

Esses grupos surgem **sem que ninguém diga ao algoritmo** o que significa cada grupo.

# **Exemplo 1: Agrupamento no Google News**

## **Como funciona?**

O Google News analisa diariamente **centenas de milhares de artigos** de notícias.
Como ninguém pode rotular tudo manualmente, o sistema usa clustering para agrupar textos semelhantes.

### **Exemplo mostrado no vídeo:**

Notícias sobre:

*   Um panda gigante que deu à luz gêmeos no zoológico.

O algoritmo:

*   Identifica artigos com palavras em comum, como _panda_, _gêmeos_, _zoo_.
*   Agrupa automaticamente esses textos, sem que ninguém especifique as regras.

### **Por que isso é importante?**

*   Os temas do dia mudam rapidamente.
*   Não existe tempo para humanos definirem critérios.
*   O algoritmo precisa ser capaz de reagir automaticamente ao conteúdo publicado.

Esse exemplo mostra bem a essência do aprendizado não supervisionado:

O algoritmo descobre sozinho quais características (palavras, padrões, correlações) são relevantes para formar grupos.

# **Exemplo 2: Agrupamento de Dados Genéticos (DNA)**

## **O que são microarranjos de DNA?**

O vídeo mostra uma matriz onde:

*   Cada **coluna** corresponde a um indivíduo.
*   Cada **linha** corresponde a um gene.
*   Cores diferentes representam o nível de expressão de cada gene.

Esses dados são extremamente complexos:

*   Milhares de genes
*   Centenas de pessoas
*   Sem rótulos dizendo quem pertence a qual grupo genético

## **Como o clustering ajuda?**

O algoritmo pode:

1.  Analisar padrões de expressão gênica.
2.  Encontrar grupos naturais de indivíduos, por exemplo:
    1.  **Grupo 1:** pessoas com características genéticas similares.
    2.  **Grupo 2:** indivíduos com outro padrão biológico.
    3.  **Grupo 3:** outro conjunto distinto.

Esses grupos podem representar:

*   Predisposições genéticas
*   Padrões hereditários
*   Similaridades fenotípicas
*   Respostas a determinados estímulos

Nada disso é informado ao algoritmo — ele descobre tudo analisando apenas os dados brutos.

# **Exemplo 3: Segmentação de Clientes (Marketing)**

Empresas possuem grandes bases de dados contendo registros de seus clientes:

*   Idade
*   Comportamento de compra
*   Interesses
*   Histórico de serviços utilizados
*   País de origem
*   Preferências de conteúdo

Sem rótulos claros, o objetivo é:

Encontrar grupos de clientes com comportamentos semelhantes para oferecer produtos, cursos ou serviços mais adequados.

### **Exemplo real citado no vídeo:**

O time da DeepLearning.AI aplicou clustering na sua comunidade e descobriu grupos motivacionais:

*   Pessoas que querem **aprender IA para adquirir conhecimento**.
*   Pessoas interessadas em **melhorar sua carreira**.
*   Pessoas que desejam **acompanhar como a IA impacta sua área**.

Esse tipo de segmentação permite:

*   Comunicações mais personalizadas.
*   Conteúdos mais relevantes.
*   Melhor suporte ao público.

# **Por que isso é Aprendizado Não Supervisionado?**

Em todos os exemplos:

*   **Não existe rótulo prévio.**
*   Não há categorias predefinidas.
*   O algoritmo descobre padrões **sem supervisão humana**.

Em vez de dizer:

“Este é o grupo A, este é o grupo B.”

Dizemos apenas:

“Aqui estão os dados. Descubra por conta própria a estrutura mais natural dentro deles.”

# **Recapitulando**

## **Aprendizado não supervisionado:**

*   Usa dados **sem rótulos**.
*   Procura **padrões ocultos**, **estrutura**, **agrupar indivíduos**, **reduzir dimensionalidade**, entre outros objetivos.
*   O tipo mais comum é o **clustering**, que divide automaticamente dados em grupos.

### **Exemplos vistos:**

*   Artigos de notícias agrupados por temas (Google News).
*   Agrupamento genético com microarranjos de DNA.
*   Segmentação de clientes para personalizar conteúdos e serviços.

![]()

# **Aprendizado Não Supervisionado – Parte 2**

## **Revisão Rápida**

No vídeo anterior, você viu:

*   O conceito geral de aprendizado não supervisionado.
*   A diferença entre supervisionado (com rótulos) e não supervisionado (sem rótulos).
*   O algoritmo **clustering**, que agrupa dados similares automaticamente.

Agora, o instrutor aprofunda a definição formal e apresenta outros tipos muito importantes de aprendizado não supervisionado.

# **Definição Formal de Aprendizado Não Supervisionado**

## **Estrutura dos Dados**

*   **Aprendizado supervisionado:** entradas **x** + rótulos de saída **y**.
*   **Aprendizado não supervisionado:** apenas entradas **x**, sem qualquer rótulo **y**.

O algoritmo não recebe instruções de qual é a resposta correta.
Ele deve **analisar os dados por conta própria** e descobrir:

*   Padrões,
*   Estruturas internas,
*   Grupos,
*   Relações relevantes,
*   Informações úteis escondidas.

Essa ausência de rótulos é o que torna o aprendizado não supervisionado mais exploratório.

# **Tipos de Aprendizado Não Supervisionado Apresentados no Curso**

A especialização foca em três categorias principais:

## **1\. Agrupamento (Clustering)**

Já explicado no vídeo anterior.

### **Objetivo:**

Agrupar automaticamente exemplos semelhantes entre si.

### **Usos comuns:**

*   Agrupamento de notícias (Google News)
*   Segmentação de clientes
*   Grupos de padrões de DNA
*   Agrupamento de imagens, documentos, comportamentos etc.

Clustering é a técnica mais “intuitiva” e frequentemente a primeira forma de aprendizado não supervisionado estudada.

## **2\. Detecção de Anomalias (Anomaly Detection)**

Um dos tipos mais importantes na prática.

### **O que é?**

Identificar pontos de dados **muito diferentes** dos demais.

Esses pontos podem indicar:

*   Comportamentos suspeitos,
*   Falhas,
*   Eventos raros,
*   Problemas operacionais,
*   Erros em sistemas,
*   Situações indesejadas.

### **Aplicações:**

*   **Detecção de fraude financeira:**
    Transações com valores ou padrões fora do comum podem sinalizar fraude.
*   **Monitoramento de máquinas e sensores:**
    Mudanças inesperadas podem indicar falhas.
*   **Segurança digital:**
    Detecção de atividades incomuns que podem indicar invasões.

O algoritmo aprende o “comportamento normal” dos dados e marca aquilo que se afasta muito desse padrão.

## **3\. Redução de Dimensionalidade (Dimensionality Reduction)**

Uma técnica poderosa e frequentemente surpreendente.

### **O que é?**

Comprimir um conjunto de dados de **alta dimensionalidade** (muitas variáveis) em outra representação de dimensões menores, **preservando ao máximo a informação essencial**.

Funciona quase como _“magia matemática”_, pois:

*   Reduz centenas ou milhares de atributos para poucos.
*   Facilita visualização.
*   Acelera cálculos.
*   Remove ruídos.
*   Destaca os padrões mais importantes.

### **Exemplo típico:**

*   Reduzir 50 variáveis genéticas → 2 dimensões para visualização em gráfico.
*   Reduzir 300 características de imagens → 10 variáveis mais informativas.

Técnicas comuns (que serão estudadas mais tarde):

*   PCA (Principal Component Analysis)
*   Autoencoders (em deep learning)
*   t-SNE, UMAP (para visualização)

# **Verificação de Compreensão: Quais são exemplos de aprendizado não supervisionado?**

O vídeo apresenta quatro situações e pede que o aluno identifique quais são supervisionadas e quais são não supervisionadas.

### **Analisando cada uma:**

### **1\. Filtro de spam**

*   Tem rótulos (spam / não spam).
    → **Aprendizado supervisionado**

### **2\. Agrupamento de notícias (Google News)**

*   Nenhum rótulo; o algoritmo agrupa sozinho.
    → **Aprendizado não supervisionado**

### **3\. Segmentação de mercado**

*   Dados sem rótulos dizendo qual tipo de cliente é qual.
    → **Aprendizado não supervisionado**

### **4\. Diagnóstico de diabetes**

*   Similar ao exemplo de tumor benigno/maligno.
*   Rótulos: diabetes / não diabetes.
    → **Aprendizado supervisionado**

# **Modelo de Regressão Linear – Parte 1**

## **Visão Geral**

Neste vídeo, o instrutor apresenta:

*   O **processo geral do aprendizado supervisionado**,
*   O **primeiro modelo estudado no curso**: **Regressão Linear**,
*   A **notação padrão** usada em machine learning.

A regressão linear é provavelmente **o algoritmo de aprendizado de máquina mais utilizado no mundo**, aparecendo em aplicações acadêmicas, industriais e comerciais há décadas.

# **O Problema: Prever o Preço de uma Casa**

## **Contexto**

Você deseja prever o preço de uma casa a partir de seu tamanho.
Para isso, utiliza um conjunto de dados de casas em **Portland (EUA)** contendo:

*   **Área da casa (x)**, em pés quadrados (ft²)
*   **Preço de venda (y)**, em milhares de dólares

Esses dados são plotados em um gráfico:

*   **Eixo horizontal:** tamanho da casa (ft²)
*   **Eixo vertical:** preço (milhares de dólares)

Cada ponto no gráfico representa uma casa real.

## **O Cenário Prático**

Imagine que você é um agente imobiliário em Portland.
Uma cliente quer vender sua casa, que tem **1250 ft²**.

Ela pergunta:

“Quanto posso conseguir vendendo minha casa?”

O objetivo é usar o modelo de aprendizado supervisionado para **estimar o preço de venda**.

# **Ajustando uma Linha Reta aos Dados**

## **Criando o Modelo de Regressão Linear**

A regressão linear busca ajustar **uma linha reta** que melhor representa a relação entre:

*   O tamanho da casa
*   O preço de venda

O modelo aprende essa linha usando o conjunto de treinamento.

Quando a linha é plotada sobre os dados:

*   Para **1250 ft²**, a linha cruza o eixo vertical aproximadamente em **US$ 220.000**,
*   Logo, essa seria uma estimativa razoável para o preço da casa da cliente.

# **Por que isso é Aprendizado Supervisionado?**

Porque o modelo aprende com exemplos onde a “resposta correta” já é conhecida:

*   Para cada casa no conjunto de dados, você sabe seu tamanho **x**
*   E sabe seu preço real **y**

Durante o treinamento:

1.  O modelo recebe pares (x, y).
2.  Aprende a relação que liga x → y.
3.  Depois, consegue prever y apenas com base em x.

Como os preços reais são fornecidos, isso é **supervisionado**.

# **Regressão x Classificação**

## **Regressão**

*   O modelo prevê **números contínuos**, como:
    *   Preços,
    *   Temperaturas,
    *   Probabilidades,
    *   Consumo de energia.

Há infinitos valores possíveis.
O exemplo da previsão do preço da casa é regressão.

## **Classificação**

*   O modelo prevê **categorias** discretas, como:
    *   “gato” vs. “cachorro”,
    *   “doente” vs. “não doente”,
    *   “10 possíveis diagnósticos”.

O número de possíveis saídas é finito e limitado.

Essa distinção é fundamental ao longo de todo o curso.

# **Representação dos Dados: Gráfico e Tabela**

## **Duas Formas de Visualizar os Dados**

### **1\. Gráfico**

*   Mostra visualmente o relacionamento entre tamanho e preço.

### **2\. Tabela**

Cada linha representa uma casa, com:

*   **Entrada (x):** tamanho em ft²
*   **Saída (y):** preço em milhares de dólares

Por exemplo:

*   Primeira linha:
    *   x = 2104
    *   y = 400
        Representa uma casa de **2104 ft² vendida por US$ 400.000**.

O gráfico e a tabela apresentam exatamente os mesmos dados, apenas de formas diferentes.

O conjunto mostrado possui **47 casas** → 47 exemplos de treinamento.

# **Notação Padrão em Machine Learning**

A notação apresentada aqui será usada ao longo de toda a especialização (e na maior parte da literatura de ML), então vale entendê-la bem.

## **Variáveis**

*   **x** = entrada (feature)
    *   Ex.: tamanho da casa
*   **y** = saída (rótulo / target)
    *   Ex.: preço da casa

## **Número de exemplos de treinamento**

*   **m = número total de exemplos**
    *   Neste caso: m = 47

## **Um exemplo de treinamento**

*   Representado como **(x, y)**
    *   Exemplo: (2104, 400)

## **Índices para indicar cada exemplo**

*   **x^(i)** = entrada do i-ésimo exemplo
*   **y^(i)** = saída do i-ésimo exemplo

Por exemplo:

*   **x^(1) = 2104**
*   **y^(1) = 400**

Observação importante:

O sobrescrito **(i)** não é exponenciação.
Não significa x elevado a i, e sim “exemplo número i”.

Essa notação permite descrever conjuntos de dados grandes e complexos de forma clara.

# **Conjunto de Treinamento**

O conjunto de dados usado para treinar o modelo é chamado de:

## **Training Set (Conjunto de Treinamento)**

A casa da sua cliente **não está no conjunto de treinamento**, porque ela ainda não foi vendida — logo, seu preço real é desconhecido.

A sequência é:

1.  Treinar o modelo usando o training set.
2.  Usar o modelo treinado para prever o preço da casa nova (1250 ft²).![]()

# **Modelo de Regressão Linear – Parte 2**

## **Objetivo do Vídeo**

Neste vídeo, o instrutor explica:

*   O fluxo completo do **aprendizado supervisionado**,
*   O que o algoritmo faz com o conjunto de treinamento,
*   O que é o modelo **f(x)** e como representá-lo matematicamente,
*   O conceito de **previsão** (ŷ),
*   E a estrutura matemática da regressão linear simples.

# **Como Funciona o Aprendizado Supervisionado**

## **Estrutura do Conjunto de Treinamento**

O conjunto de treinamento é composto por:

*   **Entradas (features)**: ex.: tamanho da casa (x)
*   **Saídas (targets)**: ex.: preço da casa (y)

As saídas y são consideradas as **respostas corretas** para o aprendizado.

Durante o treinamento:

1.  **Entradas (x)** e **saídas (y)** são fornecidas ao algoritmo.
2.  O algoritmo analisa esses dados.
3.  Ele produz uma **função f**, também chamada de **modelo**, capaz de fazer previsões para novos valores de x.

# **O Modelo: a Função f**

## **O que o algoritmo retorna?**

Após receber o conjunto de treinamento, o algoritmo supervisionado gera uma função:

### **f(x)**

Essa função será usada para fazer previsões sobre dados novos.

Historicamente, esta função era chamada de **hipótese (h)**.
Neste curso, chama-se apenas **função f**.

## **Previsão: o papel de ŷ (y-hat)**

Quando fornecemos uma nova entrada **x** para o modelo, ele produz:

### **ŷ (y-hat)**

*   **ŷ** é a **previsão**,
*   **y** é o **valor real** (caso exista).

Exemplo:

*   O preço real da casa do cliente (y) é desconhecido, pois ela ainda não foi vendida.
*   O modelo calcula **ŷ**, sua estimativa para esse preço.

Portanto:

*   **y** = valor real, conhecido apenas nos dados de treinamento
*   **ŷ** = valor previsto pelo modelo, calculado pela função f

# **Como Representamos a Função f**

## **Forma matemática do modelo**

Para regressão linear simples (1 variável), usamos uma função de linha reta:

### **f(x) = w·x + b**

Onde:

*   **w** = inclinação da linha (peso, coeficiente)
*   **b** = intercepto (ponto onde a linha cruza o eixo vertical)
*   **x** = entrada
*   **f(x) = ŷ** = previsão

O modelo é mais formalmente escrito como:

### **f<sub>w,b</sub>(x) = w·x + b**

Mostrando que a previsão depende dos valores de **w** e **b**, que o algoritmo irá aprender.

## **Representação Simplificada**

Para facilitar a escrita:

*   Às vezes omitimos o subscrito w,b e escrevemos apenas **f(x)**.
*   O significado permanece o mesmo.

# **Visualizando o Modelo no Gráfico**

Ao traçar os dados no gráfico (x no eixo horizontal e y no vertical), o algoritmo tenta encontrar a **linha que melhor se ajusta aos pontos**.

Essa linha é precisamente a representação de:

### **f(x) = w·x + b**

Cada ponto do gráfico:

*   Mostra um exemplo de treinamento,
*   E a linha tenta capturar a tendência geral desses pontos.

# **Por Que Usar uma Linha Reta?**

Mesmo que funções mais complexas (curvas, parábolas, etc.) possam se ajustar melhor em alguns casos, a linha reta é usada porque:

*   É **simples**,
*   É **rápida de treinar**,
*   É **interpretável**,
*   Serve como uma **base sólida** para modelos mais avançados.

Mais tarde no curso, você verá modelos:

*   Não lineares,
*   Polinomiais,
*   E modelos com múltiplas variáveis.

# **Nome do Modelo: Regressão Linear Univariada**

Porque:

*   “Linear” → o modelo ajusta uma reta,
*   “Univariada” → utiliza **uma única variável de entrada (x)**.

Exemplo:

*   Somente o tamanho da casa.

Nos próximos vídeos, será apresentada a versão **multivariada**, incluindo:

*   Número de quartos
*   Idade da casa
*   Localização
*   Outras características

![]()

# **Função de Custo na Regressão Linear**

## **Objetivo do Vídeo**

Este vídeo explica:

*   O que é a **função de custo** na regressão linear,
*   Por que ela é necessária,
*   Como ela mede o erro entre previsões e valores reais,
*   Como é construída matematicamente,
*   E como será usada para ajustar os parâmetros **w** e **b** do modelo.

# **Parâmetros do Modelo: w e b**

Na regressão linear simples, usamos o seguinte modelo:

## **Modelo (hipótese / função):**

_fw,b(x)=w⋅x+bf\_{w,b}(x) = w \\cdot x + b_fw,b (x)=w⋅x+b

Onde:

*   **w** = peso, coeficiente, inclinação
*   **b** = bias, intercepto
*   Ambos são **parâmetros do modelo**, ajustados durante o treinamento

Alterar **w** e **b** muda completamente a linha traçada no gráfico, e portanto muda as previsões.

# **Intuição: Como w e b afetam a linha**

### **1\. Quando w = 0 e b = 1.5**

_f(x)=0⋅x+1.5=1.5f(x) = 0 \\cdot x + 1.5 = 1.5_f(x)=0⋅x+1.5=1.5

*   É uma linha **horizontal**
*   Sempre prevê **1.5**, independentemente de x
*   b define onde ela cruza o eixo Y → **intercepto**

### **2\. Quando w = 0.5 e b = 0**

_f(x)=0.5⋅xf(x) = 0.5 \\cdot x_f(x)=0.5⋅x

*   Inclinação = **0.5**
*   Para x = 2 → f(2) = 1
*   Para x = 0 → f(0) = 0
*   Linha inclinada passando pela origem

### **3\. Quando w = 0.5 e b = 1**

_f(x)=0.5⋅x+1f(x) = 0.5 \\cdot x + 1_f(x)=0.5⋅x+1

*   Mesmo inclinação
*   Agora sobe 1 unidade quando x = 0 (novo intercepto)

# **O Problema: Como escolher os melhores w e b?**

Queremos uma linha que passe **próxima dos pontos do conjunto de treinamento**.

Para cada exemplo _(x(i),y(i))(x^{(i)}, y^{(i)})_(x(i),y(i)), o modelo prevê:

## **Previsão:**

_y^(i)=fw,b(x(i))=w⋅x(i)+b\\hat{y}^{(i)} = f\_{w,b}(x^{(i)}) = w \\cdot x^{(i)} + b_y^ (i)=fw,b (x(i))=w⋅x(i)+b

Mas como quantificar “estar próximo dos dados”?

Precisamos medir:

*   A distância entre a previsão _y^(i)\\hat{y}^{(i)}_y^ (i)
*   E o valor real _y(i)y^{(i)}_y(i)

# **Medindo Erro: Diferença entre previsão e alvo**

Para cada exemplo:

_erro(i)=y^(i)−y(i)\\text{erro}^{(i)} = \\hat{y}^{(i)} - y^{(i)}_erro(i)=y^ (i)−y(i)

Para evitar que erros positivos e negativos se anulem, elevamos ao quadrado:

## **Erro quadrático por exemplo:**

_(y^(i)−y(i))2\\left( \\hat{y}^{(i)} - y^{(i)} \\right)^2_(y^ (i)−y(i))2

# **Erro em Todo o Conjunto de Treinamento**

Se temos **m** exemplos de treinamento, somamos todos os erros quadráticos:

_∑i=1m(y^(i)−y(i))2\\sum\_{i=1}^{m} \\left( \\hat{y}^{(i)} - y^{(i)} \\right)^2_i=1∑m (y^ (i)−y(i))2

Mas este valor cresce conforme m aumenta, então usamos a **média**:

## **Erro quadrático médio (MSE):**

_1m∑i=1m(y^(i)−y(i))2\\frac{1}{m} \\sum\_{i=1}^{m} \\left( \\hat{y}^{(i)} - y^{(i)} \\right)^2_m1 i=1∑m (y^ (i)−y(i))2

# **Definição Final: Função de Custo da Regressão Linear**

Por convenção matemática, incluímos um fator adicional _12\\frac{1}{2}_21 para simplificar as derivadas no cálculo do gradiente:

## **Função de Custo J(w, b):**

_J(w,b)=12m∑i=1m(y^(i)−y(i))2J(w,b) = \\frac{1}{2m} \\sum\_{i=1}^{m} \\left( \\hat{y}^{(i)} - y^{(i)} \\right)^2_J(w,b)=2m1 i=1∑m (y^ (i)−y(i))2

Substituindo _y^(i)=fw,b(x(i))=wx(i)+b\\hat{y}^{(i)} = f\_{w,b}(x^{(i)}) = wx^{(i)} + b_y^ (i)=fw,b (x(i))=wx(i)+b:

_J(w,b)=12m∑i=1m(wx(i)+b−y(i))2J(w,b) = \\frac{1}{2m} \\sum\_{i=1}^{m} \\left( w x^{(i)} + b - y^{(i)} \\right)^2_J(w,b)=2m1 i=1∑m (wx(i)+b−y(i))2

# **Por que usamos essa função de custo?**

Porque ela mede, de forma matemática e objetiva:

*   Quão próximo o modelo está dos valores reais
*   Quão “boa” é a linha escolhida
*   Quanto o erro médio varia conforme ajustamos w e b

Valores importantes:

*   **J(w,b) alto** → linha ruim, erro grande
*   **J(w,b) baixo** → linha boa, modelo acertando

O objetivo do aprendizado é:

Encontrar os valores de w e b que minimizam J(w,b)

![]()

![]()

# **Intuição da Função de Custo**

## **Construindo Intuição para Encontrar os Melhores Parâmetros da Regressão Linear**

A função de custo é o elemento central que permite ao algoritmo ajustar seus parâmetros e aprender com os dados. Este vídeo aprofunda **a intuição por trás do cálculo do custo** e mostra como essa função nos orienta a escolher os melhores valores para **w** e **b**.

# **Revisão Rápida: O Modelo e os Parâmetros**

Na regressão linear simples, o modelo é:

_fw,b(x)=wx+bf\_{w,b}(x) = w x + b_fw,b (x)=wx+b

*   **w** controla a inclinação da linha
*   **b** desloca a linha para cima ou para baixo
*   Ajustar w e b muda completamente o alinhamento da linha com os dados

O objetivo é escolher valores para que a linha **se ajuste bem** aos dados do conjunto de treinamento.

# **Por Que Precisamos da Função de Custo?**

Para cada exemplo _(x(i),y(i))(x^{(i)}, y^{(i)})_(x(i),y(i)), o modelo faz uma previsão:

_y^(i)=fw,b(x(i))=wx(i)+b\\hat{y}^{(i)} = f\_{w,b}(x^{(i)}) = w x^{(i)} + b_y^ (i)=fw,b (x(i))=wx(i)+b

A função de custo quantifica **o quão longe** essas previsões estão dos valores reais.
O objetivo final é:

_min⁡w,b  J(w,b)\\min\_{w,b} \\; J(w,b)_w,bmin J(w,b)

Onde **J(w,b)** mede o erro médio de todas as previsões.

# **Simplificação para Criar Intuição**

Para facilitar a visualização, o vídeo simplifica o modelo ao **remover b**:

_fw(x)=wxf\_{w}(x) = w x_fw (x)=wx

Assim:

*   Só existe **um parâmetro a ajustar**, o w
*   A função de custo passa a ser:

_J(w)=12m∑i=1m(wx(i)−y(i))2J(w) = \\frac{1}{2m} \\sum\_{i=1}^{m} (w x^{(i)} - y^{(i)})^2_J(w)=2m1 i=1∑m (wx(i)−y(i))2

Essa simplificação permite visualizar a relação entre:

*   **a inclinação da linha** no gráfico da esquerda
*   **o valor do custo** no gráfico da direita

# **Construindo a Intuição: Dois Gráficos Lado a Lado**

O instrutor mostra dois gráficos simultâneos:

1.  **Gráfico à esquerda:**
    1.  Representa o modelo _fw(x)f\_w(x)_fw (x)
    2.  Eixo X = entrada x
    3.  Eixo Y = saída prevista
    4.  Mostra os pontos reais do treinamento e a linha gerada pelo modelo
2.  **Gráfico à direita:**
    1.  Representa a função de custo _J(w)J(w)_J(w)
    2.  Eixo X = possíveis valores de w
    3.  Eixo Y = custo resultante

Alterar w gera uma nova linha e um novo ponto correspondente em J(w).

# **Conjunto de Treinamento Usado no Exemplo**

Três pontos simples:

_(1,1),(2,2),(3,3)(1, 1), \\quad (2, 2), \\quad (3, 3)_(1,1),(2,2),(3,3)

Esse conjunto segue perfeitamente uma linha de inclinação 1, ideal para mostrar o comportamento do custo.

# **Caso 1: w = 1 → Ajuste Perfeito**

Linha:

_f(x)=1⋅xf(x) = 1 \\cdot x_f(x)=1⋅x

Para cada exemplo:

_y^(i)=y(i)\\hat{y}^{(i)} = y^{(i)}_y^ (i)=y(i)

Erro para todos os pontos:

_(wx(i)−y(i))=0⇒(wx(i)−y(i))2=0(w x^{(i)} - y^{(i)}) = 0 \\quad\\Rightarrow\\quad (w x^{(i)} - y^{(i)})^2 = 0_(wx(i)−y(i))=0⇒(wx(i)−y(i))2=0

Logo:

_J(1)=0J(1) = 0_J(1)=0

No gráfico da direita, o ponto (w = 1, J = 0) aparece como **o menor valor possível**.

# **Caso 2: w = 0.5 → Linha Inclinação Média**

Linha:

_f(x)=0.5xf(x) = 0.5x_f(x)=0.5x

Cálculo dos erros:

_Exemplo 1: (0.5−1)2=0.25Exemplo 2: (1−2)2=1Exemplo 3: (1.5−3)2=2.25\\begin{aligned} &\\text{Exemplo 1: } (0.5 - 1)^2 = 0.25_ [_\\\\_](file:///\\) _&\\text{Exemplo 2: } (1 - 2)^2 = 1_ [_\\\\_](file:///\\) _&\\text{Exemplo 3: } (1.5 - 3)^2 = 2.25_ [_\\\\_](file:///\\) _\\end{aligned}_ Exemplo 1: (0.5−1)2=0.25Exemplo 2: (1−2)2=1Exemplo 3: (1.5−3)2=2.25

Soma dos erros:

_0.25+1+2.25=3.50.25 + 1 + 2.25 = 3.5_0.25+1+2.25=3.5

Função de custo:

_J(0.5)=12m⋅3.5=3.56≈0.58J(0.5) = \\frac{1}{2m} \\cdot 3.5 = \\frac{3.5}{6} \\approx 0.58_J(0.5)=2m1 ⋅3.5=63.5 ≈0.58

No gráfico da direita surge o ponto:

_(w=0.5,  J=0.58)(w = 0.5, \\; J = 0.58)_(w=0.5,J=0.58)

# **Caso 3: w = 0 → Linha Horizontal no Eixo X**

Linha:

_f(x)=0f(x) = 0_f(x)=0

Erros:

_12=122=432=9\\begin{aligned} &1^2 = 1_ [_\\\\_](file:///\\) _&2^2 = 4_ [_\\\\_](file:///\\) _&3^2 = 9 \\end{aligned}_ 12=122=432=9

Soma:

_1+4+9=141 + 4 + 9 = 14_1+4+9=14

Função de custo:

_J(0)=146≈2.33J(0) = \\frac{14}{6} \\approx 2.33_J(0)=614 ≈2.33

Esse ponto é muito mais alto no gráfico da direita.

# **Caso 4: w = -0.5 → Linha Descendente**

Linha inclina para baixo.
Erros aumentam ainda mais.

Resultado:

_J(−0.5)≈5.25J(-0.5) \\approx 5.25_J(−0.5)≈5.25

E o ponto aparece ainda mais alto no gráfico da direita.

# **O Formato da Função de Custo**

Ao calcular J(w) para vários valores de w, surge um gráfico em forma de **curva convexa** (formato de tigela).
Isso representa:

*   Um único ponto mínimo
*   Que corresponde à melhor inclinação possível

Nesse exemplo:

_w=1w = 1_w=1

Esse valor gera:

*   A menor perda possível
*   A melhor linha de regressão possível

# **Relação Direta Entre f(x) e J(w)**

**Valor de w**

**Linha f(x)**

**Custo J(w)**

**Qualidade do ajuste**

\-0.5

muito ruim

alto

péssima

0

ruim

alto

ruim

0.5

moderado

médio

ok

**1.0**

**perfeita**

**mínimo**

**ideal**

Mudou **w** → mudaram:

*   a linha no gráfico da esquerda
*   o ponto correspondente no gráfico da direita

# **Objetivo do Aprendizado**

_min⁡wJ(w)\\min\_w J(w)_wmin J(w)

No caso completo:

_min⁡w,bJ(w,b)\\min\_{w,b} J(w,b)_w,bmin J(w,b)

Minimizar J significa reduzir o erro quadrático médio e obter uma linha que melhor se aproxima dos pontos reais.

# **Conclusão da Intuição**

*   A função de custo serve como **bússola** do aprendizado:
    ela indica quando os parâmetros estão bons ou ruins.
*   Avaliar J(w) para muitos valores mostra uma curva com mínimo global.
*   O melhor w é aquele que produz o menor valor de J.

![]()

![]()

![]()

![]()

# **Visualização da Função de Custo**

## **Como enxergar J(w, b) em 2D, 3D e entender sua forma geométrica**

A função de custo _J(w,b)J(w, b)_J(w,b) é o elemento central que orienta o algoritmo durante o treinamento.
Este vídeo aprofunda a **visualização geométrica** dessa função para construir uma intuição sólida sobre como o modelo encontra os melhores parâmetros.

# **1\. Retomando o Cenário**

Em regressão linear, usamos o modelo:

_fw,b(x)=wx+bf\_{w,b}(x) = w x + b_fw,b (x)=wx+b

Com:

*   **w** = inclinação
*   **b** = intercepto
*   **J(w,b)** = função de custo (erro quadrático médio)

O objetivo é:

_min⁡w,bJ(w,b)\\min\_{w,b} J(w,b)_w,bmin J(w,b)

No vídeo anterior, simplificamos o modelo definindo **b = 0**, permitindo visualizar J(w) como uma curva em U.
Agora voltamos ao cenário completo: **dois parâmetros**, portanto uma função de custo que deve ser visualizada em **3D**.

# **2\. Visualizando f(x) e J(w, b) Lado a Lado**

Assim como no vídeo anterior, temos dois gráficos simultâneos:

### **À esquerda — o modelo linear**

Mostra:

*   dados reais (tamanho da casa × preço)
*   a linha gerada pelo modelo _fw,b(x)f\_{w,b}(x)_fw,b (x) para um par w, b

### **À direita — a função de custo**

Agora já não é mais uma curva, mas uma **superfície 3D** em função dos dois parâmetros:

*   eixo X → w
*   eixo Y → b
*   eixo Z → J(w,b)

# **3\. Avaliando um Modelo Específico (exemplo ilustrado)**

O vídeo mostra a escolha de:

_w=0.06,b=50w = 0.06, \\quad b = 50_w=0.06,b=50

O modelo correspondente:

_f(x)=0.06x+50f(x) = 0.06x + 50_f(x)=0.06x+50

Visualmente, esta linha:

*   subestima os preços em quase todos os pontos
*   está deslocada para baixo
*   tem inclinação insuficiente

Consequentemente, a função de custo _J(w,b)J(w,b)_J(w,b) para esses valores é relativamente alta.

# **4\. A Função de Custo em 3D: A "Tigela de Sopa"**

Quando tínhamos apenas **um parâmetro**, a função J(w) era:

→ uma curva convexa em formato de U.

Agora, com **dois parâmetros (w e b)**, J(w,b) se torna:

→ uma superfície convexa em formato de **tigela de sopa**
→ ou uma “rede” curvada (como mostrado nas imagens do vídeo)

Essa superfície apresenta:

*   um **único vale global**
*   nenhum mínimo local
*   um ponto onde J é **mínimo** → esse é o melhor par (w, b)

Se o conjunto de dados mudar, o formato pode alongar, achatar ou inclinar, mas continua sendo uma “tigela convexa”.

# **5\. Como ler a superfície J(w,b)**

Cada ponto da superfície 3D representa:

_(w,  b,  J(w,b))\\bigl(w,\\; b,\\; J(w,b)\\bigr)_(w,b,J(w,b))

Por exemplo:

*   Se _(w=−10,b=−15)(w=-10, b=-15)_(w=−10,b=−15), o valor da altura no gráfico mostra quanto é J para essa escolha.
*   Cada ponto corresponde a uma linha diferente sendo tentada pelo modelo.

Quanto **mais alto** o ponto na superfície, **pior** é o ajuste do modelo.

Quanto **mais baixo**, **melhor**.

# **6\. Gráfico de Contorno (Contour Plot)**

Para facilitar a visualização, o vídeo converte a superfície 3D em **curvas de nível**, análogas a:

*   mapas topográficos
*   mapas de montanhas (ex: Monte Fuji)

Cada linha no gráfico de contorno representa:

_{(w,b)∣J(w,b)=constante}\\{(w, b) \\mid J(w,b) = \\text{constante}\\}_{(w,b)∣J(w,b)=constante}

Ou seja:

*   todas as combinações de w e b que resultam **no mesmo valor de custo**
*   círculos/ovais concêntricos
*   centro das elipses = **ponto de menor custo**, o fundo da tigela
*   elipses externas = valores mais altos de J

### **Intuição visual:**

*   É como olhar a tigela **de cima**.
*   O local onde as elipses são menores é o **mínimo global**.

# **7\. Relação entre Contornos e Modelos f(x)**

Ao selecionar três pares diferentes _(w,b)(w, b)_(w,b):

*   cada par gera uma linha diferente no gráfico da esquerda
*   cada par cai em um ponto diferente no gráfico de contorno
*   mesmo que os modelos sejam ruim (como no exemplo), eles podem aparecer na **mesma elipse**
    → ou seja, têm **o mesmo valor de custo**, mesmo que gerem previsões diferentes

Isso mostra:

*   a função de custo não mede simplesmente a visualização da linha
*   ela apenas mede o **erro quadrático médio global**

# **8\. Por Que o Gráfico de Contorno é Tão Importante?**

Porque:

*   É mais fácil visualizar trajetórias de otimização (como no gradiente descendente)
*   Permite entender como w e b “caminham” em direção ao mínimo
*   Em modelos com muitos parâmetros, esse raciocínio se generaliza

![]()

# **Exemplos de Visualização da Função de Custo**

## **Explorando escolhas de w e b e seus efeitos no modelo e no custo J(w, b)**

Este vídeo aprofunda o entendimento de como diferentes valores de **w** e **b** influenciam:

1.  A linha do modelo _fw,b(x)f\_{w,b}(x)_fw,b (x)
2.  O erro das previsões
3.  O valor da função de custo _J(w,b)J(w,b)_J(w,b)
4.  A posição do ponto (w, b) nos gráficos de superfície e contorno

O objetivo é desenvolver **intuição geométrica** sobre como o modelo interage com o espaço de parâmetros.

# **1\. Exemplo 1: Parâmetros muito ruins**

### **Parâmetros escolhidos:**

_w=−0.15,b≈800w = -0.15, \\quad b \\approx 800_w=−0.15,b≈800

### **Modelo resultante:**

_f(x)=−0.15x+800f(x) = -0.15x + 800_f(x)=−0.15x+800

### **Características do modelo:**

*   Cruzamento com o eixo y em **800**
*   Linha com **inclinação negativa**
*   Visualmente incompatível com a tendência crescente dos preços das casas
*   Previsões muito distantes dos valores reais

### **Consequência no custo:**

*   O ponto correspondente no gráfico de J(w,b) está **distante do vale/mínimo**
*   Custo elevado:

_J(w,b)≫Jmin⁡J(w,b) \\gg J\_{\\min}_J(w,b)≫Jmin

Esse exemplo mostra como uma combinação claramente inadequada de w e b produz tanto uma linha ruim quanto um custo alto.

# **2\. Exemplo 2: Um modelo ainda ruim, mas menos inadequado**

### **Parâmetros escolhidos:**

_w=0,b≈360w = 0, \\quad b \\approx 360_w=0,b≈360

### **Modelo resultante:**

_f(x)=0x+360=360f(x) = 0x + 360 = 360_f(x)=0x+360=360

Linha **horizontal**.
Não ajusta a tendência dos dados, mas é menos absurda que o exemplo anterior.

### **Consequência:**

*   O ponto no gráfico de contorno está **mais próximo** do centro das elipses
*   Porém, ainda longe do mínimo real

### **Intuição:**

*   Mesmo “um pouco melhor” ainda gera custos altos
*   Isso evidencia como pequenas mudanças em w e b movem o ponto no gráfico de custo

# **3\. Exemplo 3: Outro modelo ruim, ainda distante do ótimo**

Outro par de valores é analisado (não especificado no vídeo), mas seu efeito visual mostra:

*   Linha bastante desalinhada com os dados
*   Custo até **maior** do que no exemplo anterior
*   Ponto no gráfico de contorno **mais afastado** do centro

### **Intuição construída:**

Quanto mais distante a linha está dos pontos no gráfico de dados, mais longe o ponto (w, b) está do centro das elipses em J(w,b).

# **4\. Exemplo 4: Um modelo que se ajusta bem aos dados**

### **Parâmetros escolhidos:**

Valores próximos aos ideais (o vídeo não fornece valores exatos).

### **Modelo resultante:**

*   Linha que passa **muito próxima** de grande parte dos pontos
*   Pequenas distâncias verticais entre _yiy^i_yi e _y^i\\hat{y}^i_y^ i

### **Relação com o custo:**

*   O ponto correspondente no gráfico de contorno está **quase no centro da menor elipse**
*   Portanto:

_J(w,b)≈Jmin⁡J(w,b) \\approx J\_{\\min}_J(w,b)≈Jmin

### **Interpretação geométrica:**

*   A soma dos erros quadráticos

_∑i=1m(fw,b(xi)−yi)2\\sum\_{i=1}^m (f\_{w,b}(x^i) - y^i)^2_i=1∑m (fw,b (xi)−yi)2

é quase mínima

*   O modelo está próximo do melhor ajuste possível no formato linear

# **5\. Ligação entre f(x) e J(w,b)**

Para cada combinação de (w, b):

1.  Obtemos uma linha diferente
2.  Geramos previsões _y^i\\hat{y}^i_y^ i diferentes
3.  Calculamos erros individuais

_erroi=y^i−yi\\text{erro}\_i = \\hat{y}^i - y^i_erroi =y^ i−yi

1.  O custo final se torna:

_J(w,b)=12m∑i=1m(fw,b(xi)−yi)2J(w,b) = \\frac{1}{2m}\\sum\_{i=1}^{m}(f\_{w,b}(x^i)-y^i)^2_J(w,b)=2m1 i=1∑m (fw,b (xi)−yi)2

Quanto mais perto a linha fica dos pontos, menor é o custo e mais próximo o ponto (w, b) está do centro das elipses no gráfico.

# **6\. Interatividade no laboratório (descrição do vídeo)**

No laboratório opcional você poderá:

### **1\. Clicar no gráfico de contorno**

*   Cada clique define um par (w, b)
*   A linha correspondente aparece imediatamente no gráfico dos dados
*   Um ponto aparece também na superfície 3D mostrando o custo

### **2\. Girar a superfície 3D**

*   Permite enxergar a “tigela de sopa” por vários ângulos
*   Você pode observar como pequenas variações em w e b sobem ou descem a superfície

Essa exploração ajuda a fixar a relação:

_linha ruim→J alto\\text{linha ruim} \\rightarrow J \\text{ alto}_ linha ruim→J alto _linha boa→J baixo\\text{linha boa} \\rightarrow J \\text{ baixo}_linha boa→J baixo

# **7\. Motivação para o Próximo Tema: Precisamos de um algoritmo**

O vídeo conclui apontando que:

*   Escolher w e b manualmente observando gráficos é inviável
*   Especialmente em modelos mais complexos, com dezenas ou milhões de parâmetros
*   É necessário um **algoritmo matemático efetivo** que:
    *   Tome decisões iterativas
    *   Caminhe automaticamente rumo ao mínimo
    *   Funcione em alta dimensão
    *   Seja eficiente computacionalmente

Esse algoritmo é:

Gradiente Descendente

![]()

![]()

![]()

# **Descida de Gradiente**

## **Intuição, funcionamento e relação com a minimização da função de custo**

A descida de gradiente é o algoritmo padrão para minimizar funções de custo em aprendizado de máquina. Ele é usado desde modelos simples, como regressão linear, até modelos extremamente complexos, como redes neurais profundas.

# **1\. Objetivo da descida de gradiente**

O objetivo é **encontrar os valores dos parâmetros** _ww_w e _bb_b que **minimizam a função de custo**:

_min⁡w,bJ(w,b)\\min\_{w, b} J(w, b)_w,bmin J(w,b)

Inicialmente, escolhem-se valores arbitrários (comum usar 0):

_w=0,b=0w = 0, \\quad b = 0_w=0,b=0

Depois, esses valores são iterativamente ajustados até que o custo atinja um mínimo.

# **2\. Generalidade do algoritmo**

Embora aqui seja aplicado na regressão linear, o algoritmo funciona para:

*   Funções de custo com **muitos parâmetros**:

_J(w1,w2,…,wn,b)J(w\_1, w\_2,\\ldots, w\_n, b)_J(w1 ,w2 ,…,wn ,b)

*   Modelos como redes neurais, onde há **centenas ou milhões** de parâmetros
*   Qualquer função diferenciável que se deseje minimizar

A descida de gradiente é universal nesse sentido.

# **3\. Intuição geométrica: movimento sobre um terreno**

O vídeo usa uma analogia visual: imagine que a função de custo é um **terreno tridimensional**, onde:

*   Pontos altos = custo alto
*   Pontos baixos = custo baixo
*   O mínimo da função = fundo de um vale

Você “está” em um ponto da superfície (um par _w,bw, b_w,b).
O objetivo é **descer** até o ponto mais baixo possível.

### **Ideia central:**

A cada etapa, você olha ao redor em todas as direções (360°) e identifica:

Em qual direção a descida é mais íngreme?

Essa direção é determinada matematicamente pelo **gradiente**.

# **4\. A regra de atualização do gradiente descendente**

Para cada iteração:

_w:=w−α ∂J(w,b)∂ww := w - \\alpha \\, \\frac{\\partial J(w,b)}{\\partial w}_w:=w−α∂w∂J(w,b) _b:=b−α ∂J(w,b)∂bb := b - \\alpha \\, \\frac{\\partial J(w,b)}{\\partial b}_b:=b−α∂b∂J(w,b)

Onde:

*   _α\\alpha_α = taxa de aprendizado (learning rate)
*   O gradiente _(∂J∂w,∂J∂b)\\left( \\frac{\\partial J}{\\partial w}, \\frac{\\partial J}{\\partial b} \\right)_(∂w∂J ,∂b∂J ) aponta para a direção de **subida mais íngreme**
*   O algoritmo move-se na **direção oposta** para descer

# **5\. Caminho percorrido pelo gradiente descendente**

O processo segue:

1.  Começa em um ponto inicial (ex.: _w=0w=0_w=0, _b=0b=0_b=0)
2.  Calcula o gradiente
3.  Move-se um pouco na direção da maior descida
4.  Repete até os valores mudarem muito pouco

No gráfico de contorno, isso aparece como um caminho de pontos convergindo para o centro das elipses.

# **6\. Mínimos locais e comportamento do algoritmo**

Quando a função de custo tem forma simples, como na regressão linear:

*   A superfície de _J(w,b)J(w, b)_J(w,b) é uma tigela convexa
*   Existe **um único mínimo global**
*   O gradiente sempre converge corretamente

Mas para funções mais complexas, como redes neurais:

*   A superfície pode ter **vários vales**
*   Dependendo do ponto inicial, o gradiente pode chegar a diferentes mínimos

### **Representação visual do vídeo:**

*   Começa-se em um ponto da colina
*   Dá-se um passo na direção de maior descida
*   Repete até chegar ao fundo de um vale
*   Começar em outro ponto pode levar a outro vale diferente

Isso explica por que modelos profundos podem encontrar soluções diferentes ao treinar com inicializações distintas.

# **7\. Termos importantes**

**Conceito**

**Descrição**

**Gradiente**

Vetor que aponta para a direção onde o custo cresce mais rápido

**Descida mais íngreme**

Direção oposta ao gradiente

**Taxa de aprendizado (α)**

Tamanho do passo dado em cada atualização

**Mínimo local**

Vale em que o algoritmo pode ficar preso em funções complexas

**Mínimo global**

Menor valor possível de toda a função

# **8\. Relação com regressão linear**

Embora no vídeo use-se como exemplo uma função complexa, na regressão linear a superfície é sempre convexa:

*   Apenas **um vale**
*   Não há mínimos locais
*   O gradiente descendente sempre converge para a solução exata (se α não for muito grande)

![]()

# **Implementação da Descida de Gradiente**

## **Como o algoritmo funciona e como implementá-lo corretamente**

A descida de gradiente é o algoritmo usado para ajustar iterativamente os parâmetros de um modelo (como _ww_w e _bb_b na regressão linear), reduzindo progressivamente a função de custo _J(w,b)J(w, b)_J(w,b). Esta seção explica a atualização passo a passo, o papel da taxa de aprendizado e como implementar corretamente o algoritmo no código.

# **1\. Fórmula geral do gradiente descendente**

Para cada parâmetro do modelo, executa-se uma atualização:

_w:=w−α ∂J(w,b)∂ww := w - \\alpha \\, \\frac{\\partial J(w,b)}{\\partial w}_w:=w−α∂w∂J(w,b) _b:=b−α ∂J(w,b)∂bb := b - \\alpha \\, \\frac{\\partial J(w,b)}{\\partial b}_b:=b−α∂b∂J(w,b)

Onde:

*   _α\\alpha_α = taxa de aprendizado
*   _∂J∂w\\frac{\\partial J}{\\partial w}_∂w∂J e _∂J∂b\\frac{\\partial J}{\\partial b}_∂b∂J = derivadas parciais (gradientes)
*   A expressão indica:
    **novo valor = valor antigo – passo na direção da descida**

# **2\. Entendendo a notação**

## **2.1 Operador de atribuição ( = )**

No contexto do algoritmo, o **\=** não é uma igualdade matemática; é um **operador de atribuição**, equivalente ao código:

a = c # armazena o valor de c dentro de a
a = a + 1 # incrementa a

Diferente de uma afirmação matemática como:

_a=c(declarac¸a˜o de igualdade)a = c \\quad (\\text{declaração de igualdade})_a=c(declarac¸ a˜o de igualdade)

Ou de uma comparação em Python:

a == c # teste lógico

# **3\. A taxa de aprendizado (α)**

O parâmetro _α\\alpha_α controla **o tamanho dos passos** na direção da descida:

*   Se α for **muito grande** → passos longos, risco de ultrapassar o mínimo
*   Se α for **muito pequeno** → passos diminutos, convergência muito lenta
*   Tipicamente é um número entre **0 e 1**, como 0,01 ou 0,001

Mais adiante, o curso discute como escolher uma boa taxa de aprendizado.

# **4\. O termo derivado (o gradiente)**

O termo:

_∂J∂w,∂J∂b\\frac{\\partial J}{\\partial w}, \\quad \\frac{\\partial J}{\\partial b}_∂w∂J ,∂b∂J

Indica **em qual direção o custo cresce mais rapidamente**.
O gradiente descendente faz exatamente o oposto: move-se na **direção de menor crescimento**, ou seja, a mais íngreme descida.

Para entender intuitivamente:

*   Esse termo especifica **para onde o parâmetro deve ir**
*   _α\\alpha_α controla **quanto** ele deve ir

Mesmo sem conhecer cálculo, o curso explicará como obter essas derivadas para regressão linear.

# **5\. Atualização de ambos os parâmetros**

## **Por que a atualização deve ser _simultânea_**

Na regressão linear temos dois parâmetros:

*   _ww_w
*   _bb_b

Ambos influenciam a função de custo.
Durante o gradiente descendente, **os dois devem ser atualizados ao mesmo tempo**, usando seus valores _originais_ da iteração anterior.

# **6\. Atualização simultânea (correta)**

Exemplo do algoritmo correto:

temp\_w = w - α \* dJ\_dw
temp\_b = b - α \* dJ\_db
w = temp\_w
b = temp\_b

Ambos os termos à direita usam **o w e o b anteriores** para calcular os novos valores.

Isto é equivalente ao que Andrew Ng chama de "_simultaneous update_".

# **7\. Atualização não simultânea (incorreta)**

A implementação errada é esta:

temp\_w = w - α \* dJ\_dw
w = temp\_w # <-- atualizado antes da hora
temp\_b = b - α \* dJ\_db # <-- calcula usando w já modificado
b = temp\_b

Por que está errado?

*   O cálculo de _tempbtemp\_b_tempb usa um **valor de w já alterado**
*   Isso altera a direção do passo
*   O algoritmo deixa de ser gradiente descendente puro
*   Pode resultar em comportamento diferente, inclusive divergência

Essa versão ainda funciona “mais ou menos” para alguns casos simples, mas **não é o algoritmo correto**.

# **8\. Processo completo do gradiente descendente**

1.  Inicialize:

_w=0,b=0w = 0,\\quad b = 0_w=0,b=0

1.  Repita:
    1.  Calcule as derivadas:

_∂J∂w,∂J∂b\\frac{\\partial J}{\\partial w},\\quad \\frac{\\partial J}{\\partial b}_∂w∂J ,∂b∂J

*   1.  Atualize simultaneamente:

_w:=w−α∂J∂ww := w - \\alpha \\frac{\\partial J}{\\partial w}_w:=w−α∂w∂J _b:=b−α∂J∂bb := b - \\alpha \\frac{\\partial J}{\\partial b}_b:=b−α∂b∂J

1.  Continue até que:
    1.  as mudanças em _ww_w e _bb_b se tornem muito pequenas
    2.  ou o custo deixe de diminuir significativamente

Isso se chama **convergência**.

# **9\. Convergência do gradiente descendente**

Dizemos que o algoritmo convergiu quando:

*   _ww_w muda muito pouco entre iterações
*   _bb_b muda muito pouco
*   _J(w,b)J(w,b)_J(w,b) não está diminuindo de forma significativa
*   O ponto atual está muito próximo do mínimo local ou global

Para regressão linear, a função de custo é convexa (em forma de tigela).
Isso garante que **o algoritmo sempre encontra o mínimo global**, desde que α não seja muito grande.

![]()

# **Intuição da Descida de Gradiente**

## **Por que a fórmula funciona e como a derivada indica a direção correta**

A descida de gradiente adapta os parâmetros do modelo reduzindo progressivamente a função de custo. Para entender intuitivamente por que a atualização funciona, analisamos o que significam a derivada e a taxa de aprendizado em um caso simplificado com apenas **um parâmetro** _ww_w.

# **1\. Fórmula básica (caso de um parâmetro)**

A atualização fica:

_w:=w−αddwJ(w)w := w - \\alpha \\frac{d}{dw}J(w)_w:=w−αdwd J(w)

Onde:

*   _α\\alpha_α = taxa de aprendizado
*   _ddwJ(w)\\frac{d}{dw}J(w)_dwd J(w) = derivada (tecnicamente derivada parcial)
*   O objetivo é escolher novos valores de _ww_w que façam _J(w)J(w)_J(w) diminuir

# **2\. Interpretando a derivada**

## **2.1 Gráfico da função de custo**

Considere a função _J(w)J(w)_J(w):

*   eixo horizontal → _ww_w
*   eixo vertical → _J(w)J(w)_J(w)

A derivada no ponto _ww_w é a inclinação da linha tangente à curva.

# **3\. Caso 1: derivada positiva**

### **Quando _dJdw>0\\frac{dJ}{dw} > 0_dwdJ >0**

A linha tangente está inclinada **para cima**, como:

/
/
/

A derivada é positiva → indica que **aumentar w aumenta o custo**.

Atualização:

_wnovo=w−α⋅(positivo)w\_{\\text{novo}} = w - \\alpha \\cdot (\\text{positivo})_wnovo =w−α⋅(positivo)

Isso **reduz w**, movendo-o para a esquerda no gráfico — exatamente onde o custo está diminuindo.

**Conclusão:**
Se a derivada é positiva, o algoritmo move w para baixo do morro, reduzindo J.

# **4\. Caso 2: derivada negativa**

### **Quando _dJdw<0\\frac{dJ}{dw} < 0_dwdJ <0**

A tangente está inclinada **para baixo**, assim:

\\
\\
\\

A derivada é negativa → indica que **aumentar w diminui o custo**.

Atualização:

_wnovo=w−α⋅(negativo)w\_{\\text{novo}} = w - \\alpha \\cdot (\\text{negativo})_wnovo =w−α⋅(negativo)

Subtrair um número negativo significa adicionar:

_wnovo=w+α∣derivada∣w\_{\\text{novo}} = w + \\alpha |\\text{derivada}|_wnovo =w+α∣derivada∣

O valor de w aumenta — move-se para a direita, onde a curva desce até o mínimo.

**Conclusão:**
Se a derivada é negativa, o algoritmo aumenta w, novamente descendo a curva em direção ao mínimo.

# **5\. A lógica essencial**

A derivada responde à pergunta:

“Se eu der um passo pequeno para direita, o custo sobe ou desce?”

*   Derivada **positiva** → subiria → então dê o passo **para a esquerda**
*   Derivada **negativa** → desceria ampliando w → então dê o passo **para a direita**

Essa lógica gera um movimento contínuo “descendo a colina”, até chegar ao mínimo.

# **6\. Conexão com o caso real de dois parâmetros**

No caso completo da regressão linear:

_J(w,b)J(w,b)_J(w,b)

Temos dois gradientes:

_∂J∂w,∂J∂b\\frac{\\partial J}{\\partial w}, \\quad \\frac{\\partial J}{\\partial b}_∂w∂J ,∂b∂J

Cada um aponta para a direção em que o custo cresce mais rápido em cada eixo.
A descida de gradiente anda no sentido oposto desses vetores combinados.

# **7\. Papel da taxa de aprendizado (α)**

A taxa de aprendizado controla o **tamanho do passo**:

*   α grande → passos longos (rápido, mas arriscado)
*   α pequeno → passos curtos (lento, mas seguro)

A combinação:

_α⋅dJdw\\alpha \\cdot \\frac{dJ}{dw}_α⋅dwdJ

determina quão grande será o movimento em direção ao mínimo.

# **8\. Resumo visual**

### **Derivada positiva → mover w para a esquerda**

### **Derivada negativa → mover w para a direita**

Sempre reduzindo _JJ_J.

![]()

![]()

# **Taxa de Aprendizado (α)**

## **Como ela afeta o comportamento da descida de gradiente**

A taxa de aprendizado _α\\alpha_α controla o tamanho do passo que o algoritmo dá ao atualizar os parâmetros. A escolha desse valor determina se o gradiente descendente será:

*   lento
*   eficiente
*   instável
*   ou incapaz de convergir

# **1\. Regra geral da atualização**

A descida de gradiente atualiza cada parâmetro assim:

_w:=w−α∂J(w)∂ww := w - \\alpha \\frac{\\partial J(w)}{\\partial w}_w:=w−α∂w∂J(w)

E de forma análoga para _bb_b:

_b:=b−α∂J(w,b)∂bb := b - \\alpha \\frac{\\partial J(w,b)}{\\partial b}_b:=b−α∂b∂J(w,b)

# **2\. O que acontece quando α é muito pequeno?**

## **2.1 Movimento extremamente lento**

Com _α\\alpha_α pequeno (ex.: _0.00000010.0000001_0.0000001), cada etapa multiplica a derivada por um número minúsculo:

_Δw=−α⋅dJdw≈0\\Delta w = -\\alpha \\cdot \\frac{dJ}{dw} \\approx 0_Δw=−α⋅dwdJ ≈0

Isso faz com que:

*   cada passo seja muito pequeno
*   o algoritmo avance de maneira quase imperceptível
*   sejam necessárias milhares ou milhões de iterações para chegar perto do mínimo

### **Visualização mental**

*   A curva _J(w)J(w)_J(w) está à sua frente
*   Você está descendo a colina em **passos de formiga**
*   A direção está correta, mas a velocidade é extremamente lenta

**Conclusão:**
α muito pequeno = convergência correta, porém dolorosamente lenta.

# **3\. O que acontece quando α é muito grande?**

## **3.1 Passos longos que “pulam” o mínimo**

Se α for muito grande, os passos ficam exagerados:

_Δw=−α⋅dJdw(α grande → passo enorme)\\Delta w = -\\alpha \\cdot \\frac{dJ}{dw} \\quad \\text{(α grande → passo enorme)}_Δw=−α⋅dwdJ (α grande → passo enorme)

Isso causa:

*   saltos de um lado ao outro do mínimo
*   valores de _JJ_J piorando ao invés de melhorar
*   comportamento divergente

### **Exemplo visual**

1.  Você está perto do mínimo
2.  O gradiente indica “vá para a direita”
3.  α alto → você dá um passo tão grande que passa direto do mínimo
4.  No novo ponto, a derivada aponta para a esquerda
5.  α ainda grande → novo passo enorme que passa direto de novo
6.  O algoritmo fica “oscilando” e se afastando do mínimo

**Conclusão:**
α muito grande = o modelo não converge e pode divergir.

# **4\. O que acontece se você já estiver exatamente no mínimo?**

Suponha que:

*   _w=w\\\*w = w^{\\\*}_w=w\\\*
*   E esse valor está em um mínimo local

Então, nesse ponto:

_dJdw=0\\frac{dJ}{dw} = 0_dwdJ =0

Substituindo na regra de atualização:

_w:=w−α⋅0=ww := w - \\alpha \\cdot 0 = w_w:=w−α⋅0=w

Ou seja:

*   **nenhuma mudança ocorre**
*   o algoritmo permanece no mínimo
*   não importa o valor de α (desde que seja finito)

Isso explica por que a descida de gradiente **estaciona naturalmente** no mínimo, mesmo com taxa de aprendizado fixa.

# **5\. Por que os passos diminuem automaticamente perto do mínimo?**

Mesmo com uma taxa de aprendizado constante _α\\alpha_α, o tamanho do passo é:

_Δw=−α⋅dJdw\\Delta w = -\\alpha \\cdot \\frac{dJ}{dw}_Δw=−α⋅dwdJ

À medida que você se aproxima do mínimo:

*   a derivada diminui
*   o gradiente tende a zero
*   portanto os passos se tornam naturalmente menores

Isso cria o efeito:

*   **passos grandes quando longe do mínimo**
*   **passos pequenos quando perto do mínimo**

Esse comportamento faz parte da estabilidade do gradiente descendente.

# **6\. Resumo visual**

### **α muito pequeno**

*   passos minúsculos
*   convergência lenta
*   algoritmo funciona, mas pode demorar demais

### **α adequado**

*   passos proporcionais
*   convergência rápida e estável

### **α muito grande**

*   saltos exagerados
*   J aumenta ao invés de diminuir
*   algoritmo diverge ou oscila

### **No mínimo (derivada = 0)**

*   passo = 0
*   algoritmo permanece parado

# **7\. Conclusão**

A taxa de aprendizado:

*   controla o tamanho dos passos na descida da função de custo
*   determina se o algoritmo será eficiente ou instável
*   deve ser escolhida cuidadosamente para garantir convergência

![]()

![]()

![]()

# **Descida de Gradiente para Regressão Linear**

## **Como unir modelo, função de custo e gradiente descendente**

Neste capítulo, combinamos:

*   o **modelo de regressão linear**,
*   a **função de custo de erro quadrático (MSE)**,
*   e o **algoritmo de descida de gradiente**,

para treinar um modelo capaz de ajustar uma **reta** aos dados.

# **1\. Modelo de Regressão Linear**

O modelo previsto é:

_fw,b(x)=wx+bf\_{w,b}(x) = wx + b_fw,b (x)=wx+b

Onde:

*   **w** define a inclinação da reta
*   **b** define o deslocamento vertical (intercepto)

# **2\. Função de custo (erro quadrático)**

O custo mede o quão bem o modelo se ajusta aos dados:

_J(w,b)=12m∑i=1m(fw,b(x(i))−y(i))2J(w,b) = \\frac{1}{2m} \\sum\_{i=1}^m \\left(f\_{w,b}(x^{(i)}) - y^{(i)}\\right)^2_J(w,b)=2m1 i=1∑m (fw,b (x(i))−y(i))2

O fator **1/(2m)** facilita a derivação, pois o 2 cancela ao aplicar o cálculo diferencial.

# **3\. Derivadas necessárias para o gradiente descendente**

Para aplicar o gradiente descendente, precisamos das derivadas parciais de J:

### **3.1 Derivada em relação a w**

_∂J(w,b)∂w=1m∑i=1m(fw,b(x(i))−y(i))x(i)\\frac{\\partial J(w,b)}{\\partial w} = \\frac{1}{m} \\sum\_{i=1}^{m} \\left(f\_{w,b}(x^{(i)}) - y^{(i)}\\right) x^{(i)}_∂w∂J(w,b) =m1 i=1∑m (fw,b (x(i))−y(i))x(i)

### **3.2 Derivada em relação a b**

_∂J(w,b)∂b=1m∑i=1m(fw,b(x(i))−y(i))\\frac{\\partial J(w,b)}{\\partial b} = \\frac{1}{m} \\sum\_{i=1}^{m} \\left(f\_{w,b}(x^{(i)}) - y^{(i)}\\right)_∂b∂J(w,b) =m1 i=1∑m (fw,b (x(i))−y(i))

Observe:

*   a derivada de **w** inclui o termo _x(i)x^{(i)}_x(i)
*   a derivada de **b** não possui esse termo, pois b não depende de x

# **4\. De onde vêm essas fórmulas? (Resumo da derivação)**

**Opcional**, mas útil para entender o mecanismo:

1.  Substituímos a função de custo:

_J=12m∑(wx+b−y)2J = \\frac{1}{2m}\\sum (wx+b - y)^2_J=2m1 ∑(wx+b−y)2

1.  Aplicamos regras básicas de cálculo (cadeia, soma e potência):

*   O expoente 2 cancela com o denominador 2
*   Derivamos o termo interno
*   Obtemos os termos lineares acima

Esse é o motivo de adotarmos o fator **1/2m**: ele simplifica a matemática.

# **5\. Algoritmo de Descida de Gradiente Completo**

A atualização simultânea dos parâmetros é:

_w:=w−α∂J∂ww := w - \\alpha \\frac{\\partial J}{\\partial w}_w:=w−α∂w∂J _b:=b−α∂J∂bb := b - \\alpha \\frac{\\partial J}{\\partial b}_b:=b−α∂b∂J

Onde:

*   **α** = taxa de aprendizado
*   Os parâmetros são atualizados **juntos** a cada iteração

# **6\. Processo de treinamento**

O algoritmo executa repetidamente:

1.  **Calcula as previsões** _fw,b(x(i))f\_{w,b}(x^{(i)})_fw,b (x(i))
2.  **Calcula os erros** _(y^−y)(\\hat{y}-y)_(y^ −y)
3.  **Usa as derivadas** para ajustar w e b
4.  **Recalcula o custo**
5.  **Repete até convergir**

Convergência = quando as mudanças em w e b ficam muito pequenas.

# **7\. O problema dos mínimos locais**

## **Por que regressão linear não sofre com isso**

Em muitos modelos (como redes neurais), a superfície do custo pode ter:

*   múltiplos vales (mínimos locais)
*   áreas que “aprisionam” o algoritmo dependendo do ponto inicial

Porém, na regressão linear usando o custo quadrático, a superfície é sempre:

*   **convexa**
*   **em forma de tigela**
*   com **um único mínimo global**

Isso significa:

### **Propriedade fundamental:**

“Para regressão linear + MSE, o gradiente descendente sempre converge ao mesmo mínimo global, desde que α seja razoável.”

Não importa onde w e b começam:
eles sempre caminham para o fundo da tigela.

# **8\. Por que a função de custo é convexa?**

Porque ela é a soma de termos quadráticos:

_(wx+b−y)2(wx+b - y)^2_(wx+b−y)2

Funções quadráticas são convexas e não podem ter múltiplos mínimos locais.

Isso garante que:

*   não existe perigo de cair no “vale errado”
*   todo caminho leva ao mínimo global
*   o modelo é matematicamente estável

# **9\. Conclusão**

A combinação:

*   regressão linear
*   função de custo quadrático
*   derivadas fechadas e simples
*   descida de gradiente

forma um algoritmo altamente eficiente, estável e previsível.

Você agora tem todos os passos necessários para:

*   implementar a regressão linear do zero
*   entender a teoria por trás do aprendizado
*   aplicar gradiente descendente de maneira correta e segura

![]()

![]()

![]()

# **Execução da Descida do Gradiente**

## **Visualizando o processo em regressão linear**

Neste módulo, acompanhamos passo a passo o que acontece quando executamos a descida de gradiente no contexto da **regressão linear**. A ideia é visualizar como os parâmetros **w** e **b** são ajustados a cada iteração e como o modelo evolui até encontrar o **mínimo global** da função de custo.

# **1\. Cenário da demonstração**

A demonstração utiliza três visualizações simultâneas:

1.  **Gráfico do modelo com os dados** (parte superior esquerda)
    Mostra a linha de regressão atual sobre os pontos reais.
2.  **Gráfico de contorno da função de custo** (parte superior direita)
    Representa as curvas de nível da superfície de J(w, b).
3.  **Gráfico de superfície** (parte inferior)
    Mostra a forma 3D da função de custo — uma “tigela” convexa.

Para iniciar, w e b são definidos manualmente com os valores:

*   **w = –0,1**
*   **b = 900**

O modelo inicial é:

_f(x)=−0,1x+900f(x) = -0{,}1x + 900_f(x)=−0,1x+900

# **2\. Primeiras atualizações do gradiente**

Com esses valores, fazemos a primeira iteração do gradiente descendente:

*   No gráfico da função de custo, o ponto atual (w, b) se move para **baixo e à direita**.
*   A linha de regressão no gráfico dos dados também muda de inclinação e intercepto.

Cada nova etapa reduz um pouco o valor de J(w, b).

Conforme iteramos:

*   A trajetória acompanha a direção do gradiente mais íngreme
*   Os ajustes em w e b tornam o modelo cada vez mais alinhado aos pontos de treinamento
*   O custo diminui de forma consistente

Depois de várias iterações, o otimização converge ao **mínimo global** da função de custo — o ponto mais baixo da superfície.

O modelo final representa uma reta que ajusta bem os dados.

# **3\. Interpretação prática**

Com o modelo treinado, podemos usá-lo para prever preços de casas, por exemplo:

*   Para uma casa de **1250 ft²**, basta inserir x = 1250 no modelo final
*   A estimativa pode ser algo próximo a **$250.000** (valor apenas ilustrativo)

Esse é o propósito de treinar o modelo: **prever valores para novos exemplos**.

# **4\. O que é “descida de gradiente em lote” (batch gradient descent)**

A versão usada aqui é chamada de **Batch Gradient Descent**.

Significado:

*   Em **cada etapa de atualização**, o algoritmo usa **todos** os exemplos de treinamento
*   As derivadas são calculadas somando de i = 1 até m
*   O lote completo (“batch”) é sempre considerado antes de atualizar w e b

Por isso o nome “batch”.

Este é o método mais estável e matematicamente preciso, embora possa ser mais lento com conjuntos de dados gigantes.

O boletim “The Batch”, da DeepLearning.AI, usa esse termo justamente como referência a esse método.

# **5\. Outras variantes (contextualização)**

Existem versões mais rápidas ou mais eficientes do gradiente descendente:

*   **Stochastic Gradient Descent (SGD)**
    Atualiza usando apenas **um exemplo por vez**
*   **Mini-batch Gradient Descent**
    Atualiza usando **pequenos grupos** de exemplos (ex: 32, 64, 128)

Mas para regressão linear nesta especialização, usamos **apenas o batch gradient descent**, pois ele é:

*   simples
*   estável
*   totalmente determinístico
*   ideal para fins educacionais

![]()

![]()
