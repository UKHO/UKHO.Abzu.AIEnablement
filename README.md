# UKHO.Abzu.AIEnablement

## Overview
This repository is a central hub for our work with **AI-assisted development**.  

It contains curated prompts, guidelines, and supporting documentation that help us leverage tools such as **GitHub Copilot** and emerging AI agents effectively in our coding practices.

The goal is to:
- Improve productivity by using high-quality prompts.
- Standardize approaches for AI-assisted development across the team.
- Share learnings, patterns, and practices that scale with future AI tooling.
- Provide a reference point for experimenting with agent-driven coding workflows.

## Writing New Prompts

Your AI is not a mind reader!

Treat the AI like a new colleague and if you expect it to work in a specific way you must include specific instructions in your prompt.

Consider the following best practices when writing prompts:

- Chain of Thought Reasoning: Prompt the AI "Before you respond to my query, walk me through your thought process step by step"

- Few-Shot Learning: Provide examples of the expected output format to help the AI understand your requirements. Tell the AI what good looks like and what bad looks like!

- Reverse Prompting: Prompt the AI to ask clarifying questions and iterate to build up a better understanding of the task.

- Assign a Role to the AI: Clearly define the role you want the AI to assume (e.g., "You are a senior software engineer..."). This narrows down the context and helps the AI generate more relevant responses.

---

## Repository Structure
- **.github/prompts**  
  Ready-to-use and reusable prompt files for GitHub Copilot or other AI tools.

- **/docs/plans**  
  Folder to output plans

- **/docs/specs/templates**  
  Folder for spec-template_v.md

- **.mcp.json**  
  Configuration file for Microsoft Copilot settings. This will either need to be within the Visual Studio Solution or copied to your users folder.

---

## Getting Started
1. Clone this repo:
   ```
   git clone https://github.com/CompanyName/CompanyName.TeamName.AIEnablement.git
