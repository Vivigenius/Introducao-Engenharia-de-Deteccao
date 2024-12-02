# Introducao-Engenharia-de-Deteccao


![image](https://github.com/user-attachments/assets/be255adc-4229-4d48-9e04-943b31d20472)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Tarefa 2


O que é Engenharia de Detecção?


﻿Engenharia de Detecção
A segurança cibernética está crescendo e evoluindo em ritmo acelerado, agravada pelo progresso feito na tecnologia. Com isso, as ações dos adversários também estão evoluindo, e os ataques cibernéticos estão se tornando tão desenfreados e sofisticados que é difícil acompanhá-los. Além disso, as equipes de segurança devem desenvolver e se adaptar a novas mentalidades e práticas que as ajudarão a acompanhar os adversários. É aí que entra a engenharia de detecção.

A engenharia de detecção é o processo contínuo de construção e operação de análise de inteligência de ameaças para identificar atividades potencialmente maliciosas ou configurações incorretas que podem afetar seu ambiente. Ela requer uma mudança cultural com o alinhamento de todas as equipes de segurança e gerenciamento para construir sistemas de defesa eficazes e ricos em ameaças.

Tipos de detecção
A detecção de ameaças pode ser vista de duas perspectivas, cada uma compreendendo duas categorias: A primeira,  Detecção baseada em ambiente  , foca em olhar para mudanças em um ambiente com base em configurações e atividades de linha de base que foram definidas. Dentro dessa detecção, temos Detecção de configuração e Modelagem.

Na segunda perspectiva,   a detecção baseada em ameaças foca em elementos associados à atividade de um adversário, como táticas, ferramentas e artefatos que identificariam suas ações. Sob isso, temos detecções de Indicadores e Comportamento de Ameaça.

Detecção de configuração
Sob essa detecção, usamos o conhecimento atual do ambiente e infraestrutura conhecidos para identificar desalinhamentos. As configurações podem cruzar domínios, incluindo rede, ativo ou identidade.

A detecção de configuração tem os seguintes benefícios e desafios:
![image](https://github.com/user-attachments/assets/76cbb326-1ac7-4f42-875c-669981a075c1)


Modelagem

A detecção de ameaças sob esse tipo é feita definindo operações e atividades de linha de base e registrando quaisquer desvios que ocorram. A suposição primária dessa abordagem é que a atividade maliciosa pode ser suficientemente identificada a partir de atividade benigna.

A abordagem envolve a construção de um perfil de ativo ou atividade que inclui eventos de linha de base, tempo e limite de dados. Uma análise aprofundada da linha de base será discutida na próxima tarefa.

Alguns dos benefícios e desafios deste método de detecção incluem o seguinte:
![image](https://github.com/user-attachments/assets/0428308d-24ef-4166-a990-0af3a7942cac)


Detecção de Indicadores

Como lembrete, indicadores são pedaços de informação que identificam um estado e contexto de um elemento ou entidade. Existem goodindicadores usados ​​para identificar atividades ou recursos legítimos, como aqueles usados ​​em listas de permissões, e bad indicadores usados ​​para recursos suspeitos ou maliciosos, como em listas negras ou IPs de malware.

IOCs são comumente referenciados e derivados de investigações contra eventos maliciosos. Ao observar atividades de ameaças e investigações, analistas podem usar indicadores identificados para elaborar detecções e adaptá-las com base na taxa de mudança de um adversário.

Alguns dos benefícios e desafios deste método de detecção incluem o seguinte:
![image](https://github.com/user-attachments/assets/927c2b6c-891c-4989-a71c-210351691bba)


Detecção de comportamento de ameaça
Os analistas observarão as Táticas, Técnicas e Procedimentos (TTPs) de um adversário para conduzir um ataque, independentemente de quaisquer indicadores específicos. Isso torna a detecção mais escalável além dos indicadores.

Por meio dessa detecção, os analistas podem concentrar seus esforços de forma mais eficiente em responder à ameaça e mitigá-la em vez de utilizar tempo e recursos para entender como e por que os alertas foram acionados. Além disso, a detecção de comportamento de ameaça pode ser pareada com fluxos de trabalho e playbooks estabelecidos para fornecer as melhores práticas que podem ser seguidas durante uma investigação.

Alguns dos benefícios e desafios deste método de detecção incluem o seguinte:
![image](https://github.com/user-attachments/assets/d8b0784f-2b49-46b2-8eaf-111b0aa892fb)

A combinação dessas formas de detecção resulta em sistemas de defesa mais robustos. Por exemplo, a detecção baseada em modelo pode ser fortalecida com detecção de configuração liderada por especialistas para reduzir as chances de falsos positivos lançarem alertas.

Detecção como código
Detection as Code (DaC) é uma abordagem estruturada para escrever detecções incorporando princípios de melhores práticas de engenharia de software. Isso significa que engenheiros e analistas de detecção lidarão com processos de detecção e lógica como código, oferecendo escalabilidade para lidar com ambientes em rápida mudança e capacidades adversárias.

O DaC oferece um fluxo de trabalho orientado a código que cria processos de detecção ajustados que introduzem elementos críticos encontrados em fluxos de trabalho de Integração Contínua/Desenvolvimento Contínuo ( CI / CD ). Alguns desses elementos incluem:

Controle de versão: A maioria dos SIEMs e produtos EDR não têm a capacidade de rastrear alterações feitas em alertas e suas definições. Ao introduzir o controle de versão, as regras e processos de detecção podem ser rapidamente revisados, testados e contabilizados, permitindo detecções de maior qualidade.

Fluxos de trabalho de automação: ao adotar um fluxo de trabalho de CI / CD , os testes de detecção podem ser automatizados e permitir transição e entrega de produção rápidas.
Com isso, a Detecção como Código proporciona os seguintes benefícios:

Detecções personalizáveis ​​e flexíveis: usar uma linguagem comum para detecções, como Sigma e YARA, oferece uma oportunidade para o DaC ser independente de fornecedor e ser implantado em diversas soluções SIEM, EDR e XDR.

Desenvolvimento Orientado a Testes: Testes de qualidade do código de detecção podem garantir que pontos cegos e testes falso-positivos sejam identificados mais cedo no processo e promovam a eficácia da detecção. Além disso, essa abordagem melhora a qualidade das detecções e garante que elas sejam bem documentadas.

Colaborações em equipe: o uso de fluxos de trabalho de CI / CD elimina o isolamento entre equipes de segurança e promove a colaboração por meio do processo de codificação.

Reutilização de código: com os padrões de detecção surgindo ao longo do tempo, os engenheiros podem reutilizar o código para executar funções semelhantes em diferentes detecções, garantindo que o processo de detecção avance mais rápido, pois não haverá necessidade de começar do início.
![image](https://github.com/user-attachments/assets/5869a748-ecf6-4f75-ba29-8640087874ab)

RESPOSTAS DA TAREFA 2
![image](https://github.com/user-attachments/assets/7d2f5e69-e3f7-4cc2-9d4f-c8e2fc86d339)
EXPLICAÇÃO: Essa detecção usa o conhecimento atual do ambiente conhecido para identificar desalinhamentos, como explicado no texto acima.


![image](https://github.com/user-attachments/assets/fdf35103-31c6-4ec5-a3bb-e66559ce39d1)
EXPLICAÇÃO: Modelagem (modeling) é a resposta correta, pois a detecção envolve a criação de um perfil de ativos ou atividades para estabelecer uma linha de base e detectar quaisquer desvios que possam indicar atividade maliciosa.


![image](https://github.com/user-attachments/assets/ee2a8a3b-d2e3-45f4-a3f5-d96ee650789c)
EXPLICAÇÃO: Threat Behaviour está relacionado ao uso de táticas, técnicas e procedimentos (TTPs) do adversário, e pode ser facilmente integrado com playbooks defensivos e planos de remediação automatizados.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Tarefa 3


Metodologias de Engenharia de Detecção

Análise de Lacunas de Detecção
O primeiro passo envolve olhar para o ambiente e identificar áreas-chave onde as organizações podem melhorar a detecção de ameaças. Esse processo também é conhecido como modelagem de ameaças e pode ser feito das seguintes maneiras:

Reativo : avaliar os relatórios de incidentes internos mais recentes, anotar as lições aprendidas com os ataques e eliminar áreas de possível detecção que não foram identificadas.
Proativo : Usando a estrutura ATT&CK e várias fontes de inteligência de ameaças para mapear áreas potenciais de ataque e os vários TTPs que um adversário contra seu ambiente pode usar.
Observação: a modelagem de ameaças neste contexto difere do tipo de detecção discutido na tarefa anterior.

Identificação da fonte de dados e coleta de logs
Com informações sobre os atores de ameaças relevantes, TTPs e riscos potenciais que a organização pode enfrentar, fontes de dados relevantes associadas aos riscos precisam ser identificadas. Isso determinará quais logs estão disponíveis no momento que ajudarão a definir detecções contra as ameaças e saber quais estão faltando e quais são necessárias.

Criação de linha de base
Antes de usar todas as informações coletadas sobre adversários, seus TTPs e qualquer comportamento malicioso, os analistas de segurança precisam saber qual é o comportamento normal e definir suas linhas de base de segurança. Este será um processo contínuo e requer a participação de todos os departamentos dentro de uma organização.

A configuração de linhas de base de segurança envolve a identificação dos diferentes tipos de dispositivos em execução em uma organização com base em seu sistema operacional, serviços e funções. As linhas de base de segurança podem ser agrupadas em duas categorias:

Alto nível: define padrões amplos e independentes do sistema operacional, guiados por uma política de segurança especificada.
Técnico: Consiste em padrões de configuração baseados em SO descrevendo diferentes funções do sistema e os comportamentos ou atividades pretendidos. Por exemplo, linhas de base técnicas delineiam políticas de proteção do SO , atividades de rede, políticas de Gerenciamento de Identidade e Acesso ( IAM ) e políticas de aplicativo.
Coleção de Logs
Uma vez que as linhas de base e fontes de dados internos tenham sido identificadas e priorizadas, a coleta de logs e metadados úteis para detecção de ameaças deve ser feita. Dependendo da configuração da infraestrutura, um sistema centralizado pode agregar todos os logs usando sensores de rede para dados de rede e serviços como Sysmon para coletar dados do host.

Escrita de regras
Com base na configuração da infraestrutura e nos serviços SIEM, as regras de detecção precisarão ser escritas e testadas em relação às fontes de dados. As regras de detecção testam padrões anormais em relação a eventos registrados. O tráfego de rede seria avaliado por meio de regras Snort, enquanto as regras Yara avaliariam os dados do arquivo. Confira as salas Snort e Yara para mais informações.

Como parte do módulo de Engenharia de Detecção, veremos o Sigma , uma linguagem de assinatura genérica usada para escrever regras de detecção em arquivos de log.

Implantação, automação e ajuste
Regras de detecção testadas devem ser colocadas em produção para serem avaliadas em um ambiente ao vivo. Com o tempo, as detecções precisariam ser modificadas e atualizadas para levar em conta mudanças em vetores de ataque, padrões ou ambiente. Isso melhora a qualidade das detecções e encoraja a visualização da detecção como um processo contínuo.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Tarefa 4


Estruturas de Engenharia de Detecção 1


Estruturas ATT&CK e CAR do MITRE
O MITRE é bem conhecido por publicar CVEs identificados que os adversários procurariam explorar para suas atividades maliciosas. Além disso, o MITRE fornece acesso baseado em conhecimento que os analistas de segurança podem usar para rastrear táticas e técnicas comumente usadas por atores mal-intencionados em diferentes plataformas, como Windows, macOS, Linux e Mobile.

A estrutura ATT&CK ajuda a mapear ações adversas com base na infraestrutura em uso para engenharia de detecção. Ela orienta o que procurar, especialmente como parte da fase de análise de lacunas de detecção.

A base de conhecimento CAR ( Cyber ​​Analytics Repository ) é usada para detectar comportamentos adversários e priorizá-los com base na estrutura ATT&CK.
![image](https://github.com/user-attachments/assets/2c915e4b-e56a-48a2-91b4-9acd57583392)

Pirâmide da Dor
Esta é uma estrutura bem conhecida no setor e é usada principalmente para mostrar o problema para o adversário; se os defensores detectarem seus TTPs, quão difícil e/ou custoso seria para o adversário alterar seus TTPs.
![image](https://github.com/user-attachments/assets/243d1d96-3f3c-4848-a9b9-50cdebfafa1e)

Cadeia de destruição cibernética

Graças a um conceito militar de estratégia de ataque, a Lockheed Martin formulou a estrutura Cyber ​​Kill Chain para definir os passos necessários seguidos pelos adversários. A estrutura foca em sete fases cruciais que os ataques cibernéticos comumente seguem:

Reconhecimento
Armamento
Entrega
Exploração
Instalação
Comando e Controle
Ações sobre objetivos

![image](https://github.com/user-attachments/assets/bc885c24-0898-4eda-b426-fa4f384fcde2)

Como analista de segurança e engenheiro de detecção, entender a Cyber ​​Kill Chain lhe dará o conhecimento para reconhecer tentativas de intrusão criadas por um adversário e mapeá-las em seu plano de detecção. A Unified Kill Chain foi desenvolvida para complementar a Cyber ​​Kill Chain combinando-a com outras estruturas, como a estrutura MITRE ATT&CK. Isso expandiu a kill chain original em 18 fases para cobrir todos os elementos conhecidos de um ataque cibernético.
![image](https://github.com/user-attachments/assets/4f6f653e-06e1-447c-9c01-702c1e5fa1fb)


RESPOSTAS DA TAREFA 4
![image](https://github.com/user-attachments/assets/e04e3e8d-0c10-454d-9662-1e087221c357)
![image](https://github.com/user-attachments/assets/3c54fd7d-4ffb-4f22-935c-e7c0c60f7c34)
![image](https://github.com/user-attachments/assets/b1894a3e-a228-4734-818b-05962996f66d)


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Tarefa 5


Estruturas de Engenharia de Detecção 2



Estrutura de estratégia de alerta e detecção


A Palantir desenvolveu o ADS Framework para fornecer uma diretriz para documentar o conteúdo de detecção. Um desafio significativo enfrentado pelas equipes de segurança, e a Palantir não é exceção, é a fadiga e apatia de alerta, causadas principalmente por meios precários de desenvolver e implementar alertas de detecção que resultariam em resposta e mitigação de incidentes eficazes. O ADS Framework busca abordar esse desafio e fornecer uma diretriz para construir detecções e alertas eficazes.

O ADS Framework tem um fluxo rigoroso que os engenheiros de detecção devem seguir antes de publicar regras de detecção na produção. Os estágios envolvidos são:

Objetivo: Descreve os motivos pretendidos para configurar o alerta e o tipo de comportamento que precisa ser detectado.

Categorização: Mapeamento da detecção para a estrutura MITRE ATT&CK para fornecer aos analistas informações sobre os TTPs para investigação e áreas da cadeia de eliminação onde o ADS será usado.

Resumo da estratégia: fornece uma descrição de alto nível de como a estratégia de detecção que está sendo implementada funciona, descrevendo o que o alerta procurará, as fontes de dados, os recursos de enriquecimento e as maneiras de reduzir falsos positivos.

Contexto Técnico: Descreve o ambiente técnico da detecção a ser usada, fornecendo aos analistas e respondentes todas as informações necessárias para entender o alerta. Os analistas de segurança devem alinhar essas informações com as plataformas e ferramentas para coletar e processar alertas de ameaças.

Pontos Cegos e Suposições: Descreve quaisquer problemas identificados onde atividades suspeitas podem não acionar a estratégia. Suposições e pontos cegos ajudam a esclarecer maneiras pelas quais o ADS pode falhar ou ser ignorado por um adversário.

Falsos Positivos: Descreve ocorrências em que alertas podem ser disparados devido a configurações incorretas ou atividades não maliciosas dentro do ambiente. Isso facilita a configuração do seu SIEM para limitar a geração de alertas somente a ameaças direcionadas quando enviadas para produção.

Validação: Toda detecção precisa ser verificada, e aqui, você pode delinear todas as etapas necessárias para produzir um evento verdadeiro-positivo que acionaria o alerta de detecção. Considere isso um teste de unidade, que pode até ser um script ou cenário usado para gerar um alerta. Para uma validação eficaz:

Desenvolva um plano que produzirá um resultado verdadeiramente positivo.
Documente o processo do plano.
No ambiente de teste, teste e acione um alerta.
Valide a estratégia que disparou o alerta.

Prioridade: Configure os níveis de alerta com os quais a estratégia de detecção pode ser marcada. Esta seção fornece os detalhes dos critérios usados ​​para configurar as preferências e é separada dos níveis de alerta mostrados pelo SIEM .

Resposta: Fornece detalhes de como fazer a triagem e investigar um alerta de detecção. Essas informações são úteis para que analistas e respondentes possam evitar repercussões extremas.

![image](https://github.com/user-attachments/assets/6b061a71-5f75-4dfc-aabc-41823124a90b)


Modelo de nível de maturidade de detecção
Ryan Stillions apresentou o modelo Detection Maturity Level (DML) em 2014 como uma forma de uma organização avaliar seus níveis de maturidade em relação à sua capacidade de ingerir e utilizar inteligência de ameaças cibernéticas na detecção de ações adversárias. De acordo com Ryan, há dois princípios orientadores para este modelo:

A maturidade de uma organização não é medida por sua capacidade de obter informações valiosas, mas por sua capacidade de aplicá-las à detecção e resposta.
Sem funções de detecção estabelecidas, não há oportunidade de executar funções de resposta.
O modelo DML compreende nove níveis de maturidade dedicados, numerados de 0 a 8, com o menor valor representando aspectos técnicos de um ataque e o nível mais alto representando aspectos abstratos e baseados em inteligência de um ataque. Os níveis individuais podem ser descritos da seguinte forma:

Objetivos do DML-8: O auge do modelo representa organizações que podem detectar o motivo e os objetivos de um adversário. Infelizmente, é quase impossível conduzir detecções baseadas apenas em objetivos, pois, na maioria dos casos, é um jogo de adivinhação baseado em descobertas comportamentais de DMLs mais baixos.

Estratégia DML-7 : Seguindo de perto o DML-8, este nível não é técnico e representa as intenções e estratégias do adversário para cumpri-las. Organizações neste nível teriam uma fonte de inteligência madura que garantiria que elas tivessem contexto sobre os planos de um adversário, o que seria útil para os respondentes.

DML-6 Táticas: As organizações devem ser capazes de detectar uma tática sendo usada por um adversário sem necessariamente saber qual técnica ou ferramenta eles usaram. As táticas são detectáveis ​​após observar padrões de eventos que se agregam ao longo do tempo e das condições.

Técnicas DML-5: As técnicas geralmente são específicas para um indivíduo ou APT . Portanto, os adversários deixam para trás evidências de seus hábitos e comportamentos de ataque, e as organizações que podem detectar quando um determinado ator de ameaça está dentro de seu ambiente estão em vantagem.

Procedimentos DML-4: Organizações precisam detectar sequências de eventos de um adversário neste nível. Elas serão muito organizadas e seguirão um padrão dado, como o reconhecimento pré-exfiltração.

Ferramentas DML-3: A detecção de ferramentas pode cair em duas fases: a transfer phaseem que a ferramenta é baixada pela rede em um dispositivo host e reside em um sistema de arquivos ou na memória. E a segunda é a detecção por meio da ferramenta functionality and operation. Em alguns casos, esse nível de detecção exigiria que as organizações realizassem engenharia reversa contra ferramentas adversárias, dificultando causar estragos ao entender as capacidades de suas ferramentas.

DML-2 Host & Network Artefacts: A maioria dos recursos organizacionais seria gasta reunindo IOCs e artefatos como inteligência de ameaça neste nível. Infelizmente, na maioria dos casos, os indicadores são observados após o fato. O ator da ameaça provavelmente estaria causando estragos na rede quando os artefatos fossem detectados e investigados. Isso foi descrito como "perseguir o rastro de vapor de uma aeronave".

Indicadores atômicos DML-1: este nível abrange organizações que utilizam feeds de informações sobre ameaças na forma de listas de endereços IP e domínios para detectar ameaças.

DML-0 Nenhum: Na base do modelo, as organizações que operam neste nível não têm processos de detecção estabelecidos.

![image](https://github.com/user-attachments/assets/bc9886b0-e73b-4a8f-a4b7-dc1b1fc5876b)


Na publicação original do modelo DML, Ryan descreveu quatro casos de uso críticos para o modelo, a saber:

Fornecer um léxico para comunicação mais acessível de informações sobre ameaças.
Para avaliar a maturidade de detecção contra agentes de ameaças monitorados.
Avaliar a maturidade dos fornecedores e produtos de segurança em uso.
Fornecer contexto aos analistas incluindo os níveis DML nas regras Yara, assinaturas Snort e regras de correlação SIEM .





