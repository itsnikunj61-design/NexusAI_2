# Class Diagram (textual UML)

```text
<<interface>> AIService
        ^
        |
OpenAICompatibleService

Main --> ChatController --> AIService
                     |
                     v
               ChatRepository --> DatabaseManager
                     |
             +-------+-------+
             v               v
       Conversation        Message

ChatWindow --> ChatController
```
