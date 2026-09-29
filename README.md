# 📊 Simulador de Investimentos em Excel

Projeto desenvolvido durante o Bootcamp da **DIO (Digital Innovation One)** com o objetivo de criar uma ferramenta de simulação de investimentos utilizando **Microsoft Excel**, aplicando conceitos de planejamento financeiro, rendimento mensal, projeção de patrimônio e estimativa de dividendos.

O projeto também tem como objetivo demonstrar a utilização do **GitHub para documentação e compartilhamento de projetos**.

> ⚠️ **Aviso:** este projeto possui finalidade exclusivamente educacional. Os valores apresentados são resultados de uma simulação e não representam recomendação de investimento.

---

## 🎯 Objetivos do Projeto

O projeto foi desenvolvido para aplicar, na prática, os seguintes conhecimentos:

* Criar uma ferramenta de simulação de investimentos no Excel;
* Calcular o valor destinado mensalmente aos investimentos;
* Projetar o crescimento do patrimônio ao longo do tempo;
* Calcular uma estimativa de dividendos mensais;
* Trabalhar com diferentes cenários de investimento;
* Organizar dados utilizando fórmulas do Excel;
* Utilizar tabelas auxiliares para distribuição de investimentos;
* Documentar um projeto técnico utilizando Markdown;
* Utilizar o GitHub para versionamento e compartilhamento.

---

## 🛠️ Tecnologias e Ferramentas

* **Microsoft Excel**
* **Git**
* **GitHub**
* **Markdown**

### Principais recursos do Excel utilizados

* `FV`
* `VLOOKUP`
* `SUM`
* Fórmulas matemáticas e financeiras
* Referências absolutas e relativas
* Tabelas auxiliares
* Formatação de dados

---

## 📁 Estrutura do Projeto

```text
simulador-investimentos-dio/
│
├── README.md
├── PROJETO.xlsx
│
└── images/
    ├── simulador-investimentos.png
    └── distribuicao-fiis.png
```

### Arquivos

| Arquivo        | Descrição                                      |
| -------------- | ---------------------------------------------- |
| `README.md`    | Documentação do projeto                        |
| `PROJETO.xlsx` | Planilha contendo o simulador de investimentos |
| `images/`      | Imagens utilizadas para documentar o projeto   |

---

# 📈 Funcionamento da Simulação

A planilha foi estruturada para permitir a definição de algumas informações básicas do investidor e, a partir desses dados, realizar uma projeção de patrimônio.

## ⚙️ Configurações utilizadas

Na simulação desenvolvida foram utilizados os seguintes valores:

| Informação                                       |       Valor |
| ------------------------------------------------ | ----------: |
| Salário                                          | R$ 4.200,00 |
| Percentual destinado ao investimento             |         30% |
| Investimento mensal                              | R$ 1.260,00 |
| Período principal da simulação                   |     10 anos |
| Taxa de rendimento mensal                        |      1,079% |
| Rendimento da carteira utilizado para dividendos |        0,6% |

O percentual de investimento é calculado sobre o salário:

```text
R$ 4.200,00 × 30% = R$ 1.260,00
```

Dessa forma, o valor utilizado como aporte mensal na simulação é de:

**R$ 1.260,00**

---

# 💰 Projeção de Patrimônio

Para calcular o patrimônio acumulado, a planilha utiliza a função financeira `FV` do Excel.

A fórmula utilizada é:

```excel
=FV(taxa_mensal;qtd_anos*12;aporte*-1)
```

A função considera:

* taxa de rendimento mensal;
* quantidade de meses;
* aporte mensal;
* capitalização dos valores ao longo do tempo.

Na simulação principal, considerando:

* aporte mensal de R$ 1.260,00;
* período de 10 anos;
* rendimento mensal de 1,079%;

o patrimônio projetado pela planilha é de aproximadamente:

### 💰 R$ 306.538,11

---

# 📊 Cenários de Investimento

A planilha também apresenta diferentes horizontes de tempo para visualizar o crescimento do patrimônio.

| Período | Patrimônio projetado | Dividendos estimados/mês |
| ------: | -------------------: | -----------------------: |
|  2 anos |         R$ 34.306,81 |                R$ 205,84 |
|  5 anos |        R$ 105.558,91 |                R$ 633,35 |
| 10 anos |        R$ 306.538,11 |              R$ 1.839,23 |
| 20 anos |      R$ 1.417.749,98 |              R$ 8.506,50 |
| 30 anos |      R$ 5.445.933,77 |             R$ 32.675,60 |

Esses valores são **projeções matemáticas da planilha**, considerando as premissas utilizadas no modelo.

Resultados reais podem ser diferentes devido a fatores como variação de rentabilidade, inflação, taxas, impostos, oscilações de mercado e alterações nos aportes.

---

# 💵 Estimativa de Dividendos

A planilha também realiza uma estimativa de dividendos mensais.

A fórmula utilizada relaciona o patrimônio acumulado com o rendimento da carteira:

```excel
=Patrimônio_Acumulado × Rendimento_Carteira
```

Na simulação de 10 anos:

