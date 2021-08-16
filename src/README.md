Heroku project name <br>
ourpeopleapi-live

```mermaid
erDiagram
     Person ||--o{ Phone : has
     Person {
        int ID
        string firstName
        string lastName
        int CPF
        int birthDay
    }
    Phone {
        int ID
        PhoneType type
        string number
    } 
```
GenerationType.IDENTITY, na anotação @GeneratedValue,
atribui ao BD a geração do id com estratégia incremental (IDENTITY).
```java
@GeneratedValue(strategy = GenerationType.IDENTITY)
```