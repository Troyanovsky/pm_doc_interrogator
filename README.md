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

The MVP version uses routed OpenAI API, and the future version plans to use self-hosted Vicuna/ChatGLM.

The frontend will be built with HTML, Tailwind CSS, and Vue.

The backend will be hosted on Netlify. For future version, I plan to allow users to self-host or use API directly.

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