# O que é DevOps?

DevOps é originário do Lean.

**Lean** é uma abordagem de gerenciamento focada em **entregar mais valor ao cliente** com **menos desperdício**.

*   Tem como pilares:
*   **Eliminação de desperdícios**
*   **Respeito às pessoas**
*   **Melhoria contínua**

Promove **colaboração entre equipes** e a **entrega contínua de valor** ao cliente.

DevOps é a combinação de filosofias, práticas e ferramentas culturais que aumentam a capacidade de uma organização de entregar aplicativos e serviços em alta velocidade: evoluindo e aprimorando produtos em um ritmo mais acelerado do que organizações que utilizam processos tradicionais de desenvolvimento de software e gerenciamento de infraestrutura. Essa velocidade permite que as organizações atendam melhor seus clientes e concorram de forma mais eficaz no mercado.

O DevOps enfatiza melhor colaboração e eficiência para que as equipes possam inovar mais rapidamente e entregar maior valor às empresas e clientes.

![]()

Um loop infinito formado pelos estágios do ciclo de vida do software é uma representação comum da colaboração e eficiência contínuas sugeridas pelo DevOps.

DevOps é a abreviação de Desenvolvimento (Dev) e Operações (Ops). Desenvolvedores são as pessoas e os processos que criam software. Ops são as equipes e os processos que entregam e monitoram o software.

DevOps é um **conjunto de práticas e princípios** que visa **unificar desenvolvimento (Dev) e operações (Ops)** para entregar software de forma **mais rápida, estável, segura e com maior valor**.

Os desenvolvedores mudam as coisas rapidamente, lançam com frequência e medem o sucesso pela taxa de entrega. As operações são impulsionadas pela manutenção da estabilidade da aplicação. Lançamentos frequentes são motivo de preocupação quanto à estabilidade e confiabilidade da aplicação nas plataformas suportadas, especialmente durante alto tráfego de rede.

O DevOps reúne funções anteriormente isoladas (desenvolvimento, operações de TI, engenharia de qualidade e segurança) para otimizar a produtividade dos desenvolvedores e a confiabilidade das operações.

**O DevOps é uma combinação de:**

*   Filosofias culturais para remover barreiras e compartilhar a responsabilidade de ponta a ponta
*   Processos desenvolvidos para velocidade e qualidade, que otimizam a maneira como as pessoas trabalham
*   Ferramentas que se alinham aos processos e automatizam tarefas repetíveis, tornando o processo de lançamento mais eficiente e a aplicação mais confiável

**O foco está em:**

*   Colaboração entre equipes
*   Automação de processos
*   Redução de silos organizacionais
*   Responsabilidade compartilhada pelo ciclo completo do software

As equipes praticam o DevOps para aumentar a inovação e a agilidade, melhorar a qualidade, lançar mais rapidamente e reduzir custos. O DevOps melhora a eficiência de entrega e a previsibilidade do aplicativo e dos serviços.

# Problemas com Práticas Tradicionais de Desenvolvimento

As formas tradicionais de desenvolvimento de software têm se mostrado lentas e ineficientes, falhando em apoiar os esforços das equipes para entregar rapidamente aplicações estáveis ​​e de alta qualidade. Os desafios do desenvolvimento em cascata, aplicações monolíticas, processos manuais e estruturas de equipes isoladas causam gargalos e atrasos.

**Projetos de desenvolvimento em cascata** são lentos, não iterativos, resistentes a mudanças e têm longos ciclos de lançamento. Alguns motivos para isso incluem:

*   Os requisitos são rígidos, definidos no início do projeto e provavelmente não mudarão.
*   As fases de desenvolvimento são isoladas, cada uma iniciando após o término da fase anterior. Cada fase é apoiada por equipes altamente especializadas.
*   As transferências de uma fase para a outra são longas, frequentemente exigindo que as equipes troquem de ferramentas e gastem tempo esclarecendo informações incompletas ou ambíguas.
*   Os testes e a segurança ocorrem após a implementação, tornando as ações corretivas responsivas e caras.

![]()

As fases de desenvolvimento apoiadas por equipes isoladas e especializadas causam atrasos e são dispendiosas.

**Aplicações monolíticas** são difíceis de atualizar e implantar porque:

*   São desenvolvidas e implantadas como uma unidade, portanto, quando alterações são feitas, toda a aplicação precisa ser reimplantada.
*   Possuem funcionalidades fortemente acopladas, portanto, se a aplicação for grande o suficiente, a manutenção se torna um problema, pois os desenvolvedores têm dificuldade em entender toda a aplicação.
*   São implementadas usando uma única pilha de desenvolvimento, portanto, mudar a tecnologia é difícil e custoso.

![]()

Aplicações monolíticas possuem funcionalidades fortemente acopladas.

Processos manuais ao longo do ciclo de vida da aplicação são lentos, inconsistentes e propensos a erros. Por exemplo, definir e configurar manualmente a infraestrutura é demorado. Repetir esse processo manualmente não garante que nenhuma etapa será ignorada. Outro exemplo é dizer aos desenvolvedores para garantir que seu código seja completamente testado antes de enviá-lo. Mesmo com as melhores intenções, esse processo manual é lento e não impede que alguém se esqueça de um ou dois testes.

As equipes que dão suporte ao ciclo de vida de desenvolvimento de software tradicionalmente trabalham em silos. Especializadas em suas habilidades, equipes como negócios, desenvolvimento, garantia da qualidade, especialistas, manutenção e operações foram separadas umas das outras e exigem transferências programadas e rígidas. Embora essas equipes tenham o objetivo comum de entregar e dar suporte ao aplicativo, elas também têm suas próprias prioridades, ferramentas e processos. É difícil alcançar eficiência quando os membros do projeto se reportam a unidades diferentes e têm objetivos diferentes.

## 2.1. Acoplamento

**O que é acoplamento?**

**Acoplamento** se refere ao grau de dependência entre os componentes de um sistema. Ele pode ser:

*   **Forte**: os componentes conhecem detalhes internos uns dos outros e precisam mudar juntos.
*   **Fraco** (ou frouxo): os componentes são independentes e interagem de forma controlada, normalmente por meio de APIs ou mensagens assíncronas.

**Problema comum:** Alterações em um único componente exigem mudanças em diversos outros. Isso **aumenta o tempo de desenvolvimento** e **dificulta os testes**.

### 2.1.1. Problemas das Arquiteturas Fortemente Acopladas

**Exemplo: Sistemas de Varejo**

Tradicionalmente, sistemas de ponto de venda (PDV) são fortemente acoplados. Eles não são construídos em cima de APIs ou serviços reutilizáveis. Como consequência:

*   Integrações com dados de clientes, sistemas de RH e outros são rígidas.
*   Pequenas mudanças exigem grande coordenação entre times.

Esse tipo de arquitetura **limita a velocidade de entrega**, prejudicando diretamente a transformação digital da organização.

### 2.1.2. Vantagens de Arquiteturas Frouxamente Acopladas

*   Permitem que **equipes trabalhem com autonomia**.
*   Mudanças em um componente não afetam diretamente os outros.
*   Facilitam **testes independentes** e implementações mais rápidas.
*   Favorecem uma abordagem **orientada a fluxo de dados**, com comunicações assíncronas.
*   Reduzem o risco de falhas em cadeia.

### 2.1.3. Mudança de Mentalidade: Do Síncrono para o Assíncrono

Projetar sistemas pensando em **fluxo de dados assíncrono** significa:

*   Uma equipe pode trabalhar no seu componente sem depender diretamente de outra.
*   Testes e entregas se tornam mais simples.
*   A colaboração continua existindo, mas agora é mais **eficiente e menos bloqueante**.

Muitas organizações são boas em **gerenciar dependências**, designando pessoas para acompanhar integrações e cronogramas. Mas poucas conseguem **eliminá-las** de forma sistemática.

Uma das soluções mais eficazes é:

*   Criar **APIs e contratos de serviço bem definidos**.
*   Permitir que as equipes entreguem **sem precisar esperar ou depender de outras**.

A arquitetura desacoplada **libera a largura de banda de comunicação** entre as equipes, para que elas se concentrem em metas de alto nível — e não em decisões técnicas detalhadas que poderiam ser evitadas com uma boa arquitetura.

# Por que DevOps?

De acordo com o relatório Accelerate State of DevOps 2019, organizações de qualquer porte e setor podem se beneficiar do DevOps. Segundo o relatório, as equipes que adotam o DevOps com sucesso observam ciclos de entrega mais curtos, taxas de falha de mudanças reduzidas e melhor desempenho.

![]()

# Os benefícios do DevOps

Organizações de todos os portes, desde pequenas startups até grandes corporações, podem se beneficiar da adoção do DevOps. A seguir, alguns dos principais benefícios do DevOps.

## 4.1. Agilidade

Construa uma vantagem competitiva antecipando as necessidades do mercado e agregue valor rapidamente. Monitore seus aplicativos e apoie suas estratégias de desenvolvimento com dados reais. Tenha práticas de desenvolvimento implementadas que permitam que as equipes se movam em alta velocidade e entreguem continuamente atualizações controladas e pequenas, conforme necessário.

## 4.2. Entrega Rápida

