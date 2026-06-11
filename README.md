# Análise Estatística de Dados com NumPy para Marketing

Mini-projeto desenvolvido ao longo do curso **Fundamentos de Linguagem Python — Do Básico a Aplicações de IA**, da [Data Science Academy (DSA)](https://www.datascienceacademy.com.br), no **módulo sobre NumPy** (Capítulo 8 — Mini-Projeto 3).

## Contexto

Uma plataforma de e-commerce coleta dados sobre o comportamento dos usuários: número de visitas, tempo de sessão, itens adicionados ao carrinho e valor final de compra. O objetivo é transformar esses dados brutos em insights acionáveis para as equipes de marketing e produto, aumentando o ticket médio e a taxa de conversão da plataforma.

## O que o projeto cobre

| Seção | Descrição |
|---|---|
| Geração de dados | Criação de dataset sintético com 500 usuários usando `np.random` |
| Análise Descritiva | Média, mediana, desvio padrão, mínimo e máximo por variável |
| Segmentação de Clientes | Filtros booleanos para isolar clientes de alto valor e visitantes sem compra |
| Análise de Correlação | Matriz de correlação com `np.corrcoef` e heatmap com Seaborn |
| Relatório Final | Conclusões e recomendações de negócio baseadas nos dados |

## Perguntas de negócio respondidas

1. Qual é o perfil médio do usuário (visitas, tempo, ticket médio)?
2. Quais são os comportamentos distintos dos clientes de alto valor?
3. O que caracteriza os visitantes que não convertem em compradores?
4. Existe correlação entre tempo no site, itens no carrinho e valor da compra?

## Principais resultados

- Ticket médio: **R$ 252,70** | Mediana: **R$ 248,13** | Desvio padrão: **R$ 106,94**
- Clientes de alto valor (gasto > R$ 250): **245 usuários** — visitam mais (33 vezes/mês) e ficam mais tempo (37 min)
- Correlação Itens ↔ Valor da Compra: **1,00** (perfeita)
- Correlação Tempo no Site ↔ Valor da Compra: **0,59** (moderada)

## Tecnologias

- **NumPy 2.3.2** — geração de dados, operações vetorizadas e cálculos estatísticos
- **Pandas 2.3.1** — estruturação da matriz de correlação para visualização
- **Matplotlib 3.10.0** — histogramas e linhas de referência
- **Seaborn 0.13.2** — heatmap da matriz de correlação

## Arquivos

```
.
├── app.ipynb                          # Solução desenvolvida durante o curso
└── base/
    ├── DSA-Python-Cap08.ipynb         # Material base do Capítulo 8
    ├── DSA-Python-Lista3-Exercicios.ipynb
    └── DSA-Python-MiniProjeto3.ipynb  # Enunciado original do mini-projeto
```

## Como executar

```bash
# Crie e ative o ambiente virtual
python -m venv venv
venv\Scripts\activate      # Windows

# Instale as dependências
pip install numpy pandas seaborn matplotlib

# Abra o notebook principal
jupyter notebook app.ipynb
```

---

Projeto desenvolvido por **Gabriel Alves** como parte da trilha de estudos na Data Science Academy.
