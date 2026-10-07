# SRM CREDIT

###### versão: 0.1
###### fase: 0 Spec 
###### Status: Premissas para implementação inicial


## 1. Objetivo

O SRM credit Engine será responsável por receber lotes de direitos creditorios,
calcular o valor de aquisição e considerando deságio, risco e mmoeda; registrar de forma 
precisa e auditavel.

O sistema deve suportar inicialmente as moedas **BRL** e **USD**, utilizando precisão decimal para operações financeiras

Abaixo as premissas adotadas para implementação 

Unidade de prazo: dias corridos

Taxa base: 1% am

Origem da taxa base por parâmetro

Composição da taxa: Soma + spread

Juros: Compostos

Politica de arredondamento: HALF_EVEN, 2 casas


### 2.Perguntas para o negocio:

Como o risco e definido/classificado ?

Qual a fonte da TAXA ?

Juros são compostos ou simples ?

qual a fonte da contação ?

qual a politica de arredondamento ?

Qual a taxa de cambio deve ser usada na conversão ?

### 3.Criterios de aceite

#### 3.1 Usabilidade
O usuário deverá conseguir informar os dados necessários para transação sem depender de conhecimento técnico.

O sistema deverá apresentar claramente moeda, valor original, prazo, taxas, deságio e valor líquido.

Valores monetários deverão ser apresentados com separadores e casas decimais adequados ao padrão financeiro.

Erros de validação deverão indicar claramente qual informação precisa ser corrigida.

**Decisões de precisão numérica**: arredondamento Half_even 2 casas

