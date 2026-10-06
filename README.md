# Otimizador de Distribuição de Doações

Ferramenta computacional que aplica **Otimização Linear e Inteira** para alocar doações a instituições beneficiárias em **cenários de escassez**. O sistema decide automaticamente **quais produtos e quantidades** enviar a cada instituição, considerando prioridades e custos de entrega.

Desenvolvido como parte de projeto de **Iniciação Científica (2025–2026)** na USP.

## 🎯 Problema

Em cenários de escassez, decidir como distribuir doações entre instituições é um problema **complexo**: existem prioridades diferentes, custos de entrega variáveis, e demanda que **não pode ser totalmente atendida**. Uma distribuição manual tende a ser **ineficiente ou injusta**.

Este projeto modela o problema como um **problema de otimização linear/inteira** e resolve automaticamente.

## 🚀 Tecnologias

- Python 3
- Otimização Linear e Inteira ([PuLP / SciPy / Gurobi — ajuste])
- NumPy
- Pandas

## 🎯 O que faz

- Modela matematicamente a alocação de produtos a instituições
- Considera **prioridades** e **custos de entrega** como restrições
- Maximiza o atendimento das demandas dentro das restrições
- Retorna a planilha de alocações 

## 🧠 Contexto matemático

O problema é modelado como:

- **Variáveis de decisão:** quantidade de cada produto enviada a cada instituição
- **Função objetivo:** maximizar atendimento ponderado por prioridade
- **Restrições:** estoque disponível, orçamento de entrega, demandas mínimas


## 📦 Como rodar

```bash
# Clone o repositório
git clone https://github.com/Dani-ela-git/donation-optimizer.git
cd donation-optimizer

# Crie um ambiente virtual
python -m venv venv
source venv/bin/activate  # Linux/Mac
# ou: venv\Scripts\activate  # Windows

# Instale as dependências
pip install -r requirements.txt

# Rode o script principal
python main.py
