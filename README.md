# Sistema de Gestão para Empresa Farmacêutica   ![image](https://github.com/user-attachments/assets/9440b2ae-e5e9-4a5c-ac1d-f65eea3db02d)

![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=30&pause=1000&color=3DDC84&width=435&lines=Projeto+Theravita;)

### Integrantes:

- Gabriel Bachega 
- Gabriel Oliveira Mendes Silva
- Luiz Fernando Moreira Domênico
- Rafael de Godoy Vianna
- Rafael de Palma Francisco

## Descrição
<br>

Este sistema foi desenvolvido para uma empresa farmacêutica em expansão nacional, que possui 20 funcionários distribuídos em sete setores:  
Gerente de Filial, Atendimento ao Cliente, Gestão de Pessoas, Financeiro, Vendas, Almoxarifado e Transportadoras.  

O sistema visa solucionar problemas de controle de dados da empresa, incluindo o monitoramento de funcionários, estoque, ações dos setores, controle financeiro e fluxo de caixa.  

Principais funcionalidades:  
- Registro da quantidade de funcionários em cada setor, com dados pessoais (nome completo, ID, idade e gênero).  
- Gestão detalhada dos salários, considerando impostos, benefícios (vale transporte, vale refeição e alimentação), planos de saúde e odontológico, além de bonificações por participação nos lucros.  
- Controle de entradas e saídas no caixa, catálogo de produtos (mínimo 10 produtos), seus valores de compra, venda e quantidades em estoque.  
- Cadastro e consulta das transportadoras parceiras (mínimo 3), com seus locais de atendimento.  
- Apresentação do caixa total inicial (R$ 200.000,00) e estimativa de lucros mensais e anuais com base nas vendas previstas.  
- Acompanhamento dos negócios em andamento, incluindo quantidade de negócios abertos e os funcionários envolvidos (vendedores e almoxarifado).
<br>

## Funcionalidades

- Controle completo dos funcionários por setor, incluindo dados pessoais e quantitativos  
- Cálculo avançado de salários, impostos, benefícios e bonificações  
- Catálogo de produtos com gestão de estoque e preços  
- Registro e consulta das transportadoras parceiras e regiões atendidas  
- Gestão financeira do caixa, com fluxo de entradas e saídas e estimativa de lucros  
- Monitoramento dos negócios em andamento e envolvidos em processos de venda e compra  
<br>

## Tecnologias Utilizadas

#### BackEnd
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=java,mysql" />
  </a>
</p>

#### FrontEnd
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=html,css,js" />
  </a>
</p>

#### Framework
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=spring,postman" />
  </a>
</p>

## Repositórios Extras

