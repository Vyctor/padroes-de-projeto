# Padrões de projeto em Java na prática

## O que é um padrão de projeto?

Um padrão de projeto descreve um problema que ocorre frequentemente e então apresenta o cerne da solução para aquele problema, de modo
tal que você pode usar esta solução milhares de vezes, sem nunca fazer a mesma coisa.

## Padrões Criacionais

"Os padrões criacionais fornecem vários mecanismos de criação de objetos, que aumentam a flexibilidade e reutilização de código já existente.
Fornece uma interface para criar objetos em uma superclasse, mas permite que as subclasses alterem o tipo de objetos que serão criados."

-- Chistopher Alexander

### Factory Method

Um padrão que define uma interface para criar um objeto, ams permite às classes decidirem qual classe instanciar.
O factory method permite a uma classe deferir a instanciação para subclasses.

#### Problema

1. Como posso escrever um código onde as classes instanciadas possam variar dentro de uma mesma interface?
2. Como deixar o meu código desacoplado das classes concretas.

#### Solução

1. Extrair a lógica de criação dos objetos para um factory method
2. Invocar o factory para receber uma instância qualquer que implemente uma determinada interface