```text
R$ 306.538,11 × 0,6%
```

Resultado aproximado:

**R$ 1.839,23 por mês**

Novamente, trata-se de uma **estimativa matemática**, e não de uma garantia de rendimento.

---

# 🏢 Distribuição dos FIIs

A planilha possui uma segunda aba chamada:

```text
APOIO
```

Essa aba contém uma tabela auxiliar para organizar a distribuição dos investimentos de acordo com diferentes perfis.

Foram utilizados três perfis:

* Conservador
* Moderado
* Agressivo

E seis categorias de FIIs:

* Papel
* Tijolo
* Híbrido
* FOFs
* Desenvolvimento
* Hotelarias

---

## 🟢 Perfil Conservador

| Tipo de FII     | Percentual |
| --------------- | ---------: |
| Papel           |        30% |
| Tijolo          |        50% |
| Híbrido         |        10% |
| FOFs            |        10% |
| Desenvolvimento |         0% |
| Hotelarias      |         0% |
| **Total**       |   **100%** |

---

## 🟡 Perfil Moderado

| Tipo de FII     | Percentual |
| --------------- | ---------: |
| Papel           |        22% |
| Tijolo          |        40% |
| Híbrido         |         8% |
| FOFs            |        10% |
| Desenvolvimento |        10% |
| Hotelarias      |        10% |
| **Total**       |   **100%** |

---

## 🔴 Perfil Agressivo

| Tipo de FII     | Percentual |
| --------------- | ---------: |
| Papel           |        50% |
| Tijolo          |        10% |
| Híbrido         |         5% |
| FOFs            |         5% |
| Desenvolvimento |        20% |
| Hotelarias      |        10% |
| **Total**       |   **100%** |

Essas distribuições fazem parte da **simulação educacional desenvolvida no projeto**.

---

# 🧮 Fórmulas utilizadas

Algumas das principais fórmulas utilizadas na construção da ferramenta foram:

### Cálculo do aporte mensal

```excel
=Salário*30%
```

### Projeção do patrimônio

```excel
=FV(taxa_mensal;qtd_anos*12;aporte*-1)
```

### Estimativa de dividendos

```excel
=Patrimônio_Acumulado*rendimento_carteira
```

### Chaves da tabela auxiliar

A aba `APOIO` utiliza uma combinação entre perfil e tipo de FII para criar uma chave de consulta:

```excel
=Perfil&"-"&Tipo_de_FII
```

Essa estrutura permite organizar e consultar os percentuais de distribuição dos diferentes perfis.

---

# 📚 O que foi aprendido

Durante o desenvolvimento do projeto, foram praticados conceitos importantes relacionados à construção de planilhas financeiras e documentação técnica.

### Excel

* Organização de dados;
* Criação de simuladores;
* Fórmulas financeiras;
* Cálculo de juros compostos;
* Projeção de valores;
* Referências entre células;
* Tabelas auxiliares;
* Organização de cenários.

### Git e GitHub

* Criação de repositório;
* Versionamento do projeto;
* Organização de arquivos;
* Utilização do `README.md`;
* Documentação técnica;
* Compartilhamento de projetos.

---

# 🚀 Como utilizar

1. Baixe o arquivo `PROJETO.xlsx`.
2. Abra o arquivo no Microsoft Excel.
3. Acesse a aba `PROJETO-DIO`.
4. Altere os valores de acordo com o cenário que deseja simular.
5. Observe os resultados calculados automaticamente.
6. Consulte a aba `APOIO` para visualizar a distribuição dos perfis e tipos de FII.

---

# 📌 Observações

Os resultados apresentados neste projeto dependem diretamente das premissas utilizadas na planilha.

A simulação não considera todas as variáveis existentes no mercado financeiro e não representa uma previsão de rentabilidade futura.

O objetivo principal é **demonstrar a aplicação prática do Excel na criação de uma ferramenta de simulação de investimentos**, além de desenvolver conhecimentos de organização, documentação e publicação de projetos no GitHub.

---

# 🎓 Desafio DIO

Este projeto foi desenvolvido como parte de um desafio do **Bootcamp da DIO**, cujo objetivo é colocar em prática conhecimentos relacionados à criação de ferramentas de simulação de investimentos em Excel e documentação técnica.

### Objetivos de aprendizagem aplicados

* Criação de ferramentas de simulação de investimentos;
* Aplicação de cálculos financeiros;
* Projeção de patrimônio;
* Estimativa de dividendos;
* Documentação técnica;
* Utilização do GitHub para compartilhamento do projeto.

---

# 👨‍💻 Autor

**Cristiano Bonifácio**

Estudante de Tecnologia com foco em:

* Segurança da Informação
* Cybersecurity
* Cloud Computing
* Infraestrutura de TI
* Linux
* Redes
* Python

---

## 📎 Projeto

**Arquivo principal:** `PROJETO.xlsx`

Este repositório contém a planilha desenvolvida para o desafio, juntamente com sua documentação técnica.

---

⭐ Se este projeto foi útil para você, considere deixar uma estrela no repositório.