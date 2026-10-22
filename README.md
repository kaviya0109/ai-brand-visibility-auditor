# AI Brand Visibility Auditor

**A multi-stage AI agent workflow built with n8n and Google Gemini to analyse brand mentions in AI-generated answers.**

> **Project status:** In Progress 🚧

## Overview

The Mini AI Brand Visibility Auditor is an AI workflow prototype designed to analyse how brands are represented in a collection of AI-generated answers.

It processes sample answers through three sequential AI stages: brand research, visibility analysis, and verification and reporting. The goal is to identify brand mentions, competitor references, potential visibility gaps, and evidence-based recommendations.

This project explores how AI agents and workflow automation can support brand research and product decision-making.

## Problem Statement

Brands need to understand whether they appear in relevant AI-generated answers and how they are represented compared with competitors.

Manually reviewing multiple answers can be time-consuming. This prototype explores a structured workflow to organise findings, identify gaps, and generate a concise audit report.

## Solution

The workflow uses three connected AI stages:

### 1. Brand Research Agent

- Analyses supplied AI-generated answer samples.
- Identifies brand mentions and missing mentions.
- Extracts competitor references and supporting evidence.

### 2. Visibility Analysis Agent

- Reviews the research findings.
- Identifies potential visibility gaps within the supplied sample.
- Generates practical recommendations for further investigation.

### 3. Verification and Reporting Agent

- Reviews the previous agent's analysis.
- Separates observed findings from assumptions and recommendations.
- Highlights limitations and unsupported conclusions.
- Produces a structured brand visibility audit report.

## Workflow Architecture

```text
Manual Trigger
      |
      v
   Edit Fields
      |
      v
Brand Research Agent
      |
      v
Visibility Analysis Agent
      |
      v
Verification & Reporting Agent
      |
      v
Final Audit Report
```

## Tech Stack

- **Workflow Automation:** n8n
- **Language Model:** Google Gemini
- **AI Techniques:** Prompt engineering, sequential AI agent workflows, evidence-based analysis
- **Evaluation:** Manual test cases and output verification

## Current Prototype

The initial test uses a fictional brand, **Zyra Shoes**, and two fictional sample answers.

The test explores whether the workflow can identify:
- Brand mentions and missing mentions.
- Competitor references.
- Potential category-level visibility gaps.
- Recommendations and limitations supported by the supplied findings.

The workflow successfully generated a structured analysis and final report during the initial test.

**Important:** These results demonstrate workflow functionality only. Two fictional answers are not sufficient to measure real-world brand visibility or establish market trends.

## Evaluation Plan

The next development phase will focus on:

- Expanding the test dataset across multiple fictional brands and question categories.
- Creating expected outputs for each test case.
- Checking brand-mention detection and competitor extraction against expected results.
- Identifying unsupported claims and incorrect recommendations.
- Comparing AI-generated findings with manually reviewed evidence.
- Documenting accuracy, failure cases, and limitations.

## Current Limitations

- Uses manually supplied sample answers rather than live AI search results.
- Has been tested initially on only two fictional answers.
- Recommendations require human review.
- Findings cannot be generalised to real-world search visibility.
- Live data collection, broader evaluation, and production deployment are not yet implemented.

## Future Enhancements

- Add a larger, labelled evaluation dataset.
- Integrate permitted data sources or APIs for collecting real AI-generated answers.
- Introduce structured output formats for consistent reporting.
- Add evaluation metrics for mention detection and unsupported claims.
- Generate downloadable audit reports.
- Explore a simple interface for entering brand names and reviewing results.

## What I Am Learning

Through this project, I am exploring:

- Designing AI-powered product workflows.
- Breaking a product problem into specialised AI stages.
- Writing and iterating on agent instructions.
- Evaluating LLM outputs against evidence.
- Identifying hallucinations, limitations, and reliability risks.
- Translating AI-generated findings into actionable product recommendations.

## Disclaimer

This is an independent learning and portfolio project. The initial test data is fictional, and the prototype does not currently monitor live AI search engines or provide validated real-world brand visibility measurements.

---

**Author:** Kaviya K

**Project Type:** Independent AI Product Prototype