Os princípios básicos da adoção do DevOps são integração e entrega contínuas, ciclo de feedback rápido e monitoramento contínuo, o que torna os processos de desenvolvimento ágil de software mais rápidos e eficientes.

Além disso, utiliza a automação para garantir um fluxo tranquilo do Ciclo de Vida de Desenvolvimento de Software (SDLC) como uma extensão evolutiva da técnica Ágil. Oferece o escopo para revisões rápidas e consistentes, promovendo uma cultura DevOps compartilhada, de forma que quaisquer bugs sejam corrigidos em tempo hábil.

## 4.3. Confiabilidade

Garanta a qualidade das atualizações de aplicativos e das mudanças na infraestrutura para que você possa entregar de forma confiável e em um ritmo mais rápido, mantendo uma experiência positiva para os usuários finais. Utilize práticas como integração e entrega contínuas para testar se cada mudança é funcional e segura. Práticas de monitoramento e observabilidade ajudam você a se manter informado sobre o desempenho em tempo real.

## 4.4. Escala

A AWS fornece serviços que ajudam você a praticar o DevOps em sua empresa em escala. Essas ferramentas automatizam tarefas manuais, ajudam as equipes a gerenciar ambientes complexos em escala e mantêm os engenheiros no controle da alta velocidade proporcionada pelo DevOps.

Com os serviços da AWS, você pode gerenciar uma única instância ou escalar para milhares. O uso desses serviços ajuda você a aproveitar ao máximo os recursos de computação flexíveis, simplificando o provisionamento, a configuração e o dimensionamento.

## 4.5. Colaboração aprimorada

Construa equipes mais eficazes sob um modelo cultural de DevOps, que enfatiza valores como propriedade e responsabilidade. Desenvolvedores e equipes de operações colaboram estreitamente, compartilham muitas responsabilidades e combinam seus fluxos de trabalho. Isso reduz ineficiências e economiza tempo. Por exemplo, escrever código que leve em consideração o ambiente em que é executado reduz os períodos de transferência entre desenvolvedores e operações.

## 4.6. Segurança

O modelo DevOps utiliza regras de aplicação automáticas, controles refinados e técnicas de gerenciamento de configuração que ajudam a avançar rapidamente, mantendo a alavancagem e garantindo as políticas de conformidade.

Por exemplo, você pode descrever e monitorar a aplicação em escala, usando infraestrutura como código e política como código.

# Por que algumas equipes inicialmente resistem à adoção do DevOps?

A relutância em adotar o DevOps é natural, pois ele trará mudanças e revolucionará a maneira como você trabalha e interage com os outros. O DevOps terá impacto na organização e na equipe. Para superar essa relutância, é importante entender o valor do DevOps e definir expectativas realistas para as equipes. Para ter sucesso, você precisa da adesão de toda a organização e das equipes de desenvolvimento.

DevOps **não é um cargo ou equipe específica**, mas sim **uma cultura organizacional**.

Praticar DevOps implica **envolver toda a organização**, não apenas equipes técnicas.

O verdadeiro valor do DevOps está na **transformação cultural e estrutural da empresa**, fundamentada em **princípios Lean**.

# Cultura DevOps

Uma mudança para DevOps exige a criação e o desenvolvimento de uma cultura DevOps, que é uma cultura de transparência, colaboração eficaz e integrada, e objetivos comuns.

Você pode ter os processos e ferramentas para dar suporte ao DevOps, mas, para uma adoção bem-sucedida do DevOps, as pessoas da organização devem ter a mentalidade certa para nutrir a cultura DevOps.

A sigla **CALMS** resume os valores essenciais do DevOps:

1.  **Cultura** – Colaboração, confiança e foco em valor para o cliente.
2.  **Automação** – Redução de tarefas manuais, aumento de eficiência.
3.  **Lean** – Aplicação dos princípios enxutos para melhorar fluxo e eliminar desperdício.
4.  **Medição (Measurement)** – Acompanhamento de métricas para tomada de decisão.
5.  **Compartilhamento (Sharing)** – Disseminação de conhecimento e boas práticas.

Existem **sete princípios fundamentais** que podem ajudá-lo a alcançar uma cultura DevOps.

## 6.1. Crie um ambiente altamente colaborativo

O DevOps reúne o desenvolvimento e as operações para quebrar silos, alinhar metas e atingir objetivos comuns. Toda a equipe (desenvolvimento, testes, segurança, operações e outras) tem propriedade de ponta a ponta sobre o software que lança. Elas trabalham juntas para otimizar a produtividade dos desenvolvedores e a confiabilidade das operações. As equipes aprendem com as experiências umas das outras, ouvem preocupações e perspectivas e otimizam seus processos para alcançar os resultados necessários.

Essa maior visibilidade permite que os processos sejam unificados e continuamente aprimorados para atingir as metas de negócios. A colaboração também cria uma cultura de alta confiança que valoriza os esforços de cada membro da equipe e transfere conhecimento e melhores práticas entre as equipes e a organização.

## 6.2. Automatize sempre que possível

Com o DevOps, tarefas repetíveis são automatizadas, permitindo que as equipes se concentrem na inovação. A automação fornece os meios para desenvolvimento, testes e implantação rápidos. Identifique oportunidades de automação em todas as fases, como integrações de código, revisões, testes, segurança, implantações e monitoramento, usando as ferramentas e serviços certos.

Por exemplo, a infraestrutura como código (IaC) pode ser usada para ambientes predefinidos ou aprovados e versionada para que ambientes repetíveis e consistentes sejam construídos. Você também pode definir verificações regulatórias e incorporá-las em testes que são executados continuamente como parte do seu pipeline de lançamento.

## 6.3. Foco nas necessidades do cliente

Uma mentalidade de priorizar o cliente é um fator-chave para impulsionar o desenvolvimento. Por exemplo, com ciclos de feedback, as equipes de DevOps mantêm contato com seus clientes e desenvolvem software que atenda às suas necessidades. Com uma arquitetura de microsserviços, elas conseguem mudar rapidamente de direção e alinhar seus esforços a essas necessidades.

Processos simplificados e automação entregam as atualizações solicitadas com mais rapidez e mantêm a satisfação do cliente alta. O monitoramento ajuda as equipes a determinar o sucesso de suas aplicações e a alinhar continuamente seus esforços com foco no cliente.

## 6.4. Desenvolva em pequena escala e lance com frequência

As aplicações não são mais desenvolvidas como um sistema monolítico com práticas rígidas de desenvolvimento, testes e implantação. As arquiteturas de aplicações são projetadas com componentes menores e fracamente acoplados. Políticas abrangentes (como compatibilidade com versões anteriores ou gerenciamento de mudanças) estão em vigor e fornecem governança aos esforços de desenvolvimento. As equipes são organizadas para corresponder à arquitetura de sistema necessária. Elas têm um senso de propriedade por seus esforços.

Adotar práticas modernas de desenvolvimento, como lançamentos de código em pequena escala e frequentes, dá às equipes a agilidade necessária para responder às necessidades do cliente e aos objetivos de negócios.

## 6.5. Inclua segurança em todas as fases

Para oferecer suporte à entrega contínua, a segurança deve ser iterativa, incremental, automatizada e presente em todas as fases do ciclo de vida da aplicação, em vez de algo que é feito antes de um lançamento. Treine as equipes de desenvolvimento e operações para incorporar a segurança em cada etapa do ciclo de vida da aplicação. Dessa forma, você pode identificar e resolver potenciais vulnerabilidades antes que elas se tornem grandes problemas e sejam mais caras para consertar.

Por exemplo, você pode incluir testes de segurança para verificar chaves de acesso codificadas ou o uso de portas restritas.

## 6.6. Experimente e aprenda continuamente

Investigação, inovação, aprendizado e mentoria são incentivados e incorporados aos processos de DevOps. As equipes são inovadoras e seu progresso é monitorado. Com a inovação, o fracasso acontece. A liderança aceita o fracasso e as equipes são incentivadas a ver o fracasso como uma oportunidade de aprendizado.

Por exemplo, as equipes usam ferramentas de DevOps para criar ambientes sob demanda, permitindo que experimentem e inovem, talvez no uso de novas tecnologias para atender a um requisito do cliente.

## 6.7. Melhore continuamente

Métricas criteriosas ajudam as equipes a monitorar seu progresso, avaliar seus processos e ferramentas e trabalhar em direção a objetivos comuns e melhoria contínua. Por exemplo, as equipes se esforçam para melhorar as métricas de desempenho de desenvolvimento, como a taxa de transferência.

Elas também se esforçam para aumentar a estabilidade e reduzir o tempo médio de restauração do serviço. Usando as ferramentas de monitoramento corretas, você pode definir benchmarks de aplicativos para comportamentos usuais e monitorar continuamente as variações.

# 7\. Práticas de DevOps

A cultura DevOps leva a práticas de DevOps voltadas para a otimização e o aprimoramento do ciclo de vida do desenvolvimento, a fim de fornecer atualizações frequentes e confiáveis, mantendo a estabilidade.

## 7.1. Comunicação e colaboração

