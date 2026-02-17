Análise da População Prisional de Minas Gerais (2017–2024)
Sobre o projeto

Este projeto apresenta uma análise exploratória da população prisional admitida no estado de Minas Gerais entre 2017 e 2024.

A análise foi realizada a partir de dados públicos disponibilizados pela Secretaria de Justiça e Segurança Pública de Minas Gerais:

https://www.seguranca.mg.gov.br/index.php/component/sppagebuilder/page/266

O objetivo principal foi aplicar técnicas de limpeza, organização e análise de dados em grande volume, buscando identificar padrões demográficos e educacionais nas admissões ao sistema prisional.

Objetivos

Responder às seguintes perguntas:

Como evoluiu o volume de admissões ao longo dos anos?

Qual a distribuição percentual por sexo?

Qual o nível de escolaridade predominante na admissão?

Há concentração relevante em determinadas instituições ou unidades prisionais?

Tratamento e preparação dos dados

A base original continha 328.773 registros.

As seguintes etapas foram realizadas:

Remoção de 44.146 registros duplicados

Padronização dos nomes das colunas

Criação de variável temporal consolidando ano e mês

Exclusão de 2024 da análise de crescimento por se tratar de ano com dados parciais

Utilização da variável contagem_ipl como métrica principal para agregações, garantindo consistência analítica

Após o tratamento, a base final passou a conter 284.627 registros válidos.

Evolução temporal das admissões

A análise de crescimento anual considerou apenas anos completos, de 2017 a 2023.

Observou-se:

Crescimento relevante entre 2017 e 2018

Oscilações negativas e positivas nos anos seguintes

Redução significativa em 2020

Estabilização relativa entre 2021 e 2023

O ano de 2024 foi excluído da análise de crescimento por conter apenas dados até junho, o que comprometeria a comparabilidade.

Distribuição por sexo

A análise baseada na soma de admissões indica forte predominância masculina:

Masculino: 95,78%

Feminino: 4,22%

Essa proporção mantém-se estável ao longo do período analisado, caracterizando padrão estrutural do sistema prisional estadual.

Escolaridade na admissão

A categoria mais frequente foi Fundamental Incompleto, representando 67,62% do total de admissões no período.

Os dados evidenciam concentração expressiva em níveis mais baixos de escolarização formal. A análise é descritiva e não permite estabelecer relação causal, mas aponta padrão consistente ao longo dos anos.

Instituições e concentração

A maior parte das admissões ocorre em unidades administradas pelo DEPEN.

O ranking de estabelecimentos evidencia concentração relevante em determinadas unidades prisionais, indicando centralização operacional.

Tecnologias utilizadas

Python 3

Pandas

NumPy

Matplotlib

Seaborn

Google Colab

Limitações

Ausência de variáveis socioeconômicas detalhadas

Não há dados sobre reincidência ou tempo de permanência

A análise é exclusivamente exploratória

Não foram aplicados modelos estatísticos inferenciais

Considerações finais

O projeto demonstra aplicação prática de técnicas de limpeza, organização e análise exploratória de dados públicos em grande volume.

Os resultados indicam estabilidade estrutural no perfil das admissões, com predominância masculina, forte concentração em níveis educacionais mais baixos e centralização em determinadas unidades prisionais.

A análise foi conduzida com foco em consistência metodológica e interpretação responsável dos dados.

## Links

- [Notebook no Colab](https://colab.research.google.com/drive/1ESr8ZIiVcNlW785A_7c3kQjfPLPLXbCu?usp=sharing)
- [Repositório no GitHub](https://github.com/danielli-arcari/analisededados_populacaoprisionalMG_2017a2024)
- [Meu portfólio](https://danielli-arcari.github.io/)
- [LinkedIn](https://www.linkedin.com/in/danielli-arcari/)
