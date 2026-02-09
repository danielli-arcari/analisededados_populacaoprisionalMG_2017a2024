# Análise da População Prisional de Minas Gerais

## Como surgiu esse projeto

Eu estava procurando um tema próprio para praticar análise de dados e pensei: por que não trabalhar com algo que realmente importa? Achei dados públicos sobre a população prisional de MG disponibilizados pela Secretaria de Estado de Justiça e Segurança Pública e decidi analisar.

A ideia era entender perfis: quem está sendo preso? Qual é a escolaridade? Como isso mudou entre 2017 e 2024? Se consigo enxergar padrões, talvez isso seja útil para discussões sobre segurança pública e políticas prisionais.

## Os dados

Peguei dados abertos de janeiro de 2017 até junho de 2024 - 7 anos e meio de informações. No total eram 328.773 registros, mas após limpeza reduzi para 284.627 para eliminar inconsistências.

Os dados incluíam:
- Quem: sexo e nível de escolaridade na admissão
- Onde: qual unidade prisional, município, região de segurança
- Quando: ano e mês de entrada

## Processo de análise

### Primeiro: exploração
Carreguei os dados e comecei a entender o tamanho (é muita informação mesmo), quantos bairros, quantos estabelecimentos prisionais, como estavam distribuídos os dados.

### Depois: limpeza
Tive que:
- Remover registros claramente duplicados ou com erros
- Padronizar nomes de colunas (tinha tudo em maiúscula e com espaços)
- Validar os valores

Tirei cerca de 44 mil registros - 15% do total - porque não eram confiáveis.

### Análise de verdade
Comecei a fazer perguntas:
- Qual é a distribuição por sexo?
- Qual é o nível de escolaridade predominante?
- Mudou algo entre 2017 e 2024?
- Quais regiões têm mais população carcerária?

## O que descobri

### Disparidade gigante de gênero
A população prisional é **89% masculina**. Isso não é coincidência - dados nacionais e internacionais mostram a mesma coisa. Mas ver em números é diferente.

### Escolaridade baixa concentrada
O nível mais comum é "1º Grau Incompleto" com mais de 51 mil registros. Tem também analfabeto, semi-alfabetizado. Muito poucos com superior completo.

Isso levanta uma questão: será que a baixa escolaridade leva ao crime, ou a falta de oportunidades para quem tem baixa escolaridade coloca essas pessoas em situações vulneráveis? Provavelmente ambas as coisas.

### Concentração geográfica
A Penitenciária Prof. Aluízio Ignácio de Oliveira em Ribeirão das Neves é a maior. Tem muita concentração em torno de Belo Horizonte e região metropolitana, que faz sentido.

### 7 anos de dados
Consegui ver como as coisas mudaram (ou não) de 2017 até 2024. Tem períodos com mais admissões, períodos com menos. Dá para pensar sobre o que pode ter influenciado.

## Por que isso importa

Dados sobre população prisional costumam ser números abstratos nas notícias. Quando você senta e analisa, vê pessoas: quase 300 mil admissões em 7 anos em um único estado. Entender o perfil ajuda a ter conversas mais informadas sobre segurança pública, reabilitação, políticas prisionais.

## Desafios

O principal foi lidar com dados governamentais, que às vezes têm qualidade inconsistente. Alguns campos tinham padrões diferentes, alguns dados faltavam. Tive que ser cuidadosa para não descartar informação legítima só porque estava formatada diferente.

## Ferramentas

Python, Pandas para manipulação pesada de dados, NumPy para estatísticas, Matplotlib e Seaborn para visualizar. Trabalhar com quase 300 mil linhas exigiu atenção com performance e memória.

## O que aprendi

Análise de dados de verdade é 80% limpeza e 20% insights. Ninguém quer ver seus dados finais, mas se fizer tudo certo, os insights saem naturalmente.

## O que achei mais legal

Conseguir traduzir números em histórias que fazem sentido. Um padrão de escolaridade não é só um número - é uma janela para entender vulnerabilidades sociais.

## Links

- [Notebook no Colab](https://colab.research.google.com/drive/1ESr8ZIiVcNlW785A_7c3kQjfPLPLXbCu?usp=sharing)
- [Repositório no GitHub](https://github.com/danielli-arcari/analisededados_populacaoprisionalMG_2017a2024)
- [Meu portfólio](https://danielli-arcari.github.io/)
- [LinkedIn](https://www.linkedin.com/in/danielli-arcari/)