As equipes de DevOps estabelecem normas culturais sólidas em torno da transparência das informações e da comunicação. Essas equipes multifuncionais têm responsabilidade e, portanto, em vez de avaliar apenas o próprio trabalho, consideram as necessidades do projeto coletivamente. Elas criam empatia pelos esforços, parcerias e confiança umas das outras, enquanto colaboram em prol de objetivos comuns. Elas unem fisicamente os fluxos de trabalho tradicionais de desenvolvimento e operações e melhoram sistematicamente a produtividade.

As ferramentas de DevOps e a automação do processo de entrega dão suporte a esses processos e fluxos de trabalho consolidados, coordenam esforços, automatizam tarefas repetitivas e facilitam os ciclos de feedback necessários para uma boa comunicação e colaboração.

## 7.2. Monitoramento e observabilidade

O monitoramento e a observabilidade são usados ​​para avaliar a eficácia das mudanças na aplicação e na infraestrutura e como elas impactam o desempenho e a experiência geral do usuário. Parte dos ciclos de feedback do DevOps, o monitoramento e a observabilidade ajudam as equipes a reagir, aprender, planejar e aprimorar.

Um sistema observável é um sistema que gera dados suficientes de todos os recursos, aplicações e serviços na forma de logs, métricas e rastreamentos para obter visibilidade operacional de todo o sistema. Os logs relatam eventos discretos, como avisos. As métricas capturam informações de integridade e desempenho, como taxa de solicitações ou tempo de resposta. Os rastreamentos relatam transações e o fluxo de dados em um sistema distribuído, como um composto por microsserviços.

Ao observar um sistema, você pode tirar inferências concisas sobre por que algo está acontecendo.

O monitoramento informa o que está acontecendo com o seu sistema. Ao consolidar e visualizar os dados coletados por um sistema observável ao longo do tempo, as equipes obtêm insights sobre o desempenho, identificam tendências, podem definir alarmes e fazer previsões sobre os resultados esperados.

## 7.3. Integração contínua (CI)

A integração contínua é uma prática de desenvolvimento de software DevOps na qual os desenvolvedores mesclam regularmente suas alterações de código em um repositório central, após o qual compilações e testes automatizados são executados. Dessa forma, as equipes podem resolver problemas de mesclagem e defeitos de código antecipadamente, quando são mais fáceis e econômicos de resolver.

A integração contínua geralmente se refere à fase de construção ou integração do processo de lançamento de software. Ela requer tanto um componente de automação (por exemplo, um CI ou serviço de construção) quanto um componente cultural (por exemplo, aprender a integrar com frequência). Os principais objetivos da integração contínua são encontrar e corrigir bugs mais rapidamente, melhorar a qualidade do software e reduzir o tempo necessário para validar e lançar novas atualizações de software.

## 7.4. Entrega contínua/Implantação contínua (CD)

A entrega contínua é uma prática de desenvolvimento de software em que cada alteração de código é automaticamente construída, testada e, em seguida, implantada em um ambiente de teste ou preparação que não seja de produção. A aprovação manual é necessária antes do envio para produção. Quando implementado corretamente, os desenvolvedores sempre terão um artefato de construção pronto para implantação, que passou por um processo de teste padronizado.

A implantação contínua é semelhante à entrega contínua, mas com implantação automática para produção. O código testado não precisa de aprovação explícita antes de ser enviado para produção.

## 7.5. Arquitetura de microsserviços

Uma arquitetura de microsserviços é uma abordagem de design que constrói uma aplicação como um conjunto de serviços fracamente acoplados. Cada serviço é projetado para um conjunto de capacidades e se concentra na resolução de um problema de negócios específico. Os serviços não precisam compartilhar seu código ou implementação com outros serviços. Qualquer comunicação entre componentes individuais ocorre por meio de APIs bem definidas. Esses serviços podem ser atribuídos a equipes totalmente responsáveis ​​e podem ser desenvolvidos, testados e implantados independentemente de outros serviços.

De acordo com uma pesquisa da DevOps Research and Assessment (DORA), o tipo de arquitetura que a equipe escolhe é um preditor direto do sucesso que ela terá na entrega contínua. A natureza dos microsserviços permite desenvolvimento, atualizações e correções mais rápidos, além de implantações mais ágeis.

## 7.6. Infraestrutura como código

Desenvolvimento, testes e produção são executados em ambientes complexos compostos por hardware e software. A criação e configuração manual de ambientes não é escalável e está sujeita a erros.

Infraestrutura como código (IaC) é uma prática na qual a infraestrutura é provisionada e gerenciada usando técnicas de desenvolvimento de código e software, como controle de versão e integração contínua.

O modelo baseado em API da nuvem permite que desenvolvedores e administradores de sistemas interajam com a infraestrutura programaticamente e em escala, sem a necessidade de configurar e configurar recursos manualmente. Como os ambientes são definidos por código, eles podem ser implantados rapidamente com conformidade aplicada dinamicamente, atualizados com os patches mais recentes, revertidos para uma versão anterior ou duplicados de forma repetível. Além disso, ao reagir às mudanças no ambiente por meio de modificações nesse código, você pode rastrear alterações, otimizar recursos e melhorar o tempo de atividade do sistema.

Um pipeline de DevOps é um conjunto de etapas que movem o código da fonte até a implantação. O gráfico a seguir descreve as etapas típicas de um pipeline de DevOps e as fases envolvidas em um pipeline de CI/CD.

![]()

1.  **Código**

Desenvolva código em linguagens como .Java, .NET ou Python. Quando estiver pronto, entregue esse código a um local central. Os pares revisarão o novo código.

1.  **Construção**

A criação de compilações do seu software pode incluir algumas destas ações:

\- Compilar código

\- Verificar estilos e padrões de código

\- Analisar a complexidade e a manutenibilidade do código

\- Validar dependências

\- Criar imagens de contêiner

\- Executar testes unitários

1.  **Teste**

Avalie se o aplicativo atende aos requisitos funcionais, de desempenho, de design e de implementação definidos.

Algumas práticas de teste são:

\- Teste funcional

\- Teste de integração

\- Teste de regressão

\- Teste de aceitação

\- Teste de carga

\- Teste de segurança

1.  **Liberação**

Prepare e empacote o código testado com um número de versão específico.

1.  **Implantar**

Implantar a versão em ambientes específicos, como teste, preparação, alfa, beta ou produção.

1.  **Monitorar**

Monitore o aplicativo em produção para detectar rapidamente atividades ou erros incomuns.

Um pipeline de CI/CD é um bom exemplo de como as equipes de DevOps usam ferramentas para otimizar fluxos de trabalho e padronizar práticas. Um pipeline de CI/CD garante a qualidade do código, a segurança e implantações rápidas e consistentes, progredindo de forma repetitiva ao longo do pipeline. As equipes de DevOps removem iterativamente sobreposições de processos, erros humanos e gargalos por meio da automação.

Toda equipe de DevOps precisa de um pipeline de CI/CD eficiente e confiável. Um pipeline de CI/CD requer uma cadeia de ferramentas bem integrada.

# 8\. Ferramentas de DevOps

Ao aprender sobre as ferramentas de DevOps, é importante perceber que as ferramentas de DevOps da AWS se integram a outras ferramentas de terceiros. Os parceiros da AWS se integram e ampliam as ofertas da AWS. Isso significa que você pode usar ferramentas como GitHub e Jenkins para construir sua cadeia de ferramentas de DevOps, que dará suporte às suas equipes e otimizará seus processos. Use suas ferramentas de terceiros e de código aberto preferidas com a AWS para construir sua solução de ponta a ponta.

A AWS fornece serviços que ajudam você a praticar DevOps em sua empresa. Mais adiante no curso, você aprenderá sobre as ferramentas e serviços de DevOps da AWS. Por enquanto, aqui estão as categorias gerais de ferramentas que você pode precisar para apoiar seus esforços de DevOps.

## 8.1. Nuvem

As equipes de desenvolvimento precisam inovar rapidamente e entregar aplicativos confiáveis ​​e seguros. As equipes dependem de provedores de plataforma em nuvem e recursos de computação em nuvem para uma variedade de tecnologias que dão suporte aos esforços de desenvolvimento de aplicativos. Em vez de comprar, possuir e manter data centers e servidores físicos, as equipes provisionam ambientes sob demanda, usando provedores de nuvem como a AWS.

**NoOps**: Termo mal interpretado que sugere eliminação de operações, mas na prática significa **mudança de foco para automação operacional**, especialmente com o uso de **serviços em nuvem**. **Operações continuam sendo essenciais**.

## 8.2. Desenvolvimento

As equipes de DevOps precisam colaborar continuamente com seus membros. Existem diversas ferramentas que ajudam as equipes a desenvolver e entregar com mais rapidez. Ambientes de desenvolvimento integrados (IDEs) ajudam você a escrever, executar e depurar código para seus aplicativos. Kits de desenvolvimento de software (SDKs) são conjuntos de ferramentas que permitem aos programadores desenvolver aplicativos para uma plataforma específica. Repositórios de código-fonte, ou sistemas de controle de versão, armazenam os arquivos do seu projeto.

Conforme necessário, você pode acessar seus documentos e código, ver o histórico de revisões, comparar alterações ao longo do tempo ou reverter para versões anteriores.

Exemplos:

IDEs: AWS Cloud9, IntelliJ, Eclipse, Visual Studio Code

