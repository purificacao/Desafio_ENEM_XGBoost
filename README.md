# Desafio para participar do Aceleradev Data Science da Codenation em abril de 2020

Neste notebook, vamos prever as notas de matemática dos estudantes que fizeram a prova do ENEM de 2016, em função de alguns atributos dados.

__Objetivo do desafio:__ Gerar um modelo a partir dos dados de treino e fazer a predição das notas de matemática (`NU_NOTA_MT`) no dado de teste, de modo que não temos a variável `NU_NOTA_MT` no dado de teste, para podermos inferir se nosso modelo ficou realmente bom em dados "não vistos". Após, enviar o resultado para a Codenation em um arquivo answer.csv com duas colunas: `NU_INSCRICAO` e `NU_NOTA_MT` (nota de matemática predita)! Eles detêm a da nota verdadeira e fazem a avaliaçao da nossa nota predita com a nota verdadeira, atribuindo-nos uma nota percental, que creio eu, varie de 0 à 100.

Neste desafio mostrarei manobras para a EDA (Exploratory Data Analysis), além da transformação das variáveis categóricas em numéricas (que dependerá de serem nominais ou ordinais) e quantitativas discretas. Após, serão aplicados dois algoritmos poderosíssimos:

- *Random Forest*
- *Extreme Gradient Boosting (XGboost)*
 - Esse algoritmo me proporcionou um score de 94% (dado pela Codenation), me colocando dentro do Aceleradev Data Science

## Requisitos

Você precisará de python 3.6 (ou superior) e do gerenciador de pacotes pip.

Para instalar os requisitos, execute o comando como no exemplo abaixo:

    
```bash
$ pip install -r requirements.txt
```

## Detalhes

O contexto do desafio gira em torno dos resultados do ENEM 2016 (disponíveis no arquivo train.csv). Qualquer dúvida a respeito das colunas, consulte o arquivo __Dicionario_Microdados_Enem_2016.xlsx__, no folder __datasets__.