# Estudos de estatística utilizando R e Python 

## 1. Tabelas de Frequência
---
* Contrução de uma tabela de frequência em R
  > ![alt text](https://github.com/emariot/Estatistica_com_R_e_Python/blob/main/R/img/tabela_frequencia.PNG)

## 2. Amostragem, Medidas de Centralidade e Variabilidade
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
  
### Medidas de Centralidade e Variabilidade
* µ = média da população = Σx/N -> trata-se de um parâmetro populacional
* X = média da amostra = Σx/n -> trata-se de uma estatística amostral
* Moda = Valor mais frequente/comum
* Mediana: Valor que separa a metade maior da metade menor de uma amostra ou população
* Amplitude: Diferença entre o maior e o menor valor na amostra ou população.
* σ^2 = Variância Populacional = Σ(xi-X)^2/N -> média dos quadrados das diferenças entre cada elemento e a média da população. Indica a dispersão dos dados em relação à média.
* S^2 = Variância Amostral = Σ(xi-X)^2/(n-1) -> Estimativa não viciada: média dos quadrados das diferenças entre cada elemento e a média da da amóstra menos 1. O resultado é um número maior que o da Variância Populacional.
* σ = Desvio Padrão
* FIQ = Intervalo Interquartil = 3Q - 1Q

#### Medidas de posição relativa: quartis:

* Q1: 25% dos menores valores
* Q2: 50% dos valores (mediana)
* Q3: 75% dos maiores valores

#### Coeficiente de Variação (CV):
  * Um CV alto indica alta variabilidade dos dados, ou seja, menos consistência nos dados,
  * Um CV baixo indica mais consistência nos dados dentro do conjunto de dados.
  > CV = (Desvio Padrão/Média)*100
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
## 14. Séries Temporais
> Encontrar tendências, fazer prtevisões e manter controle
* Estuda o comportamento de uma variável contínua ao longo do tempo
    * Uma mesma variável analisada no decorrer do tempo
    * Relação no intervalo de tempo
    * O intervalo de tempo deve ser regular
    * Dependência da ordem
    * Não é possível analisar mais de uma amostra em um intervalo
* Estacionárias:
    * Flutuam em torno de uma mesma média e variância
* Não estacionárias:
    * Exibem trends, ciclos, padrões sazonais e outros comportamentos.
* Estocásticas:
    * Composta por um fator aleatório ue não pode ser explicado matematicamente.
* Determinísticas:
    * Explicaveis por meio de uma função.

## Componentes de uma Série Temporal: 
* Tendência
* Sazonalidade
* Aleatoridade
> ![alt text](https://github.com/emariot/Estatistica_com_R_e_Python/blob/main/R/img/elem.png)
## Previsão (Data: AirPassengers)
> ![alt text](https://github.com/emariot/Estatistica_com_R_e_Python/blob/main/R/img/series_temporais.png)
