+++
date = '2025-07-31T10:51:01+09:00'
draft = false
title = 'Mermaid'
tag = ['mermaid', 'diagram', 'visualization']
slug = 'mermaid-example'
+++

### 1\. フローチャート (Flowchart)

```mermaid
graph TD
    A[Start] --> B{Choice};
    B -- Yes --> C[Process 1];
    B -- No --> D[Process 2];
    C --> E[End];
    D --> E;
```

{{< mermaid >}}
graph TD
    A[Start] --> B{Choice};
    B -- Yes --> C[Process 1];
    B -- No --> D[Process 2];
    C --> E[End];
    D --> E;
{{< /mermaid >}}

-----

### 2\. シーケンス図 (Sequence Diagram)

```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>Bob: Hello Bob, how are you?
    Bob-->>Alice: I am good thanks!
    Alice->>Bob: See you later.
```

{{< mermaid >}}
sequenceDiagram;
    participant Alice
    participant Bob
    Alice->>Bob: Hello Bob, how are you?
    Bob-->>Alice: I am good thanks!
    Alice->>Bob: See you later.
{{< /mermaid >}}

-----

### 3\. ガントチャート (Gantt Chart)

```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title Project Schedule
    section Design
    Requirements Definition     :a1, 2024-01-01, 7d
    System Design  :a2, after a1, 5d
    section Development
    Frontend :b1, after a2, 10d
    Backend   :b2, after a2, 12d
    section Testing
    Unit Testing    :c1, after b1, 5d
    Integration Testing    :c2, after b2, 7d
```

{{< mermaid >}}
gantt
    dateFormat  YYYY-MM-DD
    title Project Schedule
    section Design
    Requirements Definition     :a1, 2024-01-02, 1M
    System Design  :a2, after a1, 5d
    section Development
    Frontend :b1, after a2, 10d
    Backend   :b2, after a2, 12d
    section Testing
    Unit Testing    :c1, after b1, 5d
    Integration Testing    :c2, after b2, 7d
{{< /mermaid >}}

-----

### 4\. クラス図 (Class Diagram)

```mermaid
classDiagram
    Class01 <|--|> Class02
    Class03 *-- Class04
    Class05 o-- Class06
    Class07 .. Class08
    Class09 -- Class10
    Class11 <|-- Class12
    Class13 --> Class14
    Class15 ..> Class16

    class Animal {
        +name: String
        +age: int
        +eat()
    }
    class Dog {
        -breed: String
        +bark()
    }
    Animal <|-- Dog
```

-----

### 5\. ステート図 (State Diagram)

システムやオブジェクトの状態とその遷移を表現します。

```mermaid
stateDiagram-v2
    [*] --> Off
    Off --> On : turn on
    On --> Off : turn off
    On --> Sleep : sleep
    Sleep --> On : wake up
    Sleep --> Off : turn off
```

{{< mermaid >}}
stateDiagram-v2
    [*] --> Off
    Off --> On : turn on
    On --> Off : turn off
    On --> Sleep : sleep
    Sleep --> On : wake up
    Sleep --> Off : turn off
{{< /mermaid >}}

-----

### 6\. ユーザー旅程図 (User Journey Diagram)

```mermaid
journey
    title My working day
    section Go to work
      Make tea: 5: Me
      Go upstairs: 3: Me
      Do work: 1: Me, Cat
    section Go home
      Go downstairs: 5: Me
      Sit down: 5: Me
```

{{< mermaid >}}
journey
    title My working day
    section Go to work
      Make tea: 5: Me
      Go upstairs: 3: Me
      Do work: 1: Me, Cat
    section Go home
      Go downstairs: 5: Me
      Sit down: 5: Me
{{< /mermaid >}}

-----

### 7\. エンティティ関係図 (ER Diagram)

```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE-ITEM : contains
    PRODUCT }|--o{ LINE-ITEM : includes
    CUSTOMER }|..|{ ADDRESS : lives in
```

{{< mermaid >}}
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE-ITEM : contains
    PRODUCT }|--o{ LINE-ITEM : includes
    CUSTOMER }|..|{ ADDRESS : lives in
{{< /mermaid >}}

### 8\. Git Graph

```mermaid
gitGraph:
    commit "Ashish"
    branch newbranch
    checkout newbranch
    commit id:"1111"
    commit tag:"test"
    checkout main
    commit type: HIGHLIGHT
    commit
    merge newbranch
    commit
    branch b2
    commit
```

{{< mermaid >}}
gitGraph:
    commit "Ashish"
    branch newbranch
    checkout newbranch
    commit id:"1111"
    commit tag:"test"
    checkout main
    commit type: HIGHLIGHT
    commit
    merge newbranch
    commit
    branch b2
    commit
{{< /mermaid >}}

### 9\. Mind Map

```mermaid
mindmap
  root((mindmap))
    Origins
      Long history
      ::icon(fa fa-book)
      Popularisation
        British popular psychology author Tony Buzan
    Research
      On effectiveness<br/>and features
      On Automatic creation
        Uses
            Creative techniques
            Strategic planning
            Argument mapping
    Tools
      Pen and paper
      Mermaid
```

{{< mermaid >}}
mindmap
  root((mindmap))
    Origins
      Long history
      Popularisation
        British popular psychology author Tony Buzan
    Research
      On effectiveness<br/>and features
      On Automatic creation
        Uses
            Creative techniques
            Strategic planning
            Argument mapping
    Tools
      Pen and paper
      Mermaid
{{< /mermaid >}}
