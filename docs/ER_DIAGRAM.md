# ER Diagram (textual)

```text
CONVERSATIONS
-------------
id PK
title
created_at
      |
      | 1:N
      v
MESSAGES
--------
id PK
conversation_id FK
role
content
created_at
```
