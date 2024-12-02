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




