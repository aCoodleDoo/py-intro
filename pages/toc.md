---
transition: slide-up
layout: two-cols
layoutClass: gap-16
---

# Domain Model

<div class="mermaid-container">
  
```mermaid {scale: 0.5}
erDiagram

    COMPANIES {
        uuid company_id PK
        string company_name
    }

    PROPERTIES {
        uuid property_id PK
        uuid company_id FK
        string property_name
    }

    USERS {
        uuid user_id PK
        string first_name
        string last_name
        string role
        uuid company_id FK
    }

    WORK_ORDERS {
        uuid work_order_id PK
        uuid unit_id FK
        string description
        uuid submitted_by FK
        uuid assigned_to FK
    }


    COMPANIES ||--|{ PROPERTIES : "has"
    COMPANIES ||--|{ USERS : "has"
    PROPERTIES }o--|| USERS : "is tenanted by"
    PROPERTIES ||--|{ WORK_ORDERS : "has"
    WORK_ORDERS }o--|| USERS : "submitted by"
    WORK_ORDERS }o--|| USERS : "assigned to"
    WORK_ORDERS }o--|| USERS : "triaged by"
```

</div>

<style scoped>
.mermaid-container {
display: flex;
justify-content: center;
align-items: flex-start;
width: 100%;
height: 85%;
padding: 20px;
border: 1px solid #ddd;
border-radius: 8px;
background-color: #f9f9f9;
box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}
</style>

::right::

## Table of Contents

<Toc text-sm minDepth="1" maxDepth="2" />

<style>
h2 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg,rgb(78, 212, 94) 10%,rgb(20, 140, 88) 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
The focus is on the interactions between users and tickets.

We are re-imagining how users interact with tickets. Chat. 

The next-gen of apps are chat windows?!
-->
