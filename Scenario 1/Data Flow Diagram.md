```mermaid

    erDiagram
    USER ||--o{ Patient : "Uses"
    CUSTOMER ||--o{ ORDER : "places"
    CUSTOMER ||--o{ INVOICE : "liable for"
    DELIVERY-ADDRESS ||--o{ ORDER : "receives"
    INVOICE ||--|{ ORDER : "covers"
    ORDER ||--|{ ORDER-ITEM : "includes"
    PRODUCT-CATEGORY ||--|{ PRODUCT : "contains"
    PRODUCT ||--o{ ORDER-ITEM : "ordered in"
