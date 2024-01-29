# DIO - Curso Java 
API RestFul com Spring Boot

## Diagrama de Classe

```mermaid
classDiagram
    class Person {
        -String name
        -Account account
        -List<Feature> features
        -Card card
        -List<News> news
        +Person(String name)
    }
    class Account {
        -String number
        -String agency
        -double balance
        -double limit
    }
    class Feature {
        -String icon
        -String description
    }
    class Card {
        -String number
        -double limit
    }
    class News {
        -String icon
        -String description
    }
    Person "1" *-- "1" Account
    Person "1" *-- "N" Feature
    Person "1" *-- "1"Card
    Person "1" *-- "N" News