SDKs: AWS SDK para Java, iPhone SDK

Repositórios de código-fonte: GitHub, AWS CodeCommit

## 8.3. CI/CD

Práticas como testes contínuos, integração contínua (CI) e entrega/implantação contínua (CD) são suportadas por ferramentas que proporcionam continuidade perfeita em todas as fases de desenvolvimento. As ferramentas de CI/CD automatizam o código continuamente integrado que as equipes desenvolvem, verificam a conformidade com os padrões, executam testes com mais frequência, promovem o código para diferentes ambientes de teste e implantam produtos na infraestrutura de forma repetida e confiável.

As ferramentas de CI/CD devem ajudar a trazer agilidade aos processos de desenvolvimento e implantação de aplicativos, ao mesmo tempo em que fornecem feedback contínuo e alertam as equipes apropriadas sobre quaisquer problemas.

Exemplos:

Ferramentas de build: Jenkins, Travis CI, AWS CodeBuild

Controle de código-fonte, repositórios: Git, AWS CodeCommit

Ferramentas de implantação: AWS CodeDeploy, AWS CloudFormation

Automação de pipeline: AWS CodePipeline, Jenkins, GitLab

## 8.4. Automação de infraestrutura

Defina programaticamente sua infraestrutura, incluindo restrições, para provisionar seus ambientes de forma repetida e consistente (sandboxes de desenvolvimento, testes, staging, produção).

Usando modelos, você pode implantar serviços de computação, permissões, dependências e muito mais. Você pode configurar regras e automatizar a correção.

Exemplos:

Ferramentas de automação de infraestrutura: AWS CloudFormation, Terraform, AWS Elastic Beanstalk

Ferramentas de gerenciamento de configuração: Chef, Puppet, AWS OpsWorks

## 8.5. Contêineres e serviços sem servidor

Contêineres e serviços de computação sem servidor permitem que os desenvolvedores se concentrem nos aplicativos, e não nos detalhes do ambiente host.

Os contêineres empacotam o código, as definições de configuração e as dependências necessárias para executar o aplicativo. Dessa forma, o aplicativo é portátil e pode ser executado em qualquer servidor. Contêineres são semelhantes a máquinas virtuais, porém mais leves, pois são virtualizados no nível do sistema operacional (SO). Os contêineres executam desde microsserviços até grandes aplicativos legados. Eles simplificam a maneira como você cria, testa e implanta aplicativos em múltiplos ambientes.

Eles tornam o aplicativo implantado mais seguro, pois as políticas de segurança podem ser implementadas no nível do contêiner. No entanto, os contêineres exigem orquestração de contêineres para gerenciar ou agendar o trabalho de contêineres individuais.

Serviços de computação sem servidor são serviços que permitem criar e executar código, e permitem que a sobrecarga da infraestrutura seja gerenciada pelo provedor de nuvem do serviço, como a AWS.

Exemplos:

Serviços sem servidor: AWS Lambda, AWS Fargate

Serviços de contêiner:

Tempos de execução: Docker, Containerd

Orquestração: Amazon Elastic Container Service (Amazon ECS), Kubernetes, Amazon Elastic Kubernetes Service (Amazon EKS)

## 8.6. Monitoramento e observabilidade

Monitoramento e observabilidade são aspectos essenciais do DevOps, ajudando você a ser proativo na prevenção de desafios antes que eles ocorram. Com ferramentas, você pode coletar métricas sobre a integridade e o desempenho do seu aplicativo. Você pode capturar a frequência de implantação, identificar implantações bem-sucedidas ou com falha, o tráfego de uso do aplicativo e muito mais.

As ferramentas podem ajudar a rastrear fluxos de solicitações e transações de ponta a ponta em um sistema distribuído. Com ferramentas, você pode visualizar e analisar logs, métricas e rastreamentos para descobrir novos insights sobre a integridade, o desempenho e a disponibilidade do seu sistema. Com insights, você pode otimizar seus processos, melhorar o desempenho do sistema e reduzir o tempo de inatividade.

Exemplos: AWS X-Ray, Amazon CloudWatch, AWS Config, AWS CloudTrail

Ao escolher as ferramentas, é importante usar aquelas que funcionam para sua equipe.

# 9\. Ciclo de Vida no DevOps

Abrange todas as fases do desenvolvimento:

*   Planejamento
*   Construção
*   Testes
*   Implantação
*   Operação
*   Suporte

Todos os membros da equipe são **corresponsáveis** por essas etapas.

A transformação DevOps não exige apenas novas ferramentas — **exige novas mentalidades e papéis**. Muitas funções evoluem:

**Analistas de Negócios → Product Owners**

*   Passam a atuar mais próximos das equipes de desenvolvimento.
*   Ajudam a priorizar o backlog e tomar decisões diárias.
*   Assumem responsabilidades estratégicas de **valor ao cliente**.

**Desenvolvedores → Engenheiros multifuncionais**

*   Deixam de ser apenas codificadores.
*   Assumem responsabilidades por **qualidade, segurança e performance**.
*   Precisam adotar uma **visão sistêmica**, entendendo impacto e valor.

No modelo tradicional, os papéis eram bem definidos:

*   O analista escrevia requisitos.
*   O desenvolvedor codificava.
*   O QA testava.
*   O operador colocava em produção.

Em DevOps, as **linhas se tornam borradas**:

*   Membros da equipe podem exercer **funções sobrepostas**.
*   A organização é feita com foco em **entregar valor ao cliente**.
*   A responsabilidade é **compartilhada**.

**Modelo Crawl → Walk → Run**

*   **Crawl**: Times estão começando, explorando DevOps com cuidado.
*   **Walk**: Processos definidos, entregas frequentes, responsabilidade mista.
*   **Run**: Equipes autônomas, entrega contínua, experimentação intensa e aprendizado ágil.

Equipes bem estruturadas no DevOps **avançam até o estágio Run**, com alto desempenho.

# 10\. O Modelo das Três Maneiras (The Three Ways)

Desenvolvido por **Gene Kim** e **Mike Orzen**, o modelo das **Três Maneiras** é um pilar da filosofia DevOps e estrutura os princípios fundamentais da prática:

**As Três Maneiras:**

1.  **Pensamento Sistêmico**
2.  **Amplificação de Ciclos de Feedback**
3.  **Cultura de Experimentação e Aprendizado Contínuo**

## 10.1. Pensamento Sistêmico

Foco no desempenho de todo o sistema, e não em silos ou equipes isoladas. DevOps quebra barreiras funcionais e promove a colaboração em toda a cadeia de valor.

Princípios:

*   Não enviar defeitos para fases posteriores.
*   Evitar otimizações locais (melhorias que prejudicam o sistema como um todo).
*   Aumentar o fluxo de entrega.
*   Buscar compreensão profunda do sistema.
*   Qualidade é responsabilidade de todos. (Deming)

Exemplo Prático – Nordstrom

A empresa operava em silos.

Ao mapear o fluxo de entrega para aplicativos móveis, descobriram que estavam enviando defeitos à produção.

A solução: testes automatizados, integração de QA e operações nas squads, e métricas de tempo de ciclo para medir qualidade sistêmica.

## 10.2. Amplificação dos Ciclos de Feedback

Refere-se à criação de ciclos de feedback curtos, rápidos e visíveis, permitindo correções contínuas no produto e melhorias no processo.

O que é um loop de feedback?

Um processo de reflexão contínua sobre o resultado das ações, que orienta os próximos passos. Quanto mais rápido o loop, maior a eficiência.

Princípios:

*   Ouvir e responder a todos os clientes (internos e externos).
*   Encurtar e ampliar os ciclos de feedback.
*   Incorporar conhecimento no ponto certo do processo.

Exemplo Prático – Starbucks

Painel de qualidade mostrava diariamente os resultados dos testes automatizados.

Quando a taxa de falhas ultrapassava o limite, o painel ficava vermelho.

O deploy era interrompido até restaurar a qualidade.

Feedback visual e frequente melhorava a responsabilidade e o foco da equipe.

## 10.3. Cultura de Experimentação e Aprendizado Contínuo

Criação de um ambiente seguro para:

*   Experimentar.
*   Assumir riscos calculados.
*   Aprender com falhas.
*   Repetir e praticar até alcançar o domínio.

Princípios:

*   Reservar tempo para melhoria contínua.
*   Recompensar equipes que assumem riscos.
*   Introduzir falhas controladas para aumentar a resiliência.

Exemplo Prático – Cultura de Testes

Nordstrom: investimentos estratégicos em inovação, proteção da capacidade das equipes.

Starbucks: CTO incentivava hackathons e dias de inovação.

Nike: equipes com modelos como “20% para inovação” adaptados à sua realidade.

Prática de falhas estruturadas, inspirada na engenharia do caos (ex: Netflix e o “Chaos Monkey”).

Maneira

Foco

Resultado Esperado

1ª – Pensamento Sistêmico

Fluxo completo

Redução de silos e defeitos

2ª – Feedbacks Ampliados

Correção contínua

Feedback rápido e preciso

3ª – Experimentação

Inovação

Cultura resiliente e aprendizado

# 11\. Lean no Desenvolvimento de Software

## 11.1. 7 Princípios

### 11.1.1. Eliminar Desperdícios

