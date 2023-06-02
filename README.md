[![lint](https://github.com/hwchase17/langchain/actions/workflows/lint.yml/badge.svg)](https://github.com/hwchase17/langchain/actions/workflows/lint.yml)
[![test](https://github.com/hwchase17/langchain/actions/workflows/test.yml/badge.svg)](https://github.com/hwchase17/langchain/actions/workflows/test.yml)
[![linkcheck](https://github.com/hwchase17/langchain/actions/workflows/linkcheck.yml/badge.svg)](https://github.com/hwchase17/langchain/actions/workflows/linkcheck.yml)
[![Downloads](https://static.pepy.tech/badge/langchain/month)](https://pepy.tech/project/langchain)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langchainai.svg?style=social&label=Follow%20%40LangChainAI)](https://twitter.com/langchainai)
[![](https://dcbadge.vercel.app/api/server/6adMQxSpJS?compact=true&style=flat)](https://discord.gg/6adMQxSpJS)
[![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/hwchase17/langchain)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/hwchase17/langchain)
[![GitHub star chart](https://img.shields.io/github/stars/hwchase17/langchain?style=social)](https://star-history.com/#hwchase17/langchain)
# 😊🔗 LangChain-agent （Courses and Applications）

⚡ Repository focus on course and application for agent of Langchain. ⚡

**📺📽️ Video and Colab**
- [LangChain Agents - Joining Tools and Chains with Decisions](https://www.youtube.com/watch?v=ziu87EXZVUE)
- [Relative Colab](https://drp.li/FmrPY) 
- [Building Custom Tools and Agents with LangChain (gpt-3.5-turbo)](https://www.bilibili.com/video/BV1DM4y1b7Hx/?spm_id_from=333.337.search-card.all.click&vd_source=f1822dbf53f171fdcf40ee09e9f405c1)
- [Relative Colab](https://colab.research.google.com/drive/1FYsa3x3PzziL57EHEIuIqa5rkCAxCbin?usp=sharing) 
- [If you are a beginner of LangChain, you can watch this video.LangChain Explained in 13 Minutes | QuickStart Tutorial for Beginners](https://www.youtube.com/watch?v=aywZrzNaKjs)


**🤖 Agents**
- [Documentation](https://langchain.readthedocs.io/en/latest/modules/agents.html)
- End-to-end Example: [GPT+WolframAlpha](https://huggingface.co/spaces/JavaFXpert/Chat-GPT-LangChain)

Looking for the JS/TS version? Check out [LangChain.js](https://github.com/hwchase17/langchainjs).

**Production Support:** As you move your LangChains into production, we'd love to offer more comprehensive support.
Please fill out [this form](https://forms.gle/57d8AmXBYp8PP8tZA) and we'll set up a dedicated support Slack channel.

## Quick Install

`pip install langchain`
or
`conda install langchain -c conda-forge`

## 🤔 What is this?

The role of Agent in LangChain is to help solve feature problems, which include tasks such as numerical operations, web search, and terminal invocation that cannot be handled internally by the language model. To address these issues and facilitate communication with external applications, we introduce the concept of an Agent as a processor. The Agent can be considered a centralized manager responsible for task allocation and scheduling. If you want the large pre-trained language model to help you solve feature problems that involve non-text processing tasks such as numerical operations, web search, and terminal invocation (e.g. opening a terminal to check which folders and files are available), which cannot be handled internally by the language model, Agents are introduced. They act as processors to complete such tasks and act as a hub for integration and task allocation and scheduling.

Agent解决的问题，如果你希望大预言模型来帮助你解决特征问题，这个特征的问题里面包括一些非纯文字处理的问题，比如说数字运算，比如说网页搜索，比如说terminal的调用（我让它打开一个terminal看看哪个文件夹有哪个文件），这些涉及到非语言模型内部能处理的事情。需要和外部的应用做沟通、调用的时候，这个时候我们就引入了agent这样一个概念，让agent做为这样的一个处理者，来完成一些事情，这就是为什么Agent会被引入。可以看成一个管理的hub，一个集成器。给任务做分配，然后做调用。

This library aims to assist in the development of those types of applications. Common examples of these applications include:

**❓ Question Answering over specific documents**

- [Documentation](https://langchain.readthedocs.io/en/latest/use_cases/question_answering.html)
- End-to-end Example: [Question Answering over Notion Database](https://github.com/hwchase17/notion-qa)

**💬 Chatbots**

- [Documentation](https://langchain.readthedocs.io/en/latest/use_cases/chatbots.html)
- End-to-end Example: [Chat-LangChain](https://github.com/hwchase17/chat-langchain)

**🤖 Agents**

- [Documentation](https://langchain.readthedocs.io/en/latest/modules/agents.html)
- End-to-end Example: [GPT+WolframAlpha](https://huggingface.co/spaces/JavaFXpert/Chat-GPT-LangChain)

## 📖 Documentation

Please see [here](https://langchain.readthedocs.io/en/latest/?) for full documentation on:

- Getting started (installation, setting up the environment, simple examples)
- How-To examples (demos, integrations, helper functions)
- Reference (full API docs)
- Resources (high-level explanation of core concepts)

## 🚀 What can this help with?

There are six main areas that LangChain is designed to help with.
These are, in increasing order of complexity:

**📃 LLMs and Prompts:**

This includes prompt management, prompt optimization, a generic interface for all LLMs, and common utilities for working with LLMs.

**🔗 Chains:**

Chains go beyond a single LLM call and involve sequences of calls (whether to an LLM or a different utility). LangChain provides a standard interface for chains, lots of integrations with other tools, and end-to-end chains for common applications.

**📚 Data Augmented Generation:**

Data Augmented Generation involves specific types of chains that first interact with an external data source to fetch data for use in the generation step. Examples include summarization of long pieces of text and question/answering over specific data sources.

**🤖 Agents:**

Agents involve an LLM making decisions about which Actions to take, taking that Action, seeing an Observation, and repeating that until done. LangChain provides a standard interface for agents, a selection of agents to choose from, and examples of end-to-end agents.

**🧠 Memory:**

Memory refers to persisting state between calls of a chain/agent. LangChain provides a standard interface for memory, a collection of memory implementations, and examples of chains/agents that use memory.

**🧐 Evaluation:**

[BETA] Generative models are notoriously hard to evaluate with traditional metrics. One new way of evaluating them is using language models themselves to do the evaluation. LangChain provides some prompts/chains for assisting in this.

For more information on these concepts, please see our [full documentation](https://langchain.readthedocs.io/en/latest/).

## 💁 Contributing

As an open-source project in a rapidly developing field, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.

For detailed information on how to contribute, see [here](.github/CONTRIBUTING.md).
