# Avanade-Dev-Week-2025
Java RESTful API criada para a Santander Dev Week.

## Diagrama de Classes

'''mermaid
classDiagram
    class Usuario {
        -String name
        -Account account
        -Feature[] features
        -Card card
        -News[] news
    }

    class Account {
        -String number
        -String agency
        -float balance
        -float limit
    }

    class Feature {
        -String icon
        -String description
    }

    class Card {
        -String cardNumber
        -float cardLimit
    }

    class News {
        -String icon
        -String description
    }

    Usuario "1" --> "1" Account : possui
    Usuario "1" --> "*" Feature : possui
    Usuario "1" --> "1" Card : possui
    Usuario "1" --> "*" News : possui
'''
