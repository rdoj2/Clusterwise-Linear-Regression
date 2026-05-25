# Repositório da Dissertação

Este repositório contém todos os códigos-fonte e conjuntos de dados utilizados nos experimentos desenvolvidos na dissertação, incluindo os algoritmos de regressão linear *clusterwise* para dados intervalares, variantes com ponderação adaptativa e os experimentos realizados com dados sintéticos e dados reais.

---

# Estrutura do Repositório

O repositório está organizado em duas partes principais:

- `Dados Sintéticos`
- `Dados Reais`

Cada pasta contém os códigos utilizados nos respectivos experimentos descritos na dissertação.

---

# Pasta: Dados Sintéticos

A pasta `Dados Sintéticos` contém os scripts utilizados nos experimentos com bases sintéticas.

Cada script corresponde a um algoritmo específico utilizado nos estudos experimentais.

## Estrutura dos scripts

### 1. `Base exp 1 + Sintetico_CLRi`

Este script contém:

- A geração das bases sintéticas utilizadas no Experimento 1;
- A implementação do algoritmo CLRi;
- O procedimento de ajuste do modelo;
- A seleção de hiperparâmetros;
- A avaliação experimental via simulação Monte Carlo.

O usuário pode executar diretamente o script para reproduzir os experimentos correspondentes ao CLRi.

---

### 2. `Base exp 2 + Sintetico_GL1`

Este script contém:

- A geração das bases sintéticas utilizadas no Experimento 2;
- A implementação do algoritmo GL1;
- O procedimento de ajuste do modelo;
- A seleção de hiperparâmetros;
- A avaliação experimental via simulação Monte Carlo.

O usuário pode executar diretamente o script para reproduzir os experimentos correspondentes ao GL1.

---

### 3. Demais scripts

Os demais arquivos da pasta correspondem às outras variantes dos algoritmos estudados na dissertação.

Esses scripts já contêm:

- Implementação completa do algoritmo;
- Ajuste do modelo;
- Seleção de hiperparâmetros;
- Avaliação experimental.

Nesses casos, o usuário deve apenas carregar a base de dados desejada no formato utilizado pelos scripts principais. O formato das bases é padronizado, de modo que basta substituir ou inserir os dados correspondentes e executar o código.

---

# Pasta: Dados Reais

A pasta `Dados Reais` está dividida em:

- `Bases Reais`
- `Códigos`

## Bases Reais

A pasta `Bases Reais` contém os conjuntos de dados reais utilizados nos experimentos da dissertação.

---

## Códigos

A pasta `Códigos` contém os scripts correspondentes aos algoritmos utilizados nos experimentos com dados reais.

Cada script realiza:

- Ajuste do modelo;
- Seleção de hiperparâmetros via validação cruzada Leave-One-Out;
- Avaliação do modelo via Duplo Leave-One-Out;
- Cálculo das métricas utilizadas na dissertação.

Os scripts seguem um padrão comum de entrada de dados. Assim, para utilizar uma nova base, o usuário precisa apenas:

1. Carregar a base de dados;
2. Definir o número de variáveis explicativas utilizadas no modelo;
3. Executar o script correspondente.

---

# Algoritmos Implementados

O repositório contém implementações dos seguintes algoritmos:

- RLCi
- RLCiP-DE
- RLCiP-DEP-LC1
- RLCiP-DEP-LC2
- RLCiP-DEP-LC3
- RLCiP-DEP-GL1
- RLCiP-DEP-GL2
- RLCiP-DEP-GL3

---

# Reprodução dos Experimentos

Para reproduzir os experimentos apresentados na dissertação:

1. Abra o script correspondente ao algoritmo desejado;
2. Carregue a base de dados apropriada;
3. Defina os parâmetros necessários;
4. Execute o script completo.

Todos os códigos foram desenvolvidos em Python.

---

# Observações

- Alguns scripts já possuem geração automática das bases sintéticas;
- Outros scripts requerem apenas o carregamento manual da base de dados;
- O formato das bases segue um padrão compatível entre os algoritmos;
- Os experimentos utilizam procedimentos de validação cruzada descritos na dissertação;
- Para informações detalhadas sobre a formulação matemática, critérios de otimização, métricas e descrição completa dos experimentos, recomenda-se consultar a dissertação associada a este repositório.
  
