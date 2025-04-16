```mermaid
block-beta
    columns 2
    comp1{{"Computer 1"}}:2
    comp2{{"Computer 2"}}:1
    comp3{{"Computer 3"}}:0
    comp4{{"Computer 4"}}:1
    comp5{{"Computer 5"}}:4

    block:attackStages:3
        stage1(["New Informations Form"]) space:2 stage2
        stage2[("Database")] space:2 stage3
        stage3[/"Website Down"/]
    end

    comp1 -- "Submit" --> stage1
    comp2 -- "Submit" --> stage1
    comp3 -- "Submit" --> stage1
    comp4 -- "Submit" --> stage1
    comp5 -- "Submit" --> stage1

    stage1 -- "Large requests" --> stage2
    stage2 -- "Update overloads" --> stage3

    style comp1 fill:#87ceeb,stroke:#333333,stroke-width:.075rem
    style comp2 fill:#87ceeb,stroke:#333333,stroke-width:.075rem
    style comp3 fill:#87ceeb,stroke:#333333,stroke-width:.075rem
    style comp4 fill:#87ceeb,stroke:#333333,stroke-width:.075rem
    style comp5 fill:#87ceeb,stroke:#333333,stroke-width:.075rem

    style stage1 fill:#90ee90,stroke:#333333,stroke-width:.075rem
    style stage2 fill:#bbf,stroke:#333333,stroke-width:.075rem
    style stage3 fill:#ce2029,stroke:#333333,stroke-width:.075rem
```
