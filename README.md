# Aumento de 36% no lucro no setor bancário

## Descrição

Este projeto demonstra como um modelo de Machine Learning reduziu drasticamente os custos de uma campanha de marketing bancário e aumentou o lucro em **36%**, prevenindo erros comuns como **data leakage**.  
O foco foi alinhar a métrica técnica com o objetivo real do negócio, garantindo aplicabilidade no mundo real.

## Contexto do Problema

O banco analisado possuía uma abordagem de campanha onde **todos os clientes eram contatados**, gerando altos custos com baixo retorno.  
Na amostra de 4.521 clientes, o cenário inicial foi:

- **Receita:** € 260.000,00  
- **Custo:** € 73.254,62  
- **Lucro:** € 187.254,38

## 🎯 Objetivo
Identificar, **antes da campanha**, os clientes mais propensos a aceitar uma oferta de depósito a prazo, utilizando apenas informações disponíveis **pré-campanha**, eliminando riscos de **data leakage**.


## Metodologia
- **Detecção e prevenção de data leakage**  
  - Exclusão de variáveis futuras (“dias desde o último contato”, “duração da ligação”)  
- **Preparação de dados**  
  - Seleção e Codificação das variáveis 
  - Balanceamento com Random Oversampler  
- **Modelagem**  
  - Algoritmo: Random Forest  
  - Métrica foco: recall no grupo-alvo (para reduzir custo sem perder clientes potenciais)
 

## 📊 Resultados
Cenário final:
- **Receita:** € 258.500,00  
- **Custo:** € 3.191,64  
- **Lucro:** € 255.308,36 (**+36%** vs. cenário inicial)  
- **Impacto:** redução significativa de falsos positivos sem perda relevante de clientes potenciais


## 💡 Principais Lições
- A melhor métrica é aquela que melhor traduz o objetivo real do negócio
- Data leakage compromete não só o modelo, mas também os resultados financeiros
- **Viabilidade prática** deve ser pensada desde a seleção de variáveis  

## Links Úteis:

- 📄 Artigo no LinkedIn: [Link](https://www.linkedin.com/pulse/da-modelagem-%C3%A0-entrega-real-uma-jornada-pr%C3%A1tica-para-garantir-f%C3%A9lix-7njxf/) 

✍️ Sequência de artigos no Medium documentando o processo de aprendizado durante o desenvolvimento deste projeto:
- [Artigo 1 - Foco no Entendimento de Negócio](https://medium.com/@fagna.felix/do-modelo-%C3%A0-estrat%C3%A9gia-como-medir-o-impacto-financeiro-de-uma-solu%C3%A7%C3%A3o-de-machine-learning-no-ba80e5231085) 
- [Artigo 2 - Foco na Modelagem](https://medium.com/@fagna.felix/do-modelo-%C3%A0-estrat%C3%A9gia-um-caso-de-sucesso-na-gera%C3%A7%C3%A3o-de-receita-com-machine-learning-parte-ii-237606db091f) 
- [Artigo 3 – Corrigindo Data Leakage](https://medium.com/@fagna.felix/do-modelo-%C3%A0-estrat%C3%A9gia-corrigindo-o-data-leakage-e-tornando-a-solu%C3%A7%C3%A3o-pronta-para-o-mundo-real-840390c49fa1)

