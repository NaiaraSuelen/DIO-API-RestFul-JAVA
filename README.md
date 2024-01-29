#DIO - Curso Java 

##Criando uma API RestFul com Spring Boot

markdown
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
    Person --> Account
    Person --> Feature
    Person --> Card
    Person --> News
