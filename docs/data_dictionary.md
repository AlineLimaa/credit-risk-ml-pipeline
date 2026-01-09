# Data Dictionary — German Credit Dataset

Este documento descreve **todas as variáveis** do dataset **German Credit**, incluindo significados dos códigos categóricos.

---

## Variável Alvo (Target)

| Variável    | Código | Significado |
| ----------- | ------ | ----------- |
| Credit_Risk | 1      | Bom pagador |
| Credit_Risk | 2      | Mau pagador |

---

## Variáveis Categóricas

### 1. Status da Conta Corrente (`Status_Checking_Account`)

| Código | Significado        |
| ------ | ------------------ |
| A11    | Saldo < 0 DM       |
| A12    | 0 ≤ Saldo < 200 DM |
| A13    | Saldo ≥ 200 DM     |
| A14    | Sem conta corrente |

### 2. Histórico de Crédito (`Credit_History`)

| Código | Significado                            |
| ------ | -------------------------------------- |
| A30    | Sem créditos / todos pagos em dia      |
| A31    | Todos pagos em dia                     |
| A32    | Créditos existentes pagos corretamente |
| A33    | Atrasos anteriores                     |
| A34    | Histórico crítico                      |

### 3. Propósito do Crédito (`Purpose`)

| Código | Significado           |
| ------ | --------------------- |
| A40    | Carro novo            |
| A41    | Carro usado           |
| A42    | Móveis / equipamentos |
| A43    | Rádio / TV            |
| A44    | Eletrodomésticos      |
| A45    | Reparos               |
| A46    | Educação              |
| A47    | Férias                |
| A48    | Retreinamento         |
| A49    | Negócios              |
| A410   | Outros                |

### 4. Conta Poupança (`Savings_Account`)

| Código | Significado           |
| ------ | --------------------- |
| A61    | < 100 DM              |
| A62    | 100 ≤ Saldo < 500 DM  |
| A63    | 500 ≤ Saldo < 1000 DM |
| A64    | ≥ 1000 DM             |
| A65    | Sem poupança          |

### 5. Tempo de Emprego (`Employment_Duration`)

| Código | Significado        |
| ------ | ------------------ |
| A71    | Desempregado       |
| A72    | < 1 ano            |
| A73    | 1 ≤ tempo < 4 anos |
| A74    | 4 ≤ tempo < 7 anos |
| A75    | ≥ 7 anos           |

### 6. Status Pessoal e Sexo (`Personal_Status`)

| Código | Significado                    |
| ------ | ------------------------------ |
| A91    | Masculino – divorciado         |
| A92    | Feminino – divorciada / casada |
| A93    | Masculino – solteiro           |
| A94    | Masculino – casado             |
| A95    | Feminino – solteira            |

### 7. Outros Devedores (`Other_Debtors`)

| Código | Significado   |
| ------ | ------------- |
| A101   | Nenhum        |
| A102   | Co-signatário |
| A103   | Fiador        |

### 8. Propriedade (`Property`)

| Código | Significado    |
| ------ | -------------- |
| A121   | Imóvel próprio |
| A122   | Seguro de vida |
| A123   | Carro / outros |
| A124   | Nenhum         |

### 9. Planos de Parcelamento (`Installment_Plans`)

| Código | Significado |
| ------ | ----------- |
| A141   | Banco       |
| A142   | Lojas       |
| A143   | Nenhum      |

### 10. Tipo de Moradia (`Housing`)

| Código | Significado |
| ------ | ----------- |
| A151   | Aluguel     |
| A152   | Própria     |
| A153   | Gratuita    |

### 11. Tipo de Trabalho (`Job`)

| Código | Significado                    |
| ------ | ------------------------------ |
| A171   | Desempregado / não qualificado |
| A172   | Não qualificado                |
| A173   | Qualificado                    |
| A174   | Altamente qualificado          |

### 12. Telefone (`Telephone`)

| Código | Significado |
| ------ | ----------- |
| A191   | Nenhum      |
| A192   | Sim         |

### 13. Trabalhador Estrangeiro (`Foreign_Worker`)

| Código | Significado |
| ------ | ----------- |
| A201   | Sim         |
| A202   | Não         |

---

## Variáveis Numéricas

| Variável                    | Descrição                        |
| --------------------------- | -------------------------------- |
| Duration                    | Duração do crédito (meses)       |
| Credit_Amount               | Valor do crédito                 |
| Installment_Rate            | Percentual da renda comprometida |
| Residence_Since             | Tempo de residência atual (anos) |
| Age                         | Idade do cliente                 |
| Number_of_Existing_Credits  | Número de créditos existentes    |
| Number_of_People_Maintained | Pessoas sob responsabilidade     |

---

## Observações

* O dataset original utiliza **códigos alfanuméricos** para variáveis categóricas.
* Para **EDA e visualizações**, recomenda-se mapear esses códigos para categorias legíveis.
* Para **modelagem**, os dados devem ser devidamente codificados (One-Hot, Ordinal, etc.).
