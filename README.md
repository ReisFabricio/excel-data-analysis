# Controle de Manutenção Preventiva

Planilha em Excel desenvolvida para acompanhar as manutenções preventivas, reunindo Ordens de Serviço (OS), responsáveis, status das atividades e prazos de conclusão. O objetivo é tornar o acompanhamento mais simples, visual e organizado, facilitando a consulta das OS, o monitoramento dos prazos e a identificação de atrasos.

<!-- Para exibir uma imagem do painel: salve a captura em uma pasta "imagens" e use ![Painel de Controle de Manutenção Preventiva](imagens/painel.png) -->

---

## 🚀 O que a planilha faz

* **Filtro dinâmico:** Permite escolher, através de uma lista suspensa, um responsável específico ou a opção "Geral".
* **Indicadores inteligentes:** Mostra a quantidade de OS abertas, em andamento e concluídas de forma automática conforme o filtro aplicado.
* **Cálculo de desvio de prazo:** Calcula os dias de diferença nas OS concluídas:
  * **Antes do prazo:** Dias de antecedência.
  * **No prazo:** Zero dias.
  * **Depois do prazo:** Valor negativo (destacado em vermelho).
* **Data de referência:** Exibe no título a data de atualização do acompanhamento. *(Nota: A função HOJE() mostra a data do dia em que a planilha é aberta).*

---

## 🛠️ Recursos e fórmulas utilizados

| Recurso | Para que serve no projeto |
| :--- | :--- |
| **Validação de dados** | Criação da lista suspensa com os responsáveis e a opção "Geral". |
| **CONT.SES** | Contagem das OS por status, respeitando o responsável selecionado. |
| **SE + DATADIF** | Cálculo da diferença, em dias, entre a data prevista e a data de conclusão. |
| **Formatação condicional** | Destaque em vermelho dos resultados negativos (conclusão após o prazo). |
| **SE** | Adaptação dos resultados ao responsável selecionado e às condições definidas. |
| **HOJE** | Exibição dinâmica da data de referência no título da planilha. |

---

## 📦 Como usar

1. Baixe o arquivo `ordens_de_servico.xlsx`.
2. Abra a aba **resumo**.
3. Na lista suspensa, escolha um responsável ou selecione **"Geral"**.
4. Acompanhe as quantidades por status e os desvios de prazo.

*(Os dados de apoio originais também estão disponíveis em formato `.csv` na pasta `materiais-de-apoio`)*.

---

## 📂 Estrutura do repositório

```text
.
├── ordens_de_servico.xlsx
├── materiais-de-apoio/
│   └── ordens_de_servico.csv
└── README.md
