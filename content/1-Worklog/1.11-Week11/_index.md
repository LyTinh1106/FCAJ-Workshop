---
title: "Week 11 Worklog"
date: 2026-07-03
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Research and understand the Amazon Textract service for automated text extraction.
* Implement a solution using Amazon Textract to process and extract text content from PDF CV files.
* Integrate AI (LLM) to analyze and evaluate CV content based on job requirements.
* Finalize the worklog documentation and project progress reports.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | **Learn about Textract**<br>- Read technical documentation on Amazon Textract and APIs that support text extraction from scanned docs/images/PDFs<br>- Conduct experiment extractions on AWS Console to understand returned JSON structures (Blocks, Lines, Words). | 29/06/2026 | 29/06/2026 | |
| 2 | **Implement Textract to process content from PDF files**<br>- Develop a Lambda function using Boto3 SDK to call Amazon Textract on PDF files stored in S3<br>- Implement text parsing and aggregation algorithms to turn raw Textract JSON blocks into structured plain text<br>- Optimize asynchronous job handling for processing multi-page PDF documents. | 29/06/2026 | 30/06/2026 | |
| 4 | **Integrate AI for CV evaluation**<br>- Integrate AI services (Using Gemini 3.1 Flash) to analyze extracted text content from CVs<br>- Construct high-quality prompts comparing candidate skills in CVs against Job Descriptions<br>- Parse AI responses to extract compatibility scores and detailed feedback commentary. | 01/07/2026 | 02/07/2026 | |
| 5 | **Write worklog**<br>- Compile detailed progress reports and worklogs for Week 9 through Week 11<br>- Sync and verify page rendering on the Hugo local server to ensure markdown tables and layout display properly. | 02/07/2026 | 03/07/2026 | |


### Week 11 Achievements:

* **Text Extraction Research**: Mastered the core concepts and usage of Amazon Textract for document processing.
* **Document Extraction Workflow**: Successfully built a workflow to extract text from PDF CVs with high accuracy.
* **Artificial Intelligence Integration**: Integrated AI-powered CV evaluation to automatically assess candidate skills and job fit.
* **Documentation Finalization**: Completed and updated detailed worklogs for all project phases.
