<link href="./style.css" rel="stylesheet"></link>

<span style="font-size: 30px;">Sample API</sapn>

- [1. API概要](#1-api概要)
- [2.API仕様](#2api仕様)
  - [2.1. 処理シーケンス](#21-処理シーケンス)

# 1. API概要
 Sample words for API testing title.

# 2.API仕様
 Sample API仕様<br>
 testing testing testing testing

## 2.1. 処理シーケンス

```mermaid
sequenceDiagram
participant app as sample app
participant frontapi as frontapi
participant backendapi as backendapi

  app->>+frontapi: sample API
  note left of frontapi: something
  
  backendapi->>backendapi: 【Common】User authentication
  backendapi-->>frontapi: Authentication Error

  frontapi->>+backendapi: Sample App
  note left of backendapi: sample no
  backendapi->>frontapi: Error Response
  frontapi->>app: Error Result Response
  note left of frontapi: code<br/>message
  backendapi->>-frontapi: Processing result response
  frontapi->>-app: Processing result response
  note left of frontapi: resultSet
```

<br>