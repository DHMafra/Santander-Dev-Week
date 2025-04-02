# Santander Dev Week 2023
Java RESTful API criada para a Santander Dev Week

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        -String nome
        -Account account
        -Feature[] features
        -Card card
        -News[] news
    }
    class Account {
        -String Number
        -String Agency
        -String Balance
        -String Limit
    }
    class Feature {
        -String icon
        -String description
    }
    class Card {
        -String Number
        -float Limit
    }
    class News {
        -String icon
        -String Description
    }
    User "1" -- "1" Account 
    User "1" -- "N" Feature 
    User "1" -- "1" Card 
    User "1" -- "N" News 
```
 