*   **Foco:** Evitar trabalho desnecessário, decisões atrasadas ou produção sem valor.
*   **Exemplos:**
    *   Codificar além do necessário.
    *   Produzir funcionalidades que não serão usadas.
    *   Atrasar decisões em busca de precisão absoluta.

_"É melhor começar e aprender do que esperar pela decisão perfeita."_

### 11.1.2. Construir Qualidade

*   **Foco:** Qualidade não é algo que se inspeciona depois, mas algo que se **constrói desde o início**.
*   Inspirado por Deming: “**A qualidade é responsabilidade de todos.**”

### 11.1.3. Criar Conhecimento

*   **Foco:** Desenvolvimento de software é aprendizado contínuo.
*   **Como implementar:**
    *   Promover ciclos de feedback.
    *   Aprender com falhas.
    *   Ajustar-se ao longo do processo.

### 11.1.4. Tomada de Decisão Diferida (Comprometimento Diferido)

*   **Foco:** Tomar decisões no **momento certo** — nem cedo demais, nem tarde demais.
*   **Conceito útil:**
    *   **Porta de mão única**: Decisão irreversível → requer mais análise.
    *   **Porta de mão dupla**: Reversível → mais vale **agir e aprender**.

### 11.1.5. Entrega Rápida

*   **Foco:** Entregar em pequenos lotes para acelerar o feedback e melhorar a adaptabilidade.
*   **Benefícios:**
    *   Correção de curso frequente.
    *   Redução de riscos.
    *   Validação contínua.

### 11.1.6. Respeito às Pessoas

*   **Foco:** Pessoas são o ativo mais valioso de uma organização.
*   **Princípio fundamental do Lean e do DevOps.**
*   **Prática:** Criar ambientes seguros e colaborativos.

_"Se não praticarmos respeito, todo o resto desmorona."_

### 11.1.7. Otimização do Todo

*   **Foco:** Otimizar o **fluxo completo de valor**, e não apenas partes isoladas.
*   **Evitar:** Subotimização local (ex: melhorar um setor à custa do todo).
*   Conexão direta com o **pensamento sistêmico**.

## 11.2. 7 Desperdícios

### 11.2.1 Trabalho Parcialmente Feito

*   Código implementado, mas:
    *   Não está em produção.
    *   Não está testado.
    *   Não foi versionado.
*   **Problema:** Atraso na entrega de valor real.

### 11.2.2. Funcionalidades Extras

*   Desenvolver **mais do que o necessário**.
*   Funcionalidades não utilizadas = custo sem retorno.

### 11.2.3. Reaprendizado ou Retrabalho

*   Reanalisar decisões por falta de documentação ou conhecimento compartilhado.
*   **Exemplo:** Voltar a discutir a mesma escolha técnica por falta de histórico.

### 11.2.4. Transferências

*   Múltiplas passagens de trabalho entre times ou pessoas.
*   **Consequência:** Desalinhamento, perda de contexto, retrabalho.

_"Minimizar entregas de ida e volta acelera o ciclo."_

### 11.1.5. Atrasos

*   Esperar por aprovações, compilações, testes, infraestrutura.
*   Qualquer espera = redução da eficiência do fluxo.

### 11.1.6. Troca de Tarefas (Multitarefa)

*   Também conhecida como "context switch".
*   **Evidência:** Multitarefas diminuem drasticamente a produtividade.

_"Multitarefa é inimiga da produtividade – dentro e fora do software."_

### 11.1.7. Defeitos

*   Falhas no código são desperdício.
*   Demandam retrabalho, degradam a confiança do usuário e atrasam entregas.

**Princípios do Lean (Software)**

**Desperdícios Elimináveis**

1\. Eliminar Desperdícios

1\. Trabalho Parcialmente Feito

2\. Construir Qualidade

2\. Funcionalidades Extras

3\. Criar Conhecimento

3\. Reaprendizado

4\. Comprometimento Diferido

4\. Transferências

5\. Entrega Rápida

5\. Atrasos

6\. Respeito às Pessoas

6\. Troca de Tarefas

7\. Otimização do Todo

7\. Defeitos

# 12\. Kata de Melhoria

O **Kata de Melhoria** é um **princípio prático de melhoria contínua**. Vem do **Sistema Toyota de Produção** e foi amplamente adotado no universo DevOps por seu poder em guiar times rumo à excelência através de pequenos ciclos de aprendizado.

**Kata**: no contexto japonês, significa "forma padrão de fazer algo repetidamente para alcançar maestria".

O **Kata de Melhoria** é um **processo sistemático de experimentação**, guiado por metas de longo prazo, que permite que equipes progridam de forma iterativa, aprendendo e se adaptando à medida que avançam em direção a uma visão.

## 12.1. Etapas do Kata de Melhoria

### 12.1.1. Entender a Direção ou Visão

Onde queremos chegar?

Ex: "Reduzir defeitos a zero", "Lançamentos sob demanda", etc.

### 12.1.2. Compreender a Condição Atual

Onde estamos agora?

Ex: "Atualmente, temos 20 defeitos por versão."

### 12.1.3. Estabelecer a Próxima Condição-Alvo

Meta intermediária mensurável.

Ex: "Reduzir para 10 defeitos na próxima entrega."

### 12.1.4. Experimentar com PDCA (Plan, Do, Check, Adjust)

Plan: Planejar os próximos passos.

Do: Executar o experimento.

Check: Verificar os resultados.

Adjust: Ajustar e planejar o próximo experimento.

**Exemplo Real – Caso Nordstrom**

Após sucesso com o **Kata de Melhoria** em apps móveis (reduzindo lançamentos de 2 por ano para sob demanda), a empresa decidiu aplicar a mesma abordagem em outras equipes:

**Contexto:**

*   Meta: Reduzir o tempo de ciclo em 20%.
*   Equipes envolvidas: Web, Personalização, Fidelidade.

**Passos seguidos:**

1.  **Entendimento da condição atual**
    1.  Mapeamento de fluxo de valor → Equipe Web com ciclo de **5 semanas**.
2.  **Definição da meta**
    1.  Reduzir o tempo de ciclo para **4 semanas**.
3.  **Primeiros experimentos**
    1.  **Remoção de aprovações manuais** no fim do ciclo ("fase de endurecimento").
    2.  Isso eliminou **1 dia inteiro** do processo.
4.  **Foco na qualidade antes da fase final**
    1.  Redução de **exceções**.
    2.  Automação de testes → menos retrabalho → menos exceções.
5.  **Melhoria da implementação**
    1.  Automatização das tarefas de release.
    2.  Redução do tempo de deploy de **vários dias para 1 dia**.

**PDCA na Prática**

Durante os experimentos:

*   **Check-ins semanais** para ações de curto prazo.
*   **Frequência adaptada** para experimentos mais longos (ex: automações complexas → checkpoints a cada 3 semanas).

PDCA não é engessado. A cadência é ajustada conforme o tipo de experimento.

**Lições de Liderança**

Um ponto crítico ressaltado:

**Líderes frequentemente acham que já sabem qual é o problema e a solução.**

Com o Kata de Melhoria:

*   A liderança **define a direção**, mas as equipes **experimentam para chegar lá**.
*   Estimula uma **cultura de aprendizado**, em vez de soluções prontas e impostas.

**Conclusão**

O Kata de Melhoria:

*   Estimula **melhoria contínua baseada em evidências**.
*   Garante que cada passo seja **consciente, iterativo e alinhado com a visão**.
*   Cria times **autônomos e responsáveis**, com capacidade de identificar, testar e resolver problemas reais.

# 13\. Estrutura de Solução de Problemas A3

A **estrutura A3** é uma abordagem estruturada para a **resolução de problemas**, originada no **Sistema Toyota de Produção**.

O nome "A3" refere-se apenas ao **tamanho do papel** (297 x 420 mm ou 11x17 pol.) tradicionalmente usado para documentar o processo — **não é um acrônimo**.

## 13.1. Relação com o Ciclo de Deming (PDCA)

A estrutura A3 é um **modelo prático do ciclo PDCA**:

**Etapas A3**

**Equivalente no PDCA**

1 a 4 – Planejamento

**Plan**

5 – Execução (contramedidas)

**Do**

6 – Verificação dos efeitos

**Check**

7 – Padronização/Ajuste

**Act**

## 13.2. As 7 Etapas da Estrutura A3

### 13.2.1. Definir o Contexto

*   **Objetivo:** Justificar por que o problema está sendo discutido.
*   **Inclui:** Impacto no negócio.
*   **Exemplo:** “Problemas de qualidade estão afetando diretamente a produção e a experiência do cliente.”

### 13.2.2. Compreender a Condição Atual

*   **Objetivo:** Mapear a realidade atual com dados.
*   **Exemplo:** “A cada release da equipe Web, temos 3 incidentes de alta gravidade.”

Termos como "condição atual" também aparecem no **Kata de Melhoria**.

### 13.2.3. Definir a Meta ou Estado-Alvo

*   **Objetivo:** Estabelecer **um resultado desejado e mensurável**.
*   **Exemplo:** “Zerar os incidentes de alta gravidade em novos releases.”

### 13.2.4. Analisar Causas-Raiz

