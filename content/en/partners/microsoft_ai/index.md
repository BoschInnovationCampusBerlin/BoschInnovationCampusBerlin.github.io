---
title: ""
description: ""
date: 2023-08-23T13:52:06+02:00
lastmod: 2023-08-23T13:52:06+02:00
draft: false
images: []
resources:
- name: "logo"
  src: "microsoft_ai.png"
---

# Microsoft Agentic AI
## Technology Stack

Microsoft’s Agentic AI technology stack is a comprehensive framework for building intelligent AI agents—autonomous software entities that can perceive, reason, and act to perform tasks with minimal human intervention. This stack integrates advanced AI models, orchestration frameworks, development tools, and governance mechanisms to enable these agents to work collaboratively and securely across applications and services. 

| End User | Maker | Pro Developer |
|:---------|:------|:--------------|
|<img src="https://www.microsoft.com/en-us/microsoft-365/blog/wp-content/uploads/sites/2/2025/05/copilot-logo-2-1.png" width="100" alt="Copilot">|<img src="https://adoption.microsoft.com/wp-content/uploads/2024/03/icon-copilot-studio.png" width="100" alt="Copilot Studio">|<img src="https://devblogs.microsoft.com/foundry/wp-content/uploads/sites/89/2025/03/ai-foundry.png" width="100" alt="Azure AI Foundry">|
|**Copilot**|**Copilot Studio**|**Azure AI Foundry**|
|No Code|Low Code|Pro Code|



## Architecture and Key Components of the Agentic AI Stack

Microsoft’s Agentic AI stack can be understood as a layered architecture, with each layer providing specific capabilities to the AI agents. From the bottom (infrastructure and models) to the top (application and interface), the stack includes:

