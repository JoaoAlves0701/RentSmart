# RentSmart — Sistema de Orçamento de Locação

## Descrição do projeto

O **RentSmart** é um programa desenvolvido em Python para simular orçamentos de locação de imóveis da imobiliária fictícia R.M Imóveis. A aplicação calcula o aluguel mensal com base no tipo de imóvel, nos adicionais selecionados e nos descontos aplicáveis. Também calcula a taxa contratual e gera uma projeção financeira para os 12 primeiros meses de locação.

O projeto foi desenvolvido como atividade acadêmica da disciplina **Algorithmic Thinking & Introduction to Object-Oriented Programming**.

## Funcionalidades

- Escolha entre apartamento, casa e estúdio.
- Cálculo dos adicionais de quarto e garagem, conforme o tipo de imóvel.
- Desconto de 5% para apartamento quando o cliente informa não possuir crianças.
- Taxa contratual de R$ 2.000,00, parcelável de 1 a 5 vezes.
- Exibição do valor mensal do aluguel, separadamente da taxa contratual.
- Validação das principais entradas informadas pelo usuário.
- Geração do arquivo `projecao_12_meses.csv` com os valores previstos para 12 meses.

## Regras de negócio

| Regra | Valor |
| --- | ---: |
| Apartamento com 1 quarto | R$ 700,00/mês |
| Casa com 1 quarto | R$ 900,00/mês |
| Estúdio | R$ 1.200,00/mês |
| Segundo quarto em apartamento | + R$ 200,00/mês |
| Segundo quarto em casa | + R$ 250,00/mês |
| Garagem em apartamento ou casa | + R$ 300,00/mês |
| Pacote de 2 vagas no estúdio | + R$ 250,00/mês |
| Vaga adicional no estúdio | + R$ 60,00/mês |
| Apartamento sem crianças | 5% de desconto sobre o aluguel com adicionais |
| Taxa contratual | R$ 2.000,00 em até 5 parcelas |

## Tecnologias utilizadas

- Python 3
- Biblioteca padrão `csv` do Python
- Visual Studio Code (ambiente de desenvolvimento)

## Organização do código

A classe `Imovel` armazena informações como tipo de imóvel, valor-base, adicionais e descontos. Seus métodos são utilizados para calcular o aluguel mensal. O programa principal recebe as escolhas do usuário, calcula o parcelamento da taxa contratual e gera o CSV com a projeção anual.

## Como executar

1. Instale o **Python 3**.
2. Abra a pasta do projeto no VS Code ou em um terminal.
3. Execute o comando:

```bash
python faculdade.py
```

No Windows, caso necessário, use `py faculdade.py`.

4. Responda às perguntas exibidas no terminal.
5. Consulte o resumo do orçamento e o arquivo `projecao_12_meses.csv` gerado após a simulação.

## Exemplo de simulação

Para um apartamento de 2 quartos, com garagem, sem crianças e com a taxa contratual dividida em 5 parcelas:

- Aluguel-base: R$ 700,00
- Segundo quarto: R$ 200,00
- Garagem: R$ 300,00
- Desconto de 5%: R$ 60,00
- **Aluguel mensal: R$ 1.140,00**
- Parcela contratual (primeiros 5 meses): R$ 400,00
- Total mensal dos meses 1 a 5: R$ 1.540,00
- Total mensal dos meses 6 a 12: R$ 1.140,00
- **Total previsto dos 12 meses: R$ 15.680,00**

## Arquivos do projeto

- `faculdade.py` — código-fonte do sistema.
- `README.md` — instruções e descrição do projeto.
- `projecao_12_meses.csv` — projeção de pagamentos gerada pela aplicação.

## Finalidade acadêmica

Este projeto demonstra o uso de pensamento algorítmico, estruturas condicionais, repetição, validação de entradas, classes, objetos, atributos, métodos e geração de arquivos CSV em Python.