*   **Objetivo:** Identificar **fatores contribuintes** ao problema.
*   **Nota importante:** Em sistemas complexos, raramente há **uma única causa-raiz**.
*   **Exemplo de causas múltiplas:**
    *   Baixa cobertura de testes.
    *   Exceções manuais no final do ciclo.
    *   Testes automatizados ausentes.

### 13.2.5. Explorar e Selecionar Contramedidas

*   **Objetivo:** Gerar ideias para resolver o problema e selecionar hipóteses para testar.
*   **Método comum:** Matriz de esforço x impacto.
*   **Exemplo de comparação:**
    *   Criar automação de testes → impacto 1, esforço alto.
    *   Criar um "gate" no processo → impacto 2, esforço baixo → _priorizar primeiro._

### 13.2.6. Criar um Plano de Implementação

*   **Objetivo:** Formalizar a ação escolhida com prazos, responsáveis e entregáveis.
*   **Exemplo:**
    *   Ação: Criar 15 scripts de testes automatizados.
    *   Prazo: 2 semanas.
    *   Responsável: Gerente de QA.

### 13.2.7. Padronizar o Sucesso (Atuar)

*   **Objetivo:** Incorporar soluções eficazes ao trabalho padrão.
*   **Exemplo:** Se os novos testes automatizados reduziram os incidentes, **torná-los parte da suíte oficial**.

**Exemplo Prático: A3 aplicado na Nordstrom**

*   **Problema:** Incidentes frequentes em produção.
*   **Causa identificada:** Exceções manuais e baixa automação.
*   **Contramedida testada:** Remoção do processo de exceção e introdução de gates.
*   **Resultado:** Redução significativa no tempo de ciclo e nos incidentes.
*   **Padronização:** Scripts automatizados foram incluídos no repositório oficial de testes.

**Dicas e Considerações**

*   O **tempo investido nas etapas 1–4** (planejamento) **é o mais importante**.
*   Evite "pular" direto para a execução.
*   Use o A3 como **ferramenta de aprendizado organizacional** — não apenas para correção de falhas.
*   Pode ser usado para **problemas técnicos, de processo ou culturais**.

## 13.3. Comparação com o Kata de Melhoria

**Aspecto**

**Kata de Melhoria**

**Estrutura A3**

Origem

Toyota Production System

Toyota Production System

Ênfase

Iterações rápidas e orientação a metas

Diagnóstico profundo e solução durável

Aplicação

Melhoria contínua

Resolução estruturada de problemas

Base metodológica

PDCA + metas intermediárias

PDCA + análise detalhada

Melhor uso

Evolução constante

Situações específicas de problema

# 14\. Modelo de Westrum

Ron Westrum é sociólogo e pesquisador especializado em **fatores humanos em sistemas de alta complexidade**, como:

*   Aviação
*   Saúde
*   Engenharia de software

Em 1988, Westrum propôs uma **tipologia de culturas organizacionais**, com foco em **segurança e fluxo de informação**.

## 14.1. Os 3 Tipos de Cultura segundo Westrum

**Cultura**

**Características principais**

**Foco**

**Patológica**

Medo, silos, punição, ocultação de informações

**Poder**

**Burocrática**

Regras rígidas, protecionismo de departamentos

**Regras**

**Generativa**

Colaboração, confiança, foco na missão e no desempenho

**Resultados/Desempenho**

## 14.2. Quadro Comparativo: Comportamentos por Tipo de Cultura

**Comportamento**

**Patológica**

**Burocrática**

**Generativa**

Cooperação

Baixa

Moderada

**Alta**

Tratamento dos mensageiros

Punidos

Ignorados

**Treinados**

Responsabilidade

Evitada

Restrita

**Compartilhada**

Formação de pontes

Desencorajada

Tolerada

**Incentivada**

Resposta ao fracasso

Culpabilização

Justiça/formal

**Investigação**

Atitude em relação à novidade

Rejeitada

Problematizada

**Implementada**

**Cultura Generativa** é o ideal para equipes DevOps — promove colaboração, experimentação e aprendizado contínuo.

## 14.3. O Fluxo de Informação nas Culturas

Westrum afirma que **a forma como a informação flui na organização reflete sua cultura**. Boas informações são:

1.  **Relevantes** – Respondem às perguntas certas.
2.  **Oportunas** – Chegam no momento necessário.
3.  **Utilizáveis** – Apresentadas de forma clara e acionável.

Em culturas generativas, essas características são comuns e fortalecem a **resposta a falhas e o aprendizado organizacional**.

## 14.4. Conexão com o DevOps

**Por que a cultura generativa é essencial?**

*   **Colaboração verdadeira** entre equipes de Dev, Ops, QA, segurança e negócio.
*   **Compartilhamento de responsabilidades** ao invés de repassar problemas.
*   **Rapidez na identificação e resolução de falhas**.
*   **Maior adaptabilidade** às mudanças e inovações tecnológicas.

**Evidência empírica: livro _Accelerate_**

Segundo o livro _Accelerate_, **a cultura organizacional é um preditor confiável de:**

*   Velocidade e qualidade na **entrega de software**.
*   **Desempenho organizacional** como um todo.
*   **Satisfação e retenção de talentos**.

## 14.5. Cultura Generativa: 3 Mecanismos Fundamentais

1.  **Colaboração eficaz**: altos níveis de confiança horizontal e vertical.
2.  **Foco na missão**: interesses pessoais/departamentais são deixados de lado.
3.  **Equidade nas interações**: hierarquia reduzida e decisões mais rápidas.

## 14.6. Benefícios de uma Cultura Generativa

*   Feedbacks mais rápidos e precisos.
*   Equipes mais resilientes e adaptáveis.
*   Melhor aproveitamento de incidentes como oportunidades de aprendizado.
*   Maior capacidade de inovação contínua.
*   Entrega de software mais confiável e eficaz.

Uma cultura generativa **não é opcional** para o sucesso do DevOps — ela é a base.
Transformações bem-sucedidas dependem da **mudança de mentalidade**, **práticas seguras de aprendizado** e **confiança entre pessoas e equipes**.

# 15\. Filosofias de Liderança no DevOps e Lean

Liderar no contexto de DevOps **exige mais do que conhecimento técnico**.
Exige **coragem, empatia, humildade, disciplina e compromisso com o aprendizado contínuo**.

Se liderarmos com essas filosofias em mente, **criamos culturas generativas**, onde equipes inovam, aprendem e entregam com excelência.

Acompanhar e classificar o trabalho da equipe ajuda a entender **onde está o esforço real**. As principais categorias são:

**Categoria**

**Descrição**

**Recursos**

Desenvolvimento de novas funcionalidades.

**Dívida Técnica**

Refatorações, melhorias de código, automações.

**Trabalho Operacional**

Suporte ao sistema, manutenção, tarefas rotineiras.

**Trabalho Não Planejado**

Incidentes, descobertas técnicas, interrupções.

## 15.1. Honrar e Extrair a Realidade

*   _Honrar a realidade_ significa reconhecer os fatos como eles são, sem negar ou minimizar.
*   _Extrair a realidade_ vai além: é criar um ambiente **onde as pessoas se sintam seguras para relatar problemas reais**.
*   Evite perguntas do tipo “**Quem fez isso?**”. Use perguntas como:
    *   “**Como isso aconteceu?**”
    *   “**Como podemos aprender com isso?**”
*   _“O fracasso leva à investigação, não à culpa.”_

## 15.2. Entender o Trabalho (Gemba)

*   Inspirado no conceito Lean de **Gemba** (o local real onde o trabalho acontece).
*   Não é microgerenciamento: é **ir para ver, não ir para mandar**.
*   Permite que o líder compreenda os desafios reais enfrentados pelas equipes.
*   Mostra comprometimento genuíno com o sucesso do time.

## 15.3. Erro Humano não é causa raiz

*   Em sistemas complexos, **há múltiplos fatores contribuintes** para falhas.
*   A pergunta não deve ser _"Quem causou isso?"_, mas sim:
    *   “**O que no sistema permitiu que isso acontecesse?**”
    *   “**Como podemos evitar que ocorra novamente?**”
*   Liderança eficaz **cultiva aprendizado, não busca culpados**.

## 15.4. Liderar pelo Exemplo

*   As ações do líder **devem refletir seus valores declarados**.
*   Coerência entre discurso e prática é essencial — especialmente em momentos de crise.
*   Se você diz que valoriza uma **cultura generativa**, **suas ações devem sustentá-la**.

## 15.5. Direcionamento Estratégico, Prioridade e Foco

*   Líderes devem:
    *   Oferecer **clareza sobre objetivos e direção**.
    *   Reduzir distrações e mudanças de prioridade.
    *   **Disciplinar o foco** para evitar trocas de contexto frequentes.

## 15.6. Capacitação com Intenção

*   Empowerment **não é só “dar liberdade”** — envolve:
    *   **Intenção**: visão clara do que se quer alcançar.
    *   **Contexto**: informações e entendimento para tomar boas decisões.
    *   **Responsabilidade**: entendimento dos resultados esperados.
*   Com esses elementos, **as equipes são realmente capacitadas** para agir com autonomia.

## 15.7. Ser um Eterno Aprendiz

