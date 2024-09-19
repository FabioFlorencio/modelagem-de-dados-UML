# 📚 Curso Modelagem de domínio e modelagem conceitual 🧱

O curso de Modelagem de Domínio e Modelagem Conceitual ensina a representar de forma abstrata sistemas e suas interações, identificando entidades, relacionamentos e regras de negócio. Foca em traduzir o mundo real em modelos que guiam o desenvolvimento de sistemas de informação.

---

- [📚 Curso Modelagem de domínio e modelagem conceitual 🧱](#-curso-modelagem-de-domínio-e-modelagem-conceitual-)
  - [🤔 Entendendo modelagem de  domínio e modelagem  conceitual](#-entendendo-modelagem-de--domínio-e-modelagem--conceitual)
    - [Modelagem de domínio](#modelagem-de-domínio)
    - [O que é modelo de domínio?](#o-que-é-modelo-de-domínio)
    - [Níveis de abstração do modelo de domínio.](#níveis-de-abstração-do-modelo-de-domínio)
    - [Nível Conceitual ou de análise (de negócio)](#nível-conceitual-ou-de-análise-de-negócio)
    - [Nível Conceitual ou de análise (de sistema)](#nível-conceitual-ou-de-análise-de-sistema)
    - [Nível Lógico ou de Design (Relacional)](#nível-lógico-ou-de-design-relacional)
    - [Nível Lógico ou de Design (Orientado a objetos)](#nível-lógico-ou-de-design-orientado-a-objetos)
    - [Nível Físico ou de implementação (relacional)](#nível-físico-ou-de-implementação-relacional)
    - [Nível Físico ou de implementação (orientado a objetos)](#nível-físico-ou-de-implementação-orientado-a-objetos)
    - [Polêmica sobre análise \& design](#polêmica-sobre-análise--design)
    - [Paradigma estruturado / relacional](#paradigma-estruturado--relacional)
    - [Paradigma orientado a objetos](#paradigma-orientado-a-objetos)
  - [📊 Modelo Conceitual (Conceitos e atributos)](#-modelo-conceitual-conceitos-e-atributos)
    - [Modelo Conceitual](#modelo-conceitual)
    - [Conceitos](#conceitos)
    - [Atributos](#atributos)
    - [Usando diagrama de classes da UML para  representar conceitos e atributos](#usando-diagrama-de-classes-da-uml-para--representar-conceitos-e-atributos)




## 🤔 Entendendo modelagem de  domínio e modelagem  conceitual


O desenvolvimento de software é dividido em fases:


![alt text](img/desv-sof-fases.png)


### Modelagem de domínio

![alt text](img/model-dominio.png)

---

### O que é modelo de domínio?

**Domínio:** é a área de negócio observada.

**Modelo de domínio:** é a área de negócio que descreve .
* As entidades do domínio
* As inter-relações entre elas


![alt text](img/compare-modelos.jpg)



### Níveis de abstração do modelo de domínio.



|  Nível                                       |  Responsável         | Objetivo                   |
|:---------------------------------------------|:---------------------|:---------------------------|
|**Conceitual** ou de <br> análise(de negócio) | Analista de negócio  |Descrever as entidades do domínio (**do negócio**) e suas inter-relações:<br> **Independente de SISTEMA**|
|**Conceitual** ou de <br> análise(de sistema) | Analista de sistemas |Descrever as entidades do domínio (**do sistema**) e suas inter-relações:<br> **\* Independente de PARADIGMA E TECNOLOGIA**|
|**Lógico** ou de Design                       | Projetista           |Descrever as entidades do domínio (**do sistema**) e suas inter-relações:<br>**\* Preso a um PARADIGMA (ex:relacional, orientado a objetos)** <br>**\*  Independente de TECNOLOGIA**|
|**Físico** ou de <br> implementação           | Implementador        |Descrever as entidades do domínio (**do sistema**) e suas inter-relações:<br>**\* Preso a um PARADIGMA (ex:relacional, orientado a objetos)** <br>**\* Preso a uma TECNOLOGIA(ex: Java, C#, etc)**|


### Nível Conceitual ou de análise (de negócio)

![nivel conceitual](img/nivel-conceito-negocio.jpg)


### Nível Conceitual ou de análise (de sistema)

![nivel conceitual sistema](img/nivel-conceito-sistema.jpg)


### Nível Lógico ou de Design (Relacional)

Paradigma: **relacional**

![alt text](img/nivel-logico.png)

### Nível Lógico ou de Design (Orientado a objetos)

Paradigma: **orientado a objetos**


![alt text](img/paradigma-oo.jpg)


### Nível Físico ou de implementação (relacional)

* **Relacional**

![alt text](img/implementacao-relacional.png)


### Nível Físico ou de implementação (orientado a objetos)

* **Orientado a objetos**

![alt text](img/implementacao-oo.png)


### Polêmica sobre análise & design

* **Análise:** descrever o PROBLEMA (independente de paradigma e tecnologia)
* **Design:** descrever a SOLUÇÃO (preso ao paradigma)

![alt text](img/polemica-analise-design.png)

### Paradigma estruturado / relacional

* **Chaves estrangeiras**
* **Criação de tabelas**
* **Normalização**
* **Outros...**


![alt text](img/paradigma-estruturado-relacional.png)

### Paradigma orientado a objetos

* **Inclusão de métodos**
*  **Normalização (?)**


![alt text](img/paradigma-oo.jpg)

---

## 📊 Modelo Conceitual (Conceitos e atributos)

### Modelo Conceitual

**Definição 1** é um modelo que descreve a estrutura das  informações que o sistema vai gerenciar (Wazlawick)
**Definição 2** é o Modelo de Domínio em nível de Análise:
* Pertence ao escopo do problema e não ao escopo da solução
* Independente de paradigma
* Independente de tecnologia

![](img/modelo-conceitual.jpg)


### Conceitos

* Um conceito pode ser qualquer entidade que tenha um significado para o  sistema e que tenha uma necessidade de armazenamento de dados.
* Um conceito deve ser uma unidade coesa, ou seja, **não se deve misturar informações de várias coisas distintas em um mesmo conceito**.

### Atributos

* **Informações alfanuméricas simples, como números, textos, datas,  etc. contidas em cada conceito.**
* Produto: descrição, preço
* Cliente: nome, email, telefone, CPF, dataNascimento
  

* Notas(1FN - 1° Forma normal)
  * ❌Não pode ser multivalorado
    * Exemplo: telefones ("3736-3938, 9988-3346, 3210-3939")
  
  * ❌Não pode ser composto
    * Exemplo: endereço ("Rua Floriano Peixoto, n° 250, apto 302, Bairro Copacabana, CEP 38410-384")


### Usando diagrama de classes da UML para  representar conceitos e atributos

![](img/class-uml-conceito.jpg)



