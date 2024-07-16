---
description: 모델의 입력으로 사용됨
---

# Prompt

Class hierarchy

{% code fullWidth="true" %}
```
BasePromptTemplate --> PipelinePromptTemplate
                       StringPromptTemplate --> PromptTemplate
                                                FewShotPromptTemplate
                                                FewShotPromptWithTemplates
                       BaseChatPromptTemplate --> AutoGPTPrompt
                                                  ChatPromptTemplate --> AgentScratchPadChatPromptTemplate



BaseMessagePromptTemplate --> MessagesPlaceholder
                              BaseStringMessagePromptTemplate --> ChatMessagePromptTemplate
                                                                  HumanMessagePromptTemplate
                                                                  AIMessagePromptTemplate
                                                                  SystemMessagePromptTemplate
```
{% endcode %}