*   O líder deve buscar **crescimento contínuo**, dentro e fora da organização.
*   Inclui:
    *   Participar de comunidades externas.
    *   Aprender com outros líderes.
    *   Tentar coisas novas, mesmo fora da zona de conforto.
*   _“Aprendizado exige persistência e entrega resiliência.”_

## 15.8. Respeito às Pessoas

*   Pessoas são o **ativo número 1** de qualquer organização.
*   O respeito ao indivíduo é a base do Lean e do DevOps.
*   Devemos criar ambientes onde as pessoas:
    *   São valorizadas.
    *   Podem errar e aprender.
    *   Têm voz nas decisões.

**Filosofia**

**Prática na Liderança**

Honrar & Extrair a Realidade

Estimular a verdade e eliminar a cultura do medo

Ir ao Gemba

Ver o trabalho onde ele acontece

Fracasso → Investigação

Aprender com erros sem culpabilização

Liderar pelo Exemplo

Ações coerentes com discurso

Direcionamento & Foco

Clareza estratégica e disciplina

Capacitação com Contexto

Autonomia guiada por propósito e responsabilidade

Aprendizado Contínuo

Liderança com humildade e crescimento

Respeito às Pessoas

Cultura centrada no humano

# 16\. Métricas e Resultados no DevOps

## 16.1. Outputs vs Outcomes

O que é um Output?

É o que é entregue:

*   Nova funcionalidade;
*   Correções de bugs;
*   Tickets resolvidos;
*   Releases publicados.

O que é um Outcome?

É o resultado real gerado por esses outputs:

*   Aumento de receita;
*   Maior retenção de clientes;
*   Redução de churn;
*   Maior eficiência operacional.

**DevOps de verdade não foca na entrega, mas no valor gerado por ela.**

Medir resultados com foco em outcomes — e não apenas outputs — **é um divisor de águas no DevOps moderno**.
Organizações de alto desempenho:

*   Automatizam o que é repetitivo;
*   Reduzem o risco com mudanças pequenas;
*   Focam em entrega contínua de valor;
*   Mantêm uma cultura de alta confiança e engajamento.

## 16.2. Os Dois Grandes Resultados Esperados

Quase toda organização quer:

1.  **Aumentar receita** (crescimento, inovação, experiência do cliente);
2.  **Reduzir custos** (eficiência, automação, estabilidade).

DevOps entrega valor exatamente nesses dois eixos — **automatizando, integrando, reduzindo erros e acelerando entregas**.

## 16.3. Métricas-Chave do DevOps

### 16.3.1. Deployment Pain (Dor de Implantação)

**O quão doloroso é lançar algo em produção?**

*   Muitas pessoas envolvidas? Salas de guerra? Noites viradas?
*   🔁 Solução: **Automatização, releases menores, deploy contínuo.**

### 16.3.2. Deployment Frequency (Frequência de Deploy)

**Com que frequência você entrega valor?**

*   Org. de alto desempenho: **várias vezes por dia**, sob demanda.
*   Relação direta com a dor de implantação — menos dor → mais deploy.

### 16.3.3. Change Failure Rate (Taxa de Falha de Mudanças)

**Quantas mudanças quebram algo na produção?**

*   Ideal: **0% a 15%**.
*   Técnicas eficazes:
    *   Releases pequenos e reversíveis;
    *   Uso de **feature flags**;
    *   Rollbacks automáticos.

### 16.3.4. Lead Time for Change (Tempo de Espera para Mudança)

**Quanto tempo leva entre a ideia e o código em produção?**

*   Org. de elite: **menos de uma hora**.
*   Combinação de **entrega contínua + cloud + testes automatizados.**

### 16.3.5 MTTR — Mean Time To Restore

**Quanto tempo leva para restaurar um serviço?**

*   Objetivo: < 1 hora.
*   Envolve:
    *   **Monitoramento eficaz**;
    *   **Alertas úteis**;
    *   **Resiliência arquitetural** (ex: blue-green deploys).

### 16.3.6. Percentual de Trabalho Não Planejado

**Quanto tempo sua equipe perde com incêndios?**

*   Incidentes inesperados → roubam capacidade da entrega de valor.
*   Planejamento adequado = espaço para inovação + menor burnout.

### 16.3.7. eNPS — Employee Net Promoter Score

**Funcionários indicariam a empresa para amigos?**

*   Perguntas:
    *   “Você indicaria sua equipe?”
    *   “Você indicaria sua empresa?”
*   Pontuação de 0 a 10.
*   Equipes com eNPS alto normalmente:
    *   São **autônomas**;
    *   Têm **clareza de propósito**;
    *   Dominam **toda a stack** ("você constrói, você opera").

Altos níveis de eNPS estão **correlacionados com maior performance** de software.

Equipes com alto eNPS:

*   *   *   Têm mais conexão com a missão da empresa.
        *   Entregam mais valor.
        *   São mais resilientes.
        *   São mais felizes e menos propensas ao burnout.

**Cálculo:** eNPS = % Promotores – % Detratores

**Pontuação**

**Classificação**

9–10

Promotor

7–8

Passivo

0–6

Detrator

**Métrica**

**O que mede**

**Bons resultados são**

Deployment Pain

Dificuldade para colocar no ar

Baixa dor, alta automação

Deployment Frequency

Frequência de entrega

Várias vezes por dia

Change Failure Rate

Mudanças que causam falhas

Menos de 15%

Lead Time for Change

Tempo entre ideia e deploy

Menos de 1h

MTTR

Tempo para restaurar serviços

Menos de 1h

Trabalho não planejado

Incidentes e interrupções

Muito baixo

eNPS

Engajamento dos colaboradores

Acima de 8

## 16.4. Ferramentas que podem ajudar

*   **Jenkins, GitHub Actions, GitLab CI/CD** → automação de deploy;
*   **LaunchDarkly, Unleash** → feature flags;
*   **Datadog, New Relic, Prometheus** → monitoramento e MTTR;
*   **Jira, Azure Boards, Trello** → backlog e lead time;
*   **CultureAmp, Officevibe, Google Forms** → medir eNPS.

# 17\. Gerenciando Riscos com DevOps

## 17.1. O que é gerenciamento de riscos no contexto de DevOps?

Assim como no Agile ou Lean, o DevOps também enfrenta resistência sob o argumento de que pode **aumentar o risco**, especialmente ao permitir que os próprios times de desenvolvimento implementem mudanças em produção. Essa percepção é comum entre gestores acostumados a modelos tradicionais de controle e **processos de aprovação manual**.

Contudo, essa resistência geralmente está baseada em **mitos**. Muitas vezes, os processos existentes de gerenciamento de mudanças funcionam apenas como **checklists burocráticos**, que não evitam falhas — apenas dão uma **falsa sensação de controle**.

Jez Humble chama isso de **"Teatro de Gerenciamento de Riscos"**: fazemos parecer que estamos mitigando riscos, mas, na prática, estamos apenas cumprindo processos ineficazes.

Em vez de priorizar documentação e aprovações formais, o DevOps foca em:

*   **Automatização de mudanças** (CI/CD).
*   **Feedback rápido e contínuo**.
*   **Monitoramento e telemetria em tempo real**.
*   **Propriedade total do ciclo de vida pelo time** (do desenvolvimento à produção).
*   **Redução do tempo médio de recuperação (MTTR)** em caso de falhas.

Essas práticas aumentam a **estabilidade real**, ao contrário da rigidez dos processos formais que apenas controlam a execução.

## 17.2. DevOps x ITIL: Conflitos e convergências

**ITIL (Biblioteca de Infraestrutura de TI)**

Inclui práticas formais como:

*   Gerenciamento de mudanças
*   Liberação
*   Configuração
*   Incidentes e problemas
*   Gerenciamento de conhecimento

**Onde surgem os conflitos?**

*   O ITIL recomenda **separação de funções**: uma equipe desenvolve, outra libera.
*   O DevOps **integra o ciclo inteiro** na mesma equipe, promovendo **responsabilidade compartilhada**.
*   O ITIL valoriza **aprovações manuais e rastreabilidade documental**.
*   O DevOps prioriza **rastreabilidade automatizada e entrega frequente**.

A prática de DevOps não substitui o controle — ela **o reinventa** com foco em **dados e resultados reais**.

## 17.3. Como mitigar riscos com DevOps

**Estratégias eficazes incluem:**

*   **Automação de testes** e pipelines de entrega.
*   **Monitoramento contínuo** com alertas proativos.
*   **Trilha de auditoria técnica** das mudanças (logs, commits, pipelines).
*   **Divisão das mudanças em pacotes menores**, entregues com maior frequência.
*   **Tempo de recuperação reduzido**: foco em restaurar o serviço rapidamente, se algo falhar.

**O problema das "janelas de congelamento"**

**O que são?**

Períodos, geralmente em eventos de alto impacto (ex.: Black Friday), nos quais **mudanças são proibidas** para evitar riscos.

**Quais os problemas?**

*   Acumulam mudanças por semanas, criando **grandes lotes**.
*   Elevam o risco de **grandes incidentes**.
*   Reduzem a **agilidade de resposta** a necessidades do mercado.

## 17.4. A verdadeira métrica de risco

Não se trata de seguir checklists. A verdadeira métrica está em:

