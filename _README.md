# Trabalho final do curso BI Master, da turma 2021.1

Os dados coletados estão divididos em dois tipos de arquivos e foram gerados por mês, abrangendo o período de janeiro/2021 a setembro/2022.

Devido as normas de Segurança da Informação da Petrobras, a utilização dos dados só é permitida após tratamento que eliminem qualquer possibilidade de rastrear as informações apresentadas.

Por esse motivo, foi realizado um tratamento inicial nos arquivos-fonte, eliminando dados que permitam rastrear a origem dos registros, além da eliminação de colunas que não serão utilizados no processo de análise de dados.

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
