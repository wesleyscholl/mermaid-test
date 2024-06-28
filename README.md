# mermaid-test

```mermaid
graph LR
    A[Square Rect] -- Link text --> B((Circle))
    A --> C(Round Rect)
    B --> D{Rhombus}
    C --> D
    D --> E
```

```mermaid
classDiagram
 
    BookStore <|-- Book
 
    BookStore <|-- Author
 
    BookStore : +String location
 
    BookStore : +int totalBooks
 
    BookStore: +findBook()
 
    BookStore: +getAuthor()
 
    class Book{
 
        +String title
 
        +int publicationYear
 
        +read()
 
    }
 
    class Author{
 
        -String name
 
        -write()
```

```mermaid
graph LR
 
Mindmap --> Idea1
 
Mindmap --> Idea2
 
Idea1 --> SubIdea1
 
Idea2 --> SubIdea2
 
style Mindmap fill:#F9D6A1
 
style Idea1 fill:#A1D6F9
 
style Idea2 fill:#A1D6F9
 
style SubIdea1 fill:#A1D6F9
 
```

```mermaid
graph TB
    sq[Square shape] --> ci((Circle shape))

    subgraph A
        od>Odd shape]-- Two line<br/>edge comment --> ro
        di{Diamond with <br/> line break} -.-> ro(Rounded<br>square<br>shape)
        di==>ro2(Rounded square shape)
    end

    %% Notice that no text in shape are added here instead that is appended further down
    e --> od3>Really long text with linebreak<br>in an Odd shape]

    %% Comments after double percent signs
    e((Inner / circle<br>and some odd <br>special characters)) --> f(,.?!+-*ز)

    cyr[Cyrillic]-->cyr2((Circle shape Начало));

     classDef green fill:#9f6,stroke:#333,stroke-width:2px;
     classDef orange fill:#f96,stroke:#333,stroke-width:4px;
     class sq,e green
     class di orange

```
