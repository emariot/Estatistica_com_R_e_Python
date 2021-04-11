# Estudos de estatística utilizando R e Python 

## 1. Tabelas de Frequência
---
* Contrução de uma tabela de frequência em R
  > ![alt text](https://github.com/emariot/Estatistica_com_R_e_Python/blob/main/R/img/tabela_frequencia.PNG)

## 2. Amostragem e Medidas de Centralidade
---

### A amostra é parte de uma população, selecionada randomicamente, que forma o conjunto de elementos que esta sendo estudado. 
* População: todo o alvo de um estudo 
* Amostra: subconjunto da população
* Censo: pesquisa com toda a população

<strong>Quando feita corretamente, a amostra preserva as mesmas características da população de onde foi retirada, caso contrário ela poderá estar enviesada. Para tanto faz-se necessário precisar: </strong>

* O tipo de coleta da amostra
* O tamanho da amostra
* A randonização dos dados

#### Viés: subestima ou superestimação da população.
* Pesquisa de elementos de fácil acesso
* Pesquisas pela Internet (contando com pessoas que possuiem interesse na pesquisa)
* Sem utilização mecanismos de seleção aleatória

#### Custo/Benefício de uma Amostra: vantagem de não trabalhar com toda a população, poupando recursos e agilizando a captação dos dados.

### Amostragem Probabilística (elementos selecionados de forma aleatória, todos com a mesma probabilidade de serem escolhidos):
* Amostragem Simples ao Acaso
* Amostragem Sistemática
* Amostragem por Conglomerado
* Amostragem Estratificada
* Reamostragem (Boostrap)

### Amostragem não Probabilística (subjetiva, com interferência do pesquisados):
* Amostragem a Esmo
* Amostragem Intencional 
* Amostragem por Voluntários

### Diferênça entre Parâmetro e Estatística
* Parâmetro: característica sobre a população
  * Valores calculados usando dados da população são chamados de parâmetros
* Estatística: característica sobre a amostra
  * Valores calculados usando dados da amostra sãochamados estatísticas
  
> A estatística inferencial realiza deduções e conclusões sobre a população baseadas nos resultados obtidos na análise da amostra. A AMOSTRA é utilizada para calcular a estatística que é usada para estimar os parâmetros da POPULAÇÃO.

### Dados Primários e Dados Secundários:
* Primários:
  * Coletados por quem faz a análise
  * Confiáveis
  * Possuem maior controle
  * Maior custo
  * Maior tempo
  * Maior equipe
* Secundários (mais comuns):
  * Coletados por terceiros
  * Menos confiáveis 
  * Pouco controle
  * Menor custo
  * Rapidez
---
## 3. Distribuição Binomial e Normal
---
## 4. Distribuição T de Student
---
## 5. Distribuição de Poisson
---
## 6. Intervalo de Confiança
---
## 7. Teste Qui quadrado
---
## 8. Teste de variância - Anova
---
## 9. Regressão Linear Simples -Y ~ X
---
* Uma variável explanatória para prever uma variável dependente
* Dataset: cars.csv: medida da velocidade e distância após freagem de vários veículos.

### Modelo de regressão em Python com bilbioteca sklearn

> ![alt text](https://github.com/emariot/Estatistica_com_R_e_Python/blob/main/Python/img/Regress%C3%A3o_linear_simples.png)

### Os resíduos se aproxímam de uma distribuição normal, significa que o modelo tem uma ótima correlação 

> ![alt text](https://github.com/emariot/Estatistica_com_R_e_Python/blob/main/Python/img/Regress%C3%A3o_linear_simples_res%C3%ADduos.png)

### * Exercício: modelo de regressão linear para prever qual será o investimento inicial necessário de uma franquia a partir da Taxa Anual cobrado pelo franqueado.

#### Variáveis: 
* FraAnual: Taxa Anual
* CusInic: Investimento Inicial

#### Regressão: 
> ![alt text](https://github.com/emariot/Estatistica_com_R_e_Python/blob/main/Python/img/franquia.png)

#### Modelo:
* Variável independente: 1300
* Variável resposta: 1352 

## 10. Regressão Linear Múltipla- Y ~ X1 + X2 + Xn
---
* Duas os mais variáveis explanatórias para prever uma variável dependente
* Dataset: mtcars.csv: dados de especificações de modelos de veículos.

### Modelo de regressão múltipla em Python: Previsão de autonomia do veículo. 
Bibliotecas: Sklearn e Stats model

> ![alt text](https://github.com/emariot/Estatistica_com_R_e_Python/blob/main/Python/img/Regress%C3%A3o_linear_multipla.png)

* Predict com regressão simples: cilindradas = 200; consumo = 21
* Predict com regressão múltipla: cilindradas = 200, cilindros = 4, cavalos = 100; consumo = 24

## 11. Regressão Logistica
---
## 12. Teste de Hipótese com Análise Exploratória de Dados
---
## 13. Teoria Central do Limite
---
