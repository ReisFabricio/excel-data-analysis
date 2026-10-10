**Controle de Manutenção Preventiva**

Planilha em Excel para acompanhar as manutenções preventivas, reunindo as Ordens de Serviço (OS), os responsáveis, os status das atividades e os prazos de conclusão.

O objetivo é tornar o acompanhamento mais simples, visual e organizado, facilitando a consulta das OS, o monitoramento dos prazos e a identificação de atrasos.

<!-- Para exibir uma imagem do painel: salve a captura em uma pasta "imagens" e use ![Painel de Controle de Manutenção Preventiva](imagens/painel.png) -->
O que a planilha faz
Permite escolher, em uma lista suspensa, um responsável específico ou a opção "Geral".
Mostra a quantidade de OS abertas, em andamento e concluídas. Em "Geral", considera todos os responsáveis, e ao escolher um nome, mostra só as OS dele.
Calcula o desvio de prazo das OS concluídas, em dias:
concluída antes do prazo: dias de antecedência;
concluída no prazo: zero;
concluída depois do prazo: valor negativo, destacado em vermelho.
Exibe no título a data de referência do acompanhamento.
Recursos e fórmulas utilizados
Recurso	Para que serve no projeto
Validação de dados	Lista suspensa com os responsáveis e a opção "Geral"
CONT.SES	Contagem das OS por status, respeitando o responsável selecionado
SE + DATADIF	Diferença, em dias, entre a data prevista e a data de conclusão
Formatação condicional	Destaque em vermelho dos resultados negativos (conclusão após o prazo)
SE	Adapta os resultados ao responsável selecionado e às condições definidas
HOJE	Exibe a data de referência no título da planilha

A função HOJE() mostra a data do dia em que a planilha é aberta, e não a data da última edição.

**Como usar**

1. Baixe o arquivo ordens_de_servico.xlsx.
2. Abra a aba resumo.
3. Na lista suspensa, escolha um responsável ou "Geral".
4. Acompanhe as quantidades por status e os desvios de prazo.

Os dados de apoio também estão disponíveis em formato .csv, na pasta materiais-de-apoio.

Estrutura do repositório
.
├── ordens_de_servico.xlsx
├── materiais-de-apoio/
│   └── ordens_de_servico.csv
└── README.md
Principal aprendizado

Colocar em prática recursos do Excel para transformar dados em informações claras e úteis, usando fórmulas, filtros e formatação para facilitar o acompanhamento das atividades.

Autor

Fabrício Reis,  em transição para a área de tecnologia e cursando Engenharia de Software.

🔗 https://www.linkedin.com/in/fabricio-reis-5986b92b1/