![Azure AI Foundry](https://miro.medium.com/v2/resize:fit:1196/0*S06XajS89tOxiZv8.jpg)

* **Foundation Models and Cognitive Services:** At the base are advanced AI models and services that provide the “brains” for agents. This includes the Azure OpenAI Service (offering large language models like GPT-4, Llama, Claude and thousands others for natural language understanding and generation) and Azure AI Services for specialized AI tasks (vision, speech, language, decision). These services provide core capabilities such as text generation, image analysis, document intelligence and more. Together, they equip agents with reasoning, language understanding, and perception skills. 
See [Azure Model Catalog](https://ai.azure.com/explore/models) and [Azure AI Foundry Documentation](https://learn.microsoft.com/en-us/azure/ai-foundry/) for details

* **Knowledge Integration:** Azure provides retrieval systems and memory stores that provide agents with long-term knowledge and context (enterprise data, documents, web content). It enables implementation of Retrieval-Augmented Generation (RAG) systems via Azure Cognitive Search, Vector DBs and others.
Find an example here [How to build a RAG solution using Azure AI Search](https://learn.microsoft.com/en-us/azure/search/tutorial-rag-build-solution)
* **Azure AI Foundry (Cloud Agent Platform):** Azure AI Foundry is Microsoft’s unified cloud platform for designing, customizing, and managing AI applications and agents2. It acts as an enterprise-grade hub for agentic AI with several subcomponents:
  * **Model Hub:** Foundry provides access to a broad catalog of AI models. It hosts thousands of foundation models (both partner-hosted and Microsoft-hosted) including third-party models, all available for developers to use or fine-tune within a governed environment. Tools like a Model Leaderboard (to rank top-performing models by task) and a Model Router (to automatically select the optimal model for a given query in real-time) help developers evaluate and utilize models efficiently.
  * **Agent Service:** The Azure AI Foundry Agent Service enables orchestration of complex, multi-agent workflows – meaning developers can deploy multiple specialized agents that collaborate to handle different subtasks of a larger process. This service supports open interaction protocols like *Agent-to-Agent (A2A)* communication and the *Model Context Protocol (MCP)* for interoperability, allowing agents to coordinate with each other and with external systems in a standardized way. 
  For an example to build an agent see here: [Quickstart: Create a new agent](https://learn.microsoft.com/en-us/azure/ai-services/agents/quickstart?pivots=ai-foundry-portal)
  * **Agent Orchestration with Semantic Kernel:** A distinctive element of agentic systems is the ability to break down complex tasks, formulate plans, and coordinate multiple agents or skills. Semantic Kernel is an open-source SDK that enables developers to design complex prompt flows, planners, and skill plugins for AI, supporting integration of memory and tools.
  To learn how to use Semantic Kernel, start here [Getting started with Semantic Kernel](https://learn.microsoft.com/en-us/semantic-kernel/get-started/quick-start-guide?pivots=programming-language-csharp)
* **Developer Tooling:** Microsoft’s developer and productivity platforms are deeply integrated into the agentic AI stack, providing pro code and low code tooling to create and deploy agents:
    * **Visual Studio Code and GitHub Copilot:** Visual Studio Code, enhanced by the Azure AI Foundry extension, provides a powerful, developer-friendly environment for building intelligent agents. It bridges the gap between code and cloud, enabling developers to rapidly prototype and deploy agents and integrate with DevOps pipelines for scalable, production-grade AI solutions. GitHub Copilot can autonomously perform development tasks like refactoring code, generating tests, or even proposing new functions. 
    Download and get information about Visual Studio Code from [Visual Studio Code Home](https://code.visualstudio.com/)  
    * **Copilot & Copilot Studio:** – For business and end-user scenarios, Microsoft Copilot provides an environment to build business process agents that operate within the Microsoft 365 ecosystem. Copilot Studio includes an Agent Builder that allows “makers” to create custom agents using low-code tools. It is also possible to integrate agents from Azure AI Foundry. 
    Access the development environment via [Copilot Studio Home](https://copilotstudio.microsoft.com/)
* **Observability and Management:** To support enterprise deployments, Azure AI Foundry includes built-in observability features for monitoring agent behavior and performance.
* **Security and Identity:** Azure AI Foundry is integrated with enterprise security frameworks. Microsoft Entra Agent ID assigns unique identities to each agent created in Azure AI Foundry or in Copilot, enabling tight access control and lifecycle management of agents as first-class entities.
More details via [Microsoft Entra Agent ID](https://techcommunity.microsoft.com/blog/microsoft-entra-blog/announcing-microsoft-entra-agent-id-secure-and-manage-your-ai-agents/3827392)

## Open Agentic Interoperability 
Microsoft is pushing for an open ecosystem for AI agents, so components of its stack support emerging standards that enable interoperability across platforms and organizations:
* **Model Context Protocol (MCP):** MCP is an open protocol intended to allow different agent platforms and language models to communicate with each other in a secure, standardized way. Microsoft prvides  first-party support for MCP across its major agent-building platforms – including GitHub, Copilot Studio, Azure AI Foundry, Semantic Kernel, Dynamics 365, and even Windows – ensuring agents built with Microsoft tech can interface with other MCP-compliant agents or tools.
To get started have a look here [MCP Curriculum for Beginners](https://github.com/microsoft/mcp-for-beginners)
* **Agent-to-Agent (A2A) Protocol:** This communication mechanism allows agents to talk directly to each other peer-to-peer. Microsoft has built A2A support into Azure AI Foundry and also into collaboration platforms like Teams. The A2A protocol facilitates secure message exchange between agents, including passing of data or credentials.
See more details here [Empowering multi-agent apps with the open Agent2Agent (A2A) protocol](https://www.microsoft.com/en-us/microsoft-cloud/blog/2025/05/07/empowering-multi-agent-apps-with-the-open-agent2agent-a2a-protocol/)

## Additional tooling
A lot of additional tooling is available to enable quick application development. Some of this components are:
* **Agent flows**: Agent flows are a powerful way to automate repetitive tasks and integrate your apps and services. Agent flows can be triggered manually, by other automated events or agents, or based on a schedule. Agent flows are deterministic—they execute actions or tasks following a rule-based path.
* **Compute Use**: Computer use is a tool in Copilot Studio that lets your agent interact with any system that has a graphical user interface. It works with websites and desktop apps by selecting buttons, choosing menus, and entering text into fields on the screen. 
* **Agent Playground**: AI Foundry and Copilot Studio provide an agent playground to test your agents. You can observe how your model responds with your data. 

The Microsoft team onsite is available to help you to configure your environment and to start the development of your agents. Please get in contact with
* Ricardo Niepel
* Pooja Bhatia
* Thomas Titze

Have a question about Microsoft AI solutions? Try the AI-powered assistant at [Microsoft AI Home](https://www.microsoft.com/en-us/ai/)