- [Repositório Framework](https://github.com/Rafael-Francisco21/ProjetoSenaiFramework.git)

- [Repositório Front-end](https://github.com/gabrielbachega1/front-theravita.git)

- [Repositório Integração de Banco de Dados](https://github.com/Lfdomenico/ProjetoSenaiBD.git)

- [Link para o Postman](https://www.postman.com/theravita/workspace/theravita/request/30232619-f4113e28-ad1b-4474-8af6-b5a9d8ccc601?action=share&creator=30232619&ctx=documentation)

<br>

# [SLIDES](https://www.canva.com/design/DAGqhFFTsGE/DcCIIW6QIAZ0YbAZsSZVjQ/edit?utm_content=DAGqhFFTsGE&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton) #

![image](https://github.com/user-attachments/assets/c16cbcb2-90e2-440b-be71-4fd526a3e524)




# [DIAGRAMA DE CLASSES](https://github.com/user-attachments/files/20729387/Diagrama.de.Classes.pdf) #


![image](https://github.com/user-attachments/assets/a496b6ff-44a8-4160-bfea-4dc13b6217ee)




 
 ## Requisitos Funcionais
 <br>

***Gestão de Funcionários***


| Código   | Descrição                                                                           | Prioridade | Dependências |
| -------- | ----------------------------------------------------------------------------------- | ---------- | ------------ |
| **RF01** | Cadastrar funcionários, incluindo: nome completo, ID, idade, gênero, setor e cargo. | **M**   | Nenhuma      |
| **RF02** | Consultar a lista de funcionários por setor.                                        | **S** | RF01         |
| **RF03** | Atualizar dados dos funcionários (nome, idade, gênero, cargo e setor).              | **M**   | RF01         |
| **RF04** | Excluir funcionários do cadastro (em caso de demissão ou desligamento).             | **M**   | RF01         |
| **RF05** | Visualizar o total de funcionários por setor.                                       | **S** | RF01, RF02   |
<br>

***Gestão de Salários e Benefícios***


| Código   | Descrição                                                                                                                                                                                                                                                            | Prioridade | Dependências |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ------------ |
| **RF06** | Calcular automaticamente o salário bruto e líquido de cada funcionário, considerando impostos, vale transporte, vale refeição (R\$300, podendo variar conforme cargo), plano de saúde (mínimo R\$3000, podendo variar), plano odontológico (R\$3000) e bonificações. | **M**   | RF01, RF07   |
| **RF07** | Consultar e atualizar os valores dos benefícios, impostos e bonificações.                                                                                                                                                                                            | **M**   | Nenhuma      |
| **RF08** | Emitir demonstrativo salarial dos funcionários.                                                                                                                                                                                                                      | **S** | RF06         |
<br>

***Gestão de Produtos e Estoque***


| Código   | Descrição                                                                                            | Prioridade | Dependências |
| -------- | ---------------------------------------------------------------------------------------------------- | ---------- | ------------ |
| **RF09** | Cadastrar produtos, contendo: nome, código, preço de compra, preço de venda e quantidade em estoque. | **M**   | Nenhuma      |
| **RF10** | Consultar a lista de produtos cadastrados.                                                           | **S** | RF09         |
| **RF11** | Atualizar informações dos produtos (preço, quantidade, descrição).                                   | **M**   | RF09         |
| **RF12** | Controlar entradas (reposição) e saídas (vendas) de produtos no estoque.                             | **M**   | RF09, RF11   |
| **RF13** | Verificar disponibilidade de produtos para venda.                                                    | **M**   | RF09, RF12   |
<br>

***Gestão Financeira e Caixa***


| Código   | Descrição                                                                     | Prioridade | Dependências           |
| -------- | ----------------------------------------------------------------------------- | ---------- | ---------------------- |
| **RF14** | Registrar entradas de caixa (vendas, investimentos, etc.).                    | **M**   | RF09, RF12, RF23       |
| **RF15** | Registrar saídas de caixa (salários, compras, despesas gerais).               | **M**   | RF06, RF09, RF12, RF23 |
| **RF16** | Visualizar o saldo atual do caixa.                                            | **M**   | RF14, RF15             |
| **RF17** | Gerar uma estimativa de lucro mensal e anual com base nas vendas programadas. | **S** | RF14, RF15, RF23       |
| **RF18** | Gerar relatório financeiro (entradas, saídas e saldo).                        | **S** | RF14, RF15, RF16       |
<br>

***Gestão de Transportadoras***


| Código   | Descrição                                                                                                         | Prioridade | Dependências |
| -------- | ----------------------------------------------------------------------------------------------------------------- | ---------- | ------------ |
| **RF19** | Cadastrar transportadoras com os seguintes dados: nome, ID e áreas de cobertura (municípios, regiões ou estados). | **M**   | Nenhuma      |
| **RF20** | Consultar a lista de transportadoras e suas áreas de atendimento.                                                 | **C**  | RF19         |
| **RF21** | Atualizar os dados das transportadoras (nome, áreas de atendimento).                                              | **M**   | RF19         |
| **RF22** | Visualizar quantidade total de transportadoras parceiras.                                                         | **C**  | RF19, RF20   |
<br>

***Gestão de Negócios em Andamento***


| Código   | Descrição                                                                                                                                                                        | Prioridade | Dependências     |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------------- |
| **RF23** | Registrar negócios em andamento, identificando tipo (venda ou compra), produtos envolvidos, quantidade e funcionários envolvidos (vendedores ou responsáveis pelo almoxarifado). | **M**   | RF01, RF09, RF13 |
| **RF24** | Consultar todos os negócios em andamento.                                                                                                                                        | **S** | RF23             |
| **RF25** | Atualizar o status de um negócio (em andamento, concluído ou cancelado).                                                                                                         | **M**   | RF23             |
<br>

**LEGENDA**

| Letra | Significado                                                                                   |
| :----: | ------------------------------------------------------------------------------------------- |
|  **M** | **Must** – Obrigatório, essencial para o funcionamento básico do sistema.                   |
|  **S** | **Should** – Importante, mas não impede o funcionamento caso não esteja na primeira versão. |
|  **C** | **Could** – Desejável, agrega valor, mas não é essencial.                                   |

