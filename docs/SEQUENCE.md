# Sequence Diagram (textual UML)

```text
User -> ChatWindow: enter prompt
ChatWindow -> ChatController: ask(prompt, model)
ChatController -> AIService: generateResponse()
AIService -> API: HTTP request
API --> AIService: response
AIService --> ChatController: text
ChatController -> ChatRepository: save user/assistant messages
ChatController --> ChatWindow: response
ChatWindow --> User: display response
```
