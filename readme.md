<!-- antes de enviar a versão final, solicitamos que todos os comentários, colocados para orientação ao aluno, sejam removidos do arquivo -->
# <Nome do projeto>

#### Aluno: [Jose Leonel Majewski](https://github.com/leonelmajewski)
#### Orientadora: [Manoela Kohler](https://github.com/manoelakohler).

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

<!-- para os links a seguir, caso os arquivos estejam no mesmo repositório que este README, não há necessidade de incluir o link completo: basta incluir o nome do arquivo, com extensão, que o GitHub completa o link corretamente -->
- [Link para o código](https://github.com/link_do_repositorio). <!-- caso não aplicável, remover esta linha -->

- [Link para a monografia](https://link_da_monografia.com). <!-- caso não aplicável, remover esta linha -->

- Trabalhos relacionados: <!-- caso não aplicável, remover estas linhas -->
    - [Nome do Trabalho 1](https://link_do_trabalho.com).
    - [Nome do Trabalho 2](https://link_do_trabalho.com).

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

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin pulvinar nisl vestibulum tortor fringilla, eget imperdiet neque condimentum. Proin vitae augue in nulla vehicula porttitor sit amet quis sapien. Nam rutrum mollis ligula, et semper justo maximus accumsan. Integer scelerisque egestas arcu, ac laoreet odio aliquet at. Sed sed bibendum dolor. Vestibulum commodo sodales erat, ut placerat nulla vulputate eu. In hac habitasse platea dictumst. Cras interdum bibendum sapien a vehicula.

Proin feugiat nulla sem. Phasellus consequat tellus a ex aliquet, quis convallis turpis blandit. Quisque auctor condimentum justo vitae pulvinar. Donec in dictum purus. Vivamus vitae aliquam ligula, at suscipit ipsum. Quisque in dolor auctor tortor facilisis maximus. Donec dapibus leo sed tincidunt aliquam.

### 4. Conclusões

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin pulvinar nisl vestibulum tortor fringilla, eget imperdiet neque condimentum. Proin vitae augue in nulla vehicula porttitor sit amet quis sapien. Nam rutrum mollis ligula, et semper justo maximus accumsan. Integer scelerisque egestas arcu, ac laoreet odio aliquet at. Sed sed bibendum dolor. Vestibulum commodo sodales erat, ut placerat nulla vulputate eu. In hac habitasse platea dictumst. Cras interdum bibendum sapien a vehicula.

Proin feugiat nulla sem. Phasellus consequat tellus a ex aliquet, quis convallis turpis blandit. Quisque auctor condimentum justo vitae pulvinar. Donec in dictum purus. Vivamus vitae aliquam ligula, at suscipit ipsum. Quisque in dolor auctor tortor facilisis maximus. Donec dapibus leo sed tincidunt aliquam.


---

Matrícula: 211.100.146

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
