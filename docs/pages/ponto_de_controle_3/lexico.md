# <center> Léxicos V2

### Histórico de Versão
|    Data    | Versão | Descrição            | Autor(es)       |
| :--------: | :----: | :------------------: | :-------------: |
| 18/03/2021 |  1.0   | Criação do documento (v1) | Durval Carvalho, Leonardo Gomes e Victor Jorge |
| 05/04/2021 |  2.0   | Aplicações de correções no documento (v2) | Durval Carvalho |

##### Versões anteriores deste documento

- [Versão 1](pages/ponto_de_controle_3/lexico_v1.md)

<!-- Esse documento ainda será escrito -->

## 1. Introdução

Atividades associadas ao processo de requisitos podem envolver leitura de documentos que impactem de alguma forma o sistema em desenvolvimento. Exemplos de documentos incluem padrões da organização, legislação pertinente, atas de reuniões ou entrevistas ocorridas durante o processo de elicitação e também o próprio documento de requisitos sendo elaborado. Nesse processo, a construção do léxico da aplicação é tarefa prioritária, pois nele são registrados os símbolos próprios do domínio da aplicação. O léxico é a base para o entendimento entre clientes, usuários e profissionais de software. [Sayão, Carvalho, 2006]


## 2. Objetivo

O objetivo deste documento é documentar o símbolos e vocabulários utilizados nos documentos de requisitos desse projeto, visando assim criar um conhecimento  compartilhado,  diminuindo  dificuldades  de  entendimento  em  relação  a  termos  próprios  do  domínio  da  aplicação.


## 3. Léxico Amplicado da Linguagem - LAL

