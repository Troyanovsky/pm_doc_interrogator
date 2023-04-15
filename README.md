# PM Doc Interrogator
A simple tool to help Product Managers check their documents & provide suggestions.

## Background
Product Managers often face the challenge of creating thorough and logical documents that can withstand scrutiny. It can take a lot of time for thorough investigations. Even with the help of AI like ChatGPT, writing prompts can be tedious, and learning how to write good prompts for interrogation is difficult.

## Target Users
This tool is targeted at Product Managers who want to ensure that their documents are thorough and logical.

## Solution
Our solution is a simple tool/interface to help PMs check their documents & provide suggestions. The tool will allow users to load a document and interrogate the document with many pre-set prompts.

## Differentiator
Our tool offers refined prompts for different scenarios and is specifically targeted at PM documents. It is easy to use and offers suggestions for improvement based on the content of the document.

## Technical Pipeline
The technical pipeline is designed as follows:

Document -> Prompt/Scenario -> LLM -> Return

The frontend will be built with HTML, Tailwind CSS, and Vue.

The first version will not have a backend, users wil send requests directly to OpenAI's API with their own API key in the browser. For future versions, I plan to spin up a proxy server and allow those without an API key to use the tool. I also plan to implement a custom LLM that users can run on their own computer for privacy. (If you are interested in contributing to this project, please reach out to me!)

## Features
The interface has four main features: Inspiration, Generate, Analyze, and Improve. The left side of the interface is an input text box, and the right side has buttons and a feedback box.

Inspiration
- Similar apps

Generate
- User stories generator
- Success criteria generator
- PRFAQ Generator

Analyze
- Missing components/sections
- Logical flaws Interrogator/consistency

Improve
- Refine language
- Ideate Future iterations/features

## TODO
- Enable streaming for responses
- Creat a proxy backend for users without API keys & users in locations blocked by OpenAI
- Add more pre-set prompts
- Allow customization of prompt buttons
- Add a custom, locally-run LLM (if possible) like Alpaca, Koala, GPT4All, etc.