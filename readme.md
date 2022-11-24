<!-- antes de enviar a versão final, solicitamos que todos os comentários, colocados para orientação ao aluno, sejam removidos do arquivo -->
# <Nome do projeto>

#### Aluno: [Jose Leonel Majewski](https://github.com/leonelmajewski)
#### Orientadora: [Manoela Kohler](https://github.com/manoelakohler).

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

---

### Resumo

<!-- trocar o texto abaixo pelo resumo do trabalho, em português -->

A análise da satisfação do usuário com os atendimentos realizados pelas equipes da TIC, obtida por meio de pesquisas de satisfações encaminhadas ao final de cada chamado aberto por este, é um importante recurso para mensurar a precepção sobre a prestação dos serviços de Tecnologia da Informação e Telecomunicações, bem como insumo para decisões em níveis estratégico e tático, além da identificação de melhorias nos processos de Atendimento e correlatos.

O presente trabalho utiliza dados de atendimentos de TIC realizados na empresa Petroleo Brasileiro S.A. - Petrobras, no período de janeiro/2021 a setembro/2022, e tem por objetivo identificar tendências e, em especial, analisar o reflexo do tempo de atendimento dos chamados na satisfação demonstrada pelo usuário.

### Abstract <!-- Opcional! Caso não aplicável, remover esta seção -->

<!-- trocar o texto abaixo pelo resumo do trabalho, em inglês -->

Analysis of user satisfaction with the technical service provided by IT teams, collected through satisfaction surveys, is an important resource to measure the perception about Information Technology and Telecommunications services, as well as input for strategic and tatical, in addition to identifying improvements in service and related processes.

The present study examines data from IT services performed at Petroleo Brasileiro S.A. - Petrobras, from January/2021 to September/2022, and aims to identify trends and, in particular, analyze the impact of service time in the satisfaction demonstrated by the user.

### 1. Introdução

Os dados coletados estão divididos em dois tipos de arquivos e foram gerados por mês, abrangendo o período de janeiro/2021 a setembro/2022.

Devido as normas de Segurança da Informação da Petrobras, a utilização dos dados só é permitida após tratamento que eliminem qualquer possibilidade de rastrear as informações apresentadas.
  
Por esse motivo, foi realizado um tratamento inicial nos arquivos-fonte, eliminando dados que permitam rastrear a origem dos registros, além da eliminação de colunas que não serão utilizados no processo de análise de dados.

### 2. Modelagem

A extração da base de dados foi realizada em formato .xlsx e apresem os campos listados abaixo:

Arquivos chamados encerrados:

![Arquivos de chamados encerrados](https://github.com/leonelmajewski/BIMaster_Trabalho_Final/blob/main/Tabela_1.png)

Arquivo de pesquisas respondidas:

![Arquivo de pesquisas respondidas](https://github.com/leonelmajewski/BIMaster_Trabalho_Final/blob/main/Tabela_2.png)

_Observação 1:_ O campo ID do Registro será utilizado como chave primária no tratamento inicial dos dados (join das tabelas) e será excluído após essa etapa, seguindo a premissa anonimização dos dados e não rastreabilidade.

_Observação 2:_ A pesquisa de satisfação é formada por três itens, sendo duas questões e um campo aberto para Comentário.

Para fins de indicadores de processo, é contabilizado apenas os resultados da questão 1 e o indicador é calculado com base na fórmula:

_Satisfação_ = (Quantidade de pesquisas com notas 4 e 5)/(Quantidade total de pesquisas respondidas)

As questões são:

_1 – Como você avalia a sua experiência com esse serviço? (Escala de 5 = Muito Satisfeito a 1 = Muito Insatisfeito)_

5	4	3	2	1

_2 – O que motivou sua opinião? (1=Prazo de resposta; 2=Atendimento (Cordialidade/ Empatia); 3=Solução; 4=Facilidade de acesso ao serviço; 5=Outros)_

5	4	3	2	1


### 3. Resultados

A análise do impacto do tempo de atendimento na satisfação do usuário demonstra que, quando considerados os registros de Incidentes e Satisfação dos usuários, evidencia o comprometimento do indicador quando o atendimento tem prazo superior a 20 minutos.

Entretanto, ao segregar a satisfação entre pesquisas que avaliam atendimento de Incidentes e pesquisas que avaliam Solicitações de Serviço, é evidenciad uma percepeção distinta, pelos usuários, quanto ao tempo de atendimento.

No caso dos Incidentes, que evidenciam uma falha ou interrupção de serviço ou recurso, a urgência no tratamento é maior uma vez que pode impactar diretamente as atividades do usuário.

No caso das Solicitações – pedido de recurso ou serviço adicional - o impacto é menor principalmente porque:

  - Não costuma impactar as atividades rotineiras dos usuários, salvo se este espera uso imediato do novo recurso ou serviço;
  
  - Solicitações de Serviço podem ter prazos distintos para atendimento, a depender da complexidade e dos recursos envolvidos. A título de exemplo, o fornecimento de uma *webcam* que tenha estoque é menor do que o fornecimento de um *software* específico, que depende do processo de aquisição de licença e que, caso envolva processo de licitação, pode levar meses para ser disponibilizado ao usuário.
  
Vale reforçar que para as Solicitações de Serviço estão mapeados tempos específicos para cada situação, refletido na variável **SLA (Tempo disponível)**.

### 4. Conclusões

A análise evidenciou que o tempo de atendimento é um fator determinante para a satisfação do usuário, quando atendido pela TIC.

Ficou evidente a importância de medir também a Satisfação dos atendimentos, de maneira segregada, para Incidentes e Solicitações de Serviço, de maneira distinta, de forma a obter informações adicionais sobre a percepção dos usuários quanto ao atendimento de suas necessidades de TIC.

Convém salientar que atendimentos em prazos muito curtos, embora aumentem a chance de satisfação, não devem ser priorizados caso o custo envolvido no atendimento seja alto. Vale ressaltar que o fator custo não foi considerado na análise em questão e pode ser tratado na evolução da análise ou em um processo distinto.
  
---

Matrícula: 211.100.146

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
