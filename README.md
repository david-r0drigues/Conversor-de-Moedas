>[Projeto ONE - Oracle Next Education](https://www.oracle.com/br/education/oracle-next-education/)

![img_2.png](img_2.png)

>Conversor de Moedas
> 
>[David Rodrigues  Turma 6 - 2024 ](https://www.linkedin.com/in/david-rodrigues-06069a244/)

Este é um projeto simples de conversor de moedas que interage com o usuário via console. Ele permite converter valores entre diferentes moedas usando taxas de câmbio atualizadas de uma API.
Estrutura do Projeto

   
    
    conversorDeMoedas/
    │
    ├── README.md/
    ├── src/
    │   ├── main/
    │   │   ├── java/
    │   │   │   ├── Conversor.java
    │   │   │   ├── ConversorDeMoedas.java
    │   ├── resources/
    ├── pom.xml

    
Conversor.java: Esta classe contém métodos para buscar as taxas de câmbio de uma API e realizar as conversões entre as moedas.
ConversorDeMoedas.java: Esta é a classe principal que contém a lógica de interação com o usuário via console.

Dependências

Este projeto utiliza a biblioteca JSON para processar as respostas da API. A dependência é gerenciada pelo Maven e está definida no arquivo pom.xml.
Adicionando Dependência JSON no pom.xml

- xml
- <dependency>
    <groupId>org.json</groupId>
    <artifactId>json</artifactId>
    <version>20240303</version>
</dependency>


*Pré-requisitos*

- *Java Development Kit (JDK) instalado.*

- *Maven instalado para gerenciamento de dependências.*

- *IntelliJ IDEA ou outro IDE de sua preferência.*

Interação com o Programa

    O programa atualizará automaticamente as taxas de câmbio ao iniciar.
    Será exibido um menu com as opções de conversão:
**************************************
    Conversor de Moedas

    1. Dólar (USD) para Euro (EUR)
    2. Euro (EUR) para Dólar (USD)
    3. Dólar (USD) para Real (BRL)
    4. Real (BRL) para Dólar (USD)
    5. Euro (EUR) para Real (BRL)
    6. Real (BRL) para Euro (EUR)
    7. Sair
**************************************
    Escolha a opção da moeda para converter:
    Digite o valor a ser convertido:
O programa exibirá o valor convertido e a taxa de câmbio atual.

Você poderá reiniciar o processo ou escolher a opção 7 para sair do programa.

Exemplo de Uso:

    Conversor de Moedas
    1. Dólar (USD) para Euro (EUR)
    2. Euro (EUR) para Dólar (USD)
    3. Dólar (USD) para Real (BRL)
    4. Real (BRL) para Dólar (USD)
    5. Euro (EUR) para Real (BRL)
    6. Real (BRL) para Euro (EUR)
    7. Sair
      Escolha a opção da moeda para converter: 1
      Digite o valor a ser convertido: 100
      Convertemos o valor: 100.00 USD para 92.00 EUR
      Taxa de câmbio atual: 1 USD = 0.9200 EUR

Implementação

O programa foi desenvolvido em Java, utilizando a biblioteca JSON para manipulação das respostas da API. A lógica de conversão está encapsulada na classe Conversor, enquanto a classe ConversorDeMoedas gerencia a interação com o usuário.
API Utilizada

A API utilizada para obter as taxas de câmbio é a ExchangeRate-API. A chave da API é inserida diretamente no código para simplificar o exemplo.