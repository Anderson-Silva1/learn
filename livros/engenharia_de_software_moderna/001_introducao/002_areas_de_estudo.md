# O que se Estuda em Engenharia de Software?

Segundo SWEBOK, podemos dividir em 12 áreas de conhecimento:

* Engenharia de Requisitos
* Projeto de Software
* Construção de Software
* Testes de Software
* Manutenção de Software
* Gerência de Configuração
* Gerência de Projetos
* Processos de Software
* Modelos de Software
* Qualidade de Software
* Prática Profissional
* Aspectos Econômicos

Porém, temos mais 3 áreas de estudo, mas são consideradas áreas de fronteira, trataremos delas posteriormente... São elas: 

* Fundamentos de Computação
* Fundamentos de Matemática
* Fundamentos de Engenharia

---

## Engenharia de Requisitos

Engenharia de Requisitos inclui o conjunto de atividades realizadas com o objetivo de definir, analisar, documentar e validar os requisitos de um sistema. 

Possuímos 2 tipos de Requisitos:

* Funcionais
* não funcionais

### Requisitos Funcionais

Requisitos funcionais definem o que um sistema deve fazer; isto é, quais funcionalidades ou serviços ele deve implementar.

Exemplo: Um sistema bancário deve mostrar saldo, isso é um requisito funcional

### Requisitos não funcionais

Requisitos não funcionais definem como um sistema deve operar

Exemplo: Um sistema bancário, ele deve mostrar o saldo em 1 segundo e estar disponível 99% do tempo para os usuários...

São outros exemplos de Requisitos não funcionais:

* *Desempenho*: informar o saldo da conta em menos de 3 segundos;

* *Disponibilidade*: estar no ar 99% do tempo;

* *Tolerância a falhas*: continuar operando mesmo se um determinado centro de dados cair;

* *Segurança*: criptografar todos os dados trocados com as agências;

* *Privacidade*: não disponibilizar para terceiros dados de clientes;

* *Interoperabilidade*: integrar-se com os sistemas do Banco Central;

* *Capacidade*: ser capaz de armazenar dados de 1 milhão de clientes;

* *Usabilidade*: ter uma versão para deficientes visuais.

## Projeto de Software

Durante a criação de um software são definidas unidades de código, porém apenas a nível de interfaces...

Possuímos 2 tipos de interfaces quando trabalhamos com software:

* Providas
* Requeridas

### Interfaces Providas

Interfaces providas são aqueles serviços que uma unidade de código torna público para uso pelo resto do sistema

### Interfaces Requeridas

Interfaces requeridas são aquelas interfaces das quais uma unidade de código depende para funcionar, onde também chamamos de dependência.

Exemplo:

```ts
export class ContaBancaria {
    private cliente: Cliente
    private saldo: Number
}
```

Nesse cenário, a classe ContaBancaria fornece uma interface para o funcionamento do sistema, logo ela é uma **Interface Provida**... Em contra mão, temos outra classe que está abstrata chamada Cliente, essa logo é uma **Interface Requerida** pois é uma dependência da classe ContaBancaria

## Construção de Software

O profissional que trabalha nessa área vai ser responsável por colocar a mao na massa e escrever os códigos, tal como tomar decisões importantes como:
* Qual a estrutura de dados e Algoritmos que serão usados?
* Quais bibliotecas e Frameworks serão usados?
* Quais técnicas de tratamento de Exceções?
* Qual o padrão de nomes, layout e documentação o sistema terá?
* Quais ferramentas serão usadas? (Isso inclui base de dados, compiladores, IDEs e etc...)