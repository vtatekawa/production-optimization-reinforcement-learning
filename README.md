
# 📊 Planejamento de Produção com Aprendizado por Reforço

Bem-vindo ao projeto **Planejamento de Produção com Aprendizado por Reforço**! Este repositório contém um notebook em Python que implementa o aprendizado por reforço para resolver o problema de sequenciamento de produção em uma fábrica. O objetivo é otimizar a produção para atender às demandas, minimizando custos relacionados ao estoque e ao não atendimento. 🚀

## 📚 Índice

- [Visão Geral](#visão-geral)
- [Descrição do Problema](#descrição-do-problema)
- [Estrutura dos Dados de Entrada](#estrutura-dos-dados-de-entrada)
- [Como Funciona o Aprendizado por Reforço](#como-funciona-o-aprendizado-por-reforço)
- [Dependências](#dependências)
- [Uso](#uso)
- [Saída](#saída)

## 📋 Visão Geral

Este notebook utiliza o aprendizado por reforço para otimizar o sequenciamento de produção em quatro linhas de produção, com o objetivo de atender à demanda de 20 produtos, minimizando os custos de estoque e a penalidade por não atendimento.

## 🧠 Como Funciona o Aprendizado por Reforço

O aprendizado por reforço (RL) é uma técnica onde um agente aprende a tomar decisões em um ambiente para maximizar uma recompensa cumulativa. A seguir estão os principais conceitos aplicados:

1. **Estado:** Representa a situação atual do estoque e da produção de cada produto.
2. **Ação:** Decisão sobre qual linha de produção utilizar para cada produto.
3. **Recompensa:** Calculada com base em como a ação atende à demanda e minimiza o excesso de estoque.

O agente aprende uma política ótima através da interação repetida com o ambiente, ajustando suas ações para maximizar a recompensa acumulada.

## 🗂 Estrutura dos Dados de Entrada

1. **Demandas:** Dados sobre as demandas mensais de cada produto.
2. **Estoque Inicial:** Estoque inicial disponível para cada produto.
3. **Produtividade:** Produtividade de cada linha de produção.
4. **Capacidades:** Capacidades máximas das linhas de produção.

Os dados são carregados de um arquivo Excel com planilhas separadas para cada conjunto de informações.

## 🛠 Dependências

Certifique-se de ter as seguintes dependências instaladas:

- Python 3.x
- Pandas
- NumPy

Instale-as usando pip:

```bash
pip install requirements.txt
```

## 🚀 Uso

1. Clone este repositório e execute o notebook:

   ```bash
   git clone <https://github.com/vtatekawa/production-optimization-reinforcement-learning>
   cd <production-optimization-reinforcement-learning>
   jupyter notebook productionPlanningRL.ipynb
   ```

2. Carregue seus dados de produção nos formatos adequados (exemplos estão na pasta `input`).
3. Execute todas as células do notebook para otimizar o plano de produção.

## 📈 Saída

Após executar o notebook, você obterá:

- **Plano de Produção Otimizado:** Sequência de produção para atender às demandas em um arquivo excel na pasta output.

---

Feito com 🧠 por [Vitor Tatekawa](https://github.com/vtatekawa)