### Usuário
| | |
|-|-|
| **Nome** | Usuário |
| **Sinônimos** | Cliente, Utilizador |
| **Noção** | Termo que se refere às pessoas que utilizam o [aplicativo](#Aplicativo) |
| **Impacto** | O Usuário é o agente que realiza a maioria das ações no [aplicativo](#Aplicativo). Algumas das ações são: Criar [receitas](#Receita), pesquisar [receitas](#Receita), avaliar [receitas](#Receita), escolher [ingredientes](#Ingrediente) e outros. |
| **Classificação** | Sujeito |


### Saudável
| | |
|-|-|
| **Nome** | Saudável |
| **Sinônimos** | Sadio, Natural |
| **Noção** | Saudável é o estado que descreve [alimentos](#Comida) naturais e frecos. Sendo o objetivo do [aplicativo](#Aplicativo) agrupar [receitas](#Receita) de [alimento](#Comida) saudáveis. |
| **Impacto** | Além de saudáveis, os [alimentos](#Comida) podem ser não saudáveis, geralmente [alimentos](#Comida) processados, com alto teor de gordura e açúcar. |
| **Classificação** | Estado |

### Receita
| | |
|-|-|
| **Nome** | Receita |
| **Sinônimos** | Pratos |
| **Noção** | Uma receita é composta por [ingredientes](#Ingrediente) e é registrada por um [usuário](#Usuário) (comum ou um [Chef](#Cozinheiro)). O objetivo da receita é fazer um [alimento](#Comida) [saudável](#Saudável). |
| **Impacto** | Uma receita pode ser utilizada para se [preparar uma refeição](#preparar-receita). Para isso é preciso seguir os [passos](#Passo) e os [ingredientes](#Ingrediente) definidos na receita. |
| **Classificação** | Objeto |

### Passo
| | |
|-|-|
| **Nome** | Passo |
| **Sinônimos** | Etapa, atividade  |
| **Noção** | Ação realizada com um [ingrediente](#Ingrediente) visando a elaboração de uma [receita](#receita) |
| **Impacto** | Os passos podem ser executados pelos [usuários](#Usuário), conforme descritos na [receita](#Receita), para no fim se obter um [alimento](#Comida) |
| **Classificação** | Objeto |

### Comida
| | |
|-|-|
| **Nome** | Comida |
| **Sinônimos** | Alimento, Prato de Comida, Refeição |
| **Noção** | A comida é o resultado final obtido após a execução de todos os [passos](#Passo) definidos em uma [receita](#Receita), com determinados [ingredientes](#Ingrediente). |
| **Impacto** | Um alimento pode ser consumido |
| **Classificação** | Objeto |


### Ingrediente
| | |
|-|-|
| **Nome** | Ingrediente  |
| **Sinônimos** | Indicação |
| **Noção** | Os ingredientes são [alimentos](#Comida) que podem ser utilizados para [preparar]((#preparar-receita)) uma [receita](#receita) |
| **Impacto** | Os ingredientes são utilizados nas [receitas](#Receita). Os ingredientes são classificados de acordo com seu gosto e aroma. Os ingredientes são processados de diversas maneiras (cozinhados, assados, refogados, defumados, etc) |
| **Classificação** | Objeto |

### Anúncio
| | |
|-|-|
| **Nome** | Anúncio |
| **Sinônimos** | Indicação, propaganda, publicidade |
| **Noção** | Texto ou imagem publicitário que surge na tela de usuários não [Premium](#Premium). Os anúncios são uma fonte de receita provinientes de [usuários](#Usuário) que não pagam pelo [aplicativo](#Aplicativo) |
| **Impacto** | Os anúncios que aparecem na tela do [aplicativo](#Aplicativo) podem ser assistidos, clicados e fechados pelos usuários. |
| **Classificação** | Objeto |


### Premium
| | |
|-|-|
| **Nome** | Premium, Prime |
| **Sinônimos** | Assinatura paga |
| **Noção** | Todo [usuário](#Usuário) possui um plano de assinatura, podendo ser um plano gratuito ou um plano Premium. Um [usuário](#Usuário) com plano Premium tem acesso a funcionalidades que usuários com plano comum não tem. Sendo a principal delas a não visualização de [anúncios](#Anúncio) dentro do [aplicativo](#Aplicativo). |
| **Impacto** | Os planos dos usuários podem ser gratuítos ou Premium. A mudança do estado do plano está associado ao pagamento da assinatura do [aplicativo](#Aplicativo). |
| **Classificação** | Estado |


### Pesquisar Receita
| | |
|-|-|
| **Nome** | Pesquisar Receita |
| **Sinônimos** | Procurar receita, Buscar Receita  |
| **Noção** | Os usuários realizam pesquisas no aplicativo digitando termos e aplicando filtros. Os resultados obtidos são [receitas](#receita) que atendem aos critérios de pesquisa. |
| **Impacto** | O resultado dessa ação do [usuário](#Usuário) é a obtenção de uma lista de [receitas](#receita) que atendem aos critérios definidos pelo [usuário](#Usuário). |
| **Classificação** | Verbo |


### Preparar Receita
| | |
|-|-|
| **Nome** | Preparar Receita |
| **Sinônimos** | Cozinhar receita, Realizar Receita  |
| **Noção** | Uma [receita](#receita) é preparada por um [usuário](#Usuário) quando todos os [passos](#Passo) são seguidos, com determinados [ingredientes](#Ingrediente).
| **Impacto** | O resultado do preparo de uma [receita](#receita) é um [alimento](#Comida) [saudável](#Saudável). |
| **Classificação** | Verbo |

### Avaliar Receita
| | |
|-|-|
| **Nome** | Avaliar Receita |
| **Sinônimos** | Qualificar Receita, Dar nota |
| **Noção** | Os [usuários](#Usuário) quando acessam a página de detalhamento de uma [receita](#receita) pode avaliá-la, clicando no widget de avaliação. |
| **Impacto** | Uma [receita](#receita) com muitas avaliações se torna mais revelante, tendo maior destaque nos [resultados das pesquisas](#pesquisar-receita) e nos destaques na página inicial do [aplicativo](#Aplicativo). |
| **Classificação** | Verbo |

### Compartilhar uma Receita
| | |
|-|-|
| **Nome** | Compartilhar uma Receita |
| **Sinônimos** | Enviar o link de uma receita |
| **Noção** | Os [usuários](#Usuário) quando acessam a página de detalhamento de uma [receitas](#receita) pode clicar no widget de compartilhamento para enviar a receita para seus amigos |
| **Impacto** | Uma [receita](#receita) que recebe muitas visualizações de usuários se torna mais relevante, tendo maior destaque nos [resultados das pesquisas](#pesquisar-receita) |
| **Classificação** | Verbo |

### Fazer Login
| | |
|-|-|
| **Nome** | Compartilhar uma Receita |
| **Sinônimos** | Sign in, Entrar |
| **Noção** | O [usuário](#Usuário) ao entrar no [aplicativo](#Aplicativo) pela primeira vez ou após deslogar, pode se autentificar utilizando o email e senha, ou a conexão com alguma rede social previamente cadastrada. |
| **Impacto** | Após a autentificação o [usuário](#Usuário) irá carregar todos os dados previamente definidos ([receitas](#receita) favoritadas, configurações de conta, [restrições alimentares](#restrição-alimentar) registradas, etc.) |
| **Classificação** | Verbo |


### Fazer Cadastro
| | |
|-|-|
| **Nome** | Compartilhar uma Receita |
| **Sinônimos** | Sign up, registrar |
| **Noção** | O usuário pode criar uma conta no aplicativo utilizando email e senha ou a conexão com alguma rede social.
| **Impacto** | Após a realização do cadastro o [usuário](#Usuário) poderá acessar as principais funcionalidades do [aplicativo](#Aplicativo) e poderá perpeturar suas configurações.
| **Classificação** | Verbo |

### Estar Logado
| | |
|-|-|
| **Nome** | Estar Logado |
| **Sinônimos** | Estar autenticado, Estar identificado, acessando com autenticação |
| **Noção** | Logado é o estado da conta de um [usuário](#Usuário). A realização de um [cadastro](#Fazer-Cadastro) de conta ou de [login](#Fazer-Login) leva a esse estado. |
| **Impacto** | Uma conta logada pode ser deslogada ou deletada |
| **Classificação** | Estado |


### Restrição Alimentar
| | |
|-|-|
| **Nome** | Restrição Alimentar |
| **Sinônimos** | Restrição Alimentar, Limitação Alimentar |
| **Noção** | Uma conta com restrições alimentares são contas que foram definidas para não mostrar [receitas](#receita) que possuem [ingredientes](#Ingrediente) ingredientes na lista de [ingredientes](#Ingrediente) restritos. Para configurar uma conta com restrições alimentares o [usuário](#Usuário) deve adicionar [ingredientes](#Ingrediente) na lista de [ingredientes](#Ingrediente) restritos |
| **Impacto** | Uma conta pode se tornar "Com restrições alimentares" quando há [ingredientes](#Ingrediente) na lista de [ingredientes](#Ingrediente) restritos. |
| **Classificação** | Estado |


### Aroma
| | |
|-|-|
| **Nome** | Aroma |
| **Sinônimos** | Cheiro, Essência |
| **Noção** | Os aromas são características dos [ingredientes](#Ingrediente) |
| **Impacto** | Os aromas podem ser filtrados e utilizados para buscar [ingredientes](#Ingrediente) e [alimentos](#Comida). Esses aromas podem ser ou não recomendados na criação de uma [receita](#receita). |
| **Classificação** | Objeto |

### Sabores
| | |
|-|-|
| **Nome** | Sabores |
| **Sinônimos** | Gostos, Gustação |
| **Noção** | Os sabores são características associadas com os [ingredientes](#Ingrediente) |
| **Impacto** | Os sabores podem ser filtrados e utilizados para buscar [ingredientes](#Ingrediente) e [alimentos](#Comida). Esses sabores podem ou não ser recomendados na criação de uma [receitas](#receita). |
| **Classificação** | Objeto |


### Score
| | |
|-|-|
| **Nome** | Score |
| **Sinônimos** | Pontuação, Nota |
| **Noção** | Cada [receita](#receita) possui uma pontuação associada |
| **Impacto** | Os [usuários](#Usuário) avaliam as [receitas](#receita). |
| **Classificação** | Objeto |


### Roda de Sabores
| | |
|-|-|
| **Nome** | Roda de Sabores |
| **Sinônimos** | Tela de Sabores, Sabores da Receita |
| **Noção** | Na tela de descrição de uma [receita](#receita) é possível visualizar todos os [ingredientes](#Ingrediente) e seus respectivos [sabores](#sabores) e [aromas](#aromas), possibilitando assim uma rápida visualização dos [sabores](#sabores) e [aromas](#aromas) que aquela [receita](#receita) pode propocionar |
| **Impacto** | Os [usuários](#Usuário) analisam se as [receitas](#receita) propocionam a experiência gastronômica desejada |
| **Classificação** | Objeto |


### Porções
| | |
|-|-|
| **Nome** | Porções |
| **Sinônimos** | Fração, Fatias, Divisão |
| **Noção** | Porções são a quantidade de pessoas que uma determinada [receita](#receita) é capaz de servir. |
| **Impacto** | O [usuário](#Usuário) pode modificar a quantidade de porções aumentando ou diminuindo a quantidade de [ingredientes](#Ingrediente) que serão usados na [receita](#receita). O usuário também pode mudar a quantidade de [ingredientes](#Ingrediente) aumentando ou diminuindo a quantidade de porções que a [refeição](#Comida) deve servir |
| **Classificação** | Objeto |

### Logs de execução
| | |
|-|-|
| **Nome** | Logs de execução |
| **Sinônimos** | Histórico de execução |
| **Noção** | Os programas em execução salvam de tempos em tempos o histórico do programa, para que os desenvolvedores possam analisar comportamentos e erros |
| **Impacto** | Os desenvolvedores podem analisar os logs de execução enviados pelos [aplicativos](#Aplicativo) para futuros insights de erros de usabilidade e bugs  |
| **Classificação** | Objeto |

### Background
| | |
|-|-|
| **Nome** | Background |
| **Sinônimos** | Segundo Plano |
| **Noção** | Background é o estado de um [aplicativo](#Aplicativo) que foi iniciado mas não está em modo de exibição na tela do smartphone. [Aplicativos](#Aplicativo) nesse estado são carregados mais rapidamente e realizam algumas tarefas como downloads, alertas e etc. |
| **Impacto** | Um [aplicativo](#Aplicativo) pode está em fechado, em execução ou em background. |
| **Classificação** | Estado |

### Aplicativo
| | |
|-|-|
| **Nome** | Aplicativo |
| **Sinônimos** | App, Sistema, Plataforma |
| **Noção** | É um programa de computador concebido para processar dados eletronicamente, facilitando e reduzindo o tempo de execução de uma tarefa pelo usuário. O termo [aplicativo](#Aplicativo) geralmente se refere a uma classe de programas de computador que executam em dispositivos móveis. Neste contexto, o termo aplicativo se refere ao *Plant Jammer* em toda sua completude de funcionalidades. |
| **Impacto** | O aplicativo pode ser aberto, fechado, deletado de um smartphone. |
| **Classificação** | Objeto |

### Cozinheiro
| | |
|-|-|
| **Nome** | Cozinheiro |
| **Sinônimos** | Chef, [Usuário](#Usuário) |
| **Noção** | O cozinheiro tem uma atuação que exige habilidade com as panelas, nas combinações dos temperos e no corte certo das carnes. O profissional prepara todos os alimentos da cozinha e trabalha em conjunto com o chef de cozinha. |
| **Impacto** | O cozinheiro pode utilizar o [aplicativo](#aplicativo) publicando suas [receitas](#receita) ou adquirindo novos conhecimentos através de receitas de outros [usuários](#Usuário) |
| **Classificação** | Sujeito |

### Nome de usuário
| | |
|-|-|
| **Nome** | Nome de usuário |
| **Sinônimos** | Nick, apelido, codinome |
| **Noção** | O **nome de usuário** é o nome interno utlizado para identificar o [usuário](#usuário) dentro do [aplicativo](#aplicativo). O nome de usuário está diretamente vinculado à sua [conta](#conta) |
| **Impacto** | O nome pode ser alterado. O nome pode ser conferido na área de configurações da [conta](pages/ponto_de_controle_3/lexico?id=conta) |
| **Classificação** | Objeto |

### Conta
| | |
|-|-|
| **Nome** | [Conta](pages/ponto_de_controle_3/lexico?id=conta) |
| **Sinônimos** | Perfil, Perfil do usuário |
| **Noção** | É o registro interno do sistema que permite com que o [usuário](#usuário) acesse o [aplicativo](#aplicativo), e interaja com todas as suas funcionalidades salvando seu progresso. No perfil estão todas as informações conhecidas sobre o [usuário](#usuário). Todas as funcionalidades que envolvem metas, históricos, lembretes e favoritos dependem da existência de uma [conta](pages/ponto_de_controle_3/lexico?id=conta) ativa naquele contexto para funcionar. |
| **Impacto** | A [conta](pages/ponto_de_controle_3/lexico?id=conta) pode ser criada e excluída pelo [usuário](#usuário) |
| **Classificação** | Objeto |

### Configurações da conta
| | |
|-|-|
| **Nome** | Configurações da [conta](pages/ponto_de_controle_3/lexico?id=conta) |
| **Sinônimos** |  |
| **Noção** | É uma seção do [aplicativo](#aplicativo) que disponibiliza as informações básicas do [usuário](#usuário), como: e-mail, [nome de usuário](#nome-de-usuário), nome completo e idioma |
| **Impacto** | As configurações da [conta](pages/ponto_de_controle_3/lexico?id=conta) pode ser acessada pelo [usuário](#usuário) e a partir de lá algumas de suas informações podem ser mudadas. Nas configurações de [conta](pages/ponto_de_controle_3/lexico?id=conta) também é possível deletar a [conta](pages/ponto_de_controle_3/lexico?id=conta). |
| **Classificação** | Objeto |

### Quadro nutricional
| | |
|-|-|
| **Nome** | Quadro nutricional |
| **Sinônimos** | Informações nutricionais |
| **Noção** | É uma seção do [aplicativo](#aplicativo) que disponibiliza as informações nutricionais do [usuário](#usuário) baseado nos pratos que supostamente comporam sua dieta. As informações nutricionais são divididas em seções: distribuição de energia por macronutriente, ácidos graxos, vitaminas, minerais e proteínas. |
| **Impacto** | O [usuário](#usuário) pode acessar seu quadro nutricional quando desejar. O quadro nutricional é atualizado de acordo com as refeições realizadas pelo [usuário](#usuário). |
| **Classificação** | Objeto |

### Dieta
| | |
|-|-|
| **Nome** | Dieta |
| **Sinônimos** | Jejuns de certos alimentos, privação de certas refeições |
| **Noção** | É um padrão alimentar adotado pelo [usuário](#usuário) a fim de se alcançar um objetivo nutricional, como por exemplo, reduzir a quantidade de sódio ingerido. A dieta é um dos pilares do [aplicativo](#aplicativo) e influencia nas sugestões de [pratos](#receita) |
| **Impacto** | Cada [usuário](#Usuário) pode definir quais são suas metas alimentares |
| **Classificação** | Objeto |

### Compartilhar aplicativo
| | |
|-|-|
| **Nome** | Compartilhar aplicativo |
| **Sinônimos** | Compartilhar o app |
| **Noção** | O [usuário](#usuário) que gostam do [aplicativo](#aplicativo) pode compartilhar o link para download e enviá-lo para amigos utilizando outras redes sociais. |
| **Impacto** | Outra pessoa receberá o convite e poderá entrar no aplicativo através do registro de [contas](#conta). |
| **Classificação** | Verbo |

### Planejamento
| | |
|-|-|
| **Nome** | Planejamento |
| **Sinônimos** | Meal Plans |
| **Noção** | O planejamento é uma espécie de calendário do [usuário](#usuário) em forma de lista onde cada dia retém as informações de planejamento associadas a ele. |
| **Impacto** | O [usuário](#usuário) pode editar livremente o planejamento adicionando e removendo pratos. É possível também compartilhar o planejamento entre [usuários](#usuário). |
| **Classificação** | Objeto |


## Bibliografia

1. Sayão, Miriam. ; Carvalho, Gustavo R. Construção de léxico de aplicações. Proceedings of the International Joint Conference IBERAMIA/SBIA/SBRN 2006 - 4th Workshop inInformation and Human Language Technology, Outubro de 2016.