*   **Frequência e qualidade das entregas**
*   **Tempo de recuperação (MTTR)**
*   **Taxa de sucesso das mudanças**
*   **Capacidade da equipe em responder a falhas rapidamente**

O foco deve estar em **resultados e capacidades**, e não em **documentação ou aprovações formais**.

# 18\. Como Lidar com Trabalho Não Planejado

Trabalho não planejado é toda atividade que interrompe o fluxo normal de trabalho da equipe sem ter sido prevista ou priorizada formalmente. Pode se manifestar como:

*   Incidentes em produção
*   Solicitações inesperadas
*   Descobertas técnicas tardias
*   Mudanças de prioridade
*   Perguntas "rápidas" que tomam horas

## 18.1. Tipos de Trabalho Não Planejado

### 18.1.1. Incidentes e interrupções

Exemplo clássico: um problema em produção interrompe o trabalho para correção emergencial.

**Impacto**: desvia o foco da equipe, atrasa entregas planejadas e sobrecarrega emocionalmente os membros.

### 18.1.2. Descoberta Técnica

Atividades como:

*   Entendimento de requisitos vagos
*   Pesquisas técnicas para viabilidade
*   Exploração de soluções antes do desenvolvimento

**Descoberta** é frequentemente ignorada como trabalho formal, mas é altamente disruptiva se não for planejada.

### 18.1.3. Troca de contexto (context switching)

Ocorre quando:

*   As prioridades mudam com frequência
*   Equipes são designadas a múltiplos projetos
*   Há interrupções frequentes com novas tarefas

**Problema**: gera perda de foco, menor produtividade e **queda de qualidade**.

## 18.2. Estratégias

### 18.2.1. Rastreie o trabalho não planejado

“Você não consegue melhorar o que não mede.”

Rastrear o trabalho não planejado ajuda a:

*   Entender seu volume real
*   Quantificar o impacto na entrega
*   Justificar mudanças no modelo de trabalho

### 18.2.2. Minimize a troca de contexto

**Como fazer isso?**

*   Priorize com clareza: uma prioridade de cada vez
*   Evite múltiplas alocações de equipe
*   Centralize a definição de prioridades em instâncias estratégicas
*   Crie espaços para trabalho focado sem interrupções

Multitarefa é superestimada. Troca de contexto **não é produtividade**, é desperdício.

### 18.2.3. Planeje capacidade para descoberta

Inclua nas estimativas:

*   Tempo para refinar requisitos
*   Análise técnica preliminar
*   Prototipagem ou spikes técnicos

Essa prática evita que a descoberta se torne um **trabalho emergencial**.

### 18.2.4. Arquitetura com acoplamento frouxo

Equipes com **autonomia para testar, implantar e operar** suas próprias entregas reduzem:

*   Interdependências
*   Espera por outros times
*   Ambientes complexos e sincronizados

Sistemas frouxamente acoplados ajudam a isolar problemas e reduzir o impacto de interrupções.

### 18.2.5. Integre e capacite a equipe

*   Envolva operações, qualidade e segurança desde o início
*   Crie times multifuncionais com **propriedade de ponta a ponta**
*   Automatize testes e deploys
*   Gere visibilidade com telemetria e métricas

O trabalho não planejado é inevitável, mas pode ser **reduzido, previsto e gerenciado** com boas práticas:

**Problema**

**Solução**

Incidentes em produção

Automatização, CI/CD, testes integrados

Solicitações inesperadas

Backlog emergencial, triagem central

Descoberta técnica

Reservar tempo no planejamento

Troca de contexto

Priorização clara e alinhamento estratégico

Dependências entre equipes

Arquitetura com acoplamento frouxo

# 19\. Tornando o trabalho visível

*   Permite compreender **a real capacidade da equipe**.
*   Ajuda a identificar **gargalos**, **bloqueios** e **desvios de foco**.
*   Cria espaço para **negociação de prioridades** com base em dados, não em suposições.
*   Revela **trabalho não planejado**, muitas vezes invisível e altamente disruptivo.

## 19.1. Métodos e Ferramentas para Tornar o Trabalho Visível

**Formas comuns:**

**Método**

**Descrição**

**Quadro Kanban físico**

Quadro com colunas como "A fazer", "Em progresso", "Concluído".

**Quadros digitais**

Ferramentas como Jira, Trello, Azure Boards, Asana.

**Importante:**
Não importa a ferramenta, mas sim **engajar a equipe e capturar o trabalho real.** Faça experimentos com ferramentas até encontrar a que mais funciona para sua equipe.

## 19.2. O Que Observar ao Tornar o Trabalho Visível

**Comportamentos típicos revelados:**

*   **Trabalho em lotes grandes** → dificuldade de entrega contínua.
*   **Trabalho parado** em "Em andamento" → indício de bloqueios.
*   **Trabalho não planejado** → causa de desvios e atrasos.
*   **Distribuição desbalanceada** entre tipos de trabalho → problemas estruturais (ex: foco excessivo em novos recursos sem cuidar da dívida técnica).

## 19.3. Categorias Úteis de Classificação do Trabalho

Muitas organizações classificam o trabalho em:

*   **Funcionalidades** (features)
*   **Operacional**
*   **Conformidade e risco**
*   **Dívida técnica**
*   **Trabalho não planejado**

**Nota:** As definições podem variar entre equipes. O importante é manter a consistência e a rastreabilidade.

## 19.4. Priorização Baseada em Realidade

Tornar o trabalho visível ajuda a **quebrar com a priorização ilusória**, baseada em desejos e compromissos desconectados da capacidade real.

**Como isso se traduz na prática:**

*   **Previsão mais realista de entregas.**
*   **Melhor comunicação com stakeholders.**
*   Possibilidade de **planejar o trabalho não planejado**, alocando capacidade para ele no backlog.

**Tornar o Trabalho Visível Também Reduz Carga Cognitiva**

*   Times deixam de trabalhar “no escuro”.
*   A visibilidade reduz a **ansiedade causada por sobrecarga**.
*   Cria uma cultura de transparência e confiança.

## 19.5. Ciclo de Melhoria com Visibilidade

1.  **Capturar** o trabalho atual.
2.  **Observar** gargalos e padrões.
3.  **Discutir** dados com a equipe.
4.  **Ajustar** prioridades e metas com base em fatos.
5.  **Repetir** mensalmente para gerar aprendizado e melhoria contínua.

# 20\. Trabalho em Processo (WIP)

Muito trabalho em andamento (WIP) gera:

*   **Baixo foco**
*   **Mais retrabalho**
*   **Ciclos de entrega mais longos**
*   **Maior sobrecarga cognitiva**
*   **Maior risco de falhas e esquecimentos**

Limitar o WIP melhora o **fluxo**, **qualidade**, e **previsibilidade** do trabalho.

## 20.1. O Que São Limites de WIP?

**Limites de WIP** (Work in Progress) são restrições deliberadas sobre **quantas tarefas** podem estar sendo executadas simultaneamente em uma etapa ou por uma equipe.

**Exemplo prático:**

Em um quadro Kanban, você pode limitar a coluna “Em andamento” a 3 itens. Só é possível iniciar algo novo quando algum item for concluído.

## 20.2. Por Que Só Limitar WIP Não Basta?

Para gerar resultados reais, você precisa:

**Prática**

**Função no sistema**

**Limite de WIP**

Reduz multitarefa

**Tela visual (ex: Jira)**

Torna gargalos visíveis

**Ciclos de feedback**

Ligam desenvolvimento à operação

**Dados de produção**

Informam decisões de melhoria

## 20.3. Os 5 Ladrões do Tempo (Dominica DeGrandis)

**Ladrão do tempo**

**Como contribui para excesso de WIP**

**1\. Muito trabalho**

Equipe assume mais do que pode concluir

**2\. Prioridades conflitantes**

Gera troca de contexto e distrações

**3\. Dependências ocultas**

Equipe começa múltiplas tarefas para tentar avançar

**4\. Trabalho não planejado**

Interrupções constantes elevam o WIP

**5\. Trabalho negligenciado**

Itens esquecidos permanecem em aberto, acumulando WIP

## 20.4. Como Aplicar Limites de WIP com Sucesso

**Estratégias recomendadas:**

1.  **Comece pequeno.**
    Limite uma única etapa do fluxo (ex: “Em andamento” → máximo 2 tarefas por dev).
2.  **Use sistema puxado.**
    Só puxe nova tarefa **quando concluir** a atual.
3.  **Incorpore no Kanban.**
    Configure limites visuais em ferramentas como Jira, Trello ou quadros físicos.
4.  **Exercite a enxameação.**
    Se há tarefas bloqueadas, junte a equipe para resolvê-las em vez de começar algo novo.
5.  **Negocie com as partes interessadas.**
    Mostre resultados concretos (tempo de entrega menor, menos retrabalho, mais qualidade).

**Resultado**

**Impacto Real**

Tempo de ciclo menor

Entregas mais rápidas

Redução de multitarefa

Mais qualidade e foco

Menos bloqueios e gargalos

Fluxo contínuo

Planejamento e previsibilidade

Decisões mais acertadas

Menor sobrecarga cognitiva

Engajamento da equipe

Visibilidade de impedimentos reais

Apoio da liderança
