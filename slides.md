---
marp: true
paginate: true
headingDivider: 1
style: |
  section.grid th {
    font-weight: normal;
    text-align: left;
  }
  section.center-headings h1,
  section.center-headings h2 {
      text-align: center;
  }
  section.center p {
    text-align: center;
  }
  table {
    margin: 0 auto;
    width: max-content;
  }
  th {
      background-color: #f6f8fa;
  }
  section.heading-top h1, section.heading-top h2 {
    position: absolute;
    top: 50px;
  }
---

# :gem: Serverless

#### L'écosystème serverless (20 minutes)
- Cloud
- Open Source
- Framework
#### Les pratiques et paradigmes associés
#### Avantages / Inconvénients
#### Azure Function (40 minutes)

# Stateless
<!-- _class: center-headings -->

# :snowflake: / :fire: Start
<!-- _class: center-headings -->

# API Gateway
<!-- _class: center-headings -->

# :tomato: Lambda Specs​ 1/2

|Runtime|Versions|
|:---:|:---:|
| Node.js | 12.13.0, 10.16.3, and 8.10|
|Java     |11 and 8|
|Python|3.8, 3.7, 3.6, and 2.7|
|.NET Core| 2.1|
|Go| 1.x|
|Ruby| 2.5|
|Rust| n/a |

# :tomato: Lambda Specs​ 2/2

|Key|Value|
|:---:|:---:|
|AMI| 64-bit Amazon Linux|
|Memory| 128MB - 3008MB, in 64 MB increments​|
|Ephemeral disk space| 512MB​|
|Max execution duration| 900 seconds​|
|Compressed package size| 50MB​|
|Uncompressed package size| 250MB|​

# Azure Functions
<!-- _class: center-headings -->
![bg width:800px opacity:.2](./images/azure-function.png)

# Langages supportés
<!-- _class: grid center-headings -->
![bg width:800px opacity:.2](./images/azure-function.png)

| Language | Versions |
|---|---|
| JS / TS | 	Node 10 & 12|
| F# |	.NET Core 3.1|
| Java |	Java 8|
| PowerShell | 	PowerShell Core 6 |
| Python | 3.6 & 3.7|


# Déclencheurs et liaisons 
(passer rapidement au code)
<!-- _class: grid center-headings center -->
![bg width:800px opacity:.2](./images/azure-function.png)

| Blob storage | Queue | Azure Cosmos DB |
| --- | --- | --- |
| Event Grid | Event Hubs | IoT Hub |
| HTTP and webhooks | Microsoft Graph | Mobile Apps |
| Notification Hubs | Queue Storage | SendGrid |
| Service Bus | SignalR Service | Table storage |
| Timer | Twilio | |


# Application Patterns
<!-- _class: center-headings -->
![bg width:800px opacity:.2](./images/azure-function.png)

#
<!-- class: center -->
## Pattern #1: Function Chaining

![function chaining](./images/function-chaining.png)

## Pattern #2: Fan out/fan in

![fan](./images/fan-out-fan-in.png)

#
## Pattern #3: Async HTTP APIs

![async http](./images/async-http-api.png)

#
## Pattern #4: Monitor

![monitor](./images/monitor.png)

#
## Pattern #5: Human interaction
![approval](./images/approval.png)


## Pattern #6: Aggregator (stateful entities)
![aggregator](./images/aggregator.png)