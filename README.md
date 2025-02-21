# Decola Tech 2025
Java RESTful API criada para o Decola Tech 2025.

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        +String name
        +Account account
        +List<Feature> features
        +List<News> news
        +Card card
    }

    class Account {
        +String number
        +String agency
        +Float balance
        +Float limit
    }

    class Feature {
        +String icon
        +String description
    }

    class News {
        +String icon
        +String description
    }

    class Card {
        +String number
        +Float limit
    }

    User "1" --> "1" Account
    User "1" --> "*" Feature
    User "1" --> "*" News
    User "1" --> "1" Card


