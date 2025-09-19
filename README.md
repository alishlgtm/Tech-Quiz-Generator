# 📘 Project Details – SPPU Exam Quiz Generator  

This document provides an in-depth explanation of the **Tech-Quiz-Generator** project. It explains the workflow, setup, and customization options.  

---

## 🎯 Project Goal  

The goal of this project is to help students preparing for **SPPU exams** practice with **automatically generated MCQs** based on their syllabus, notes, and unit-wise question banks.  

It uses **LangFlow + Astra DB + LLMs** to create a **no-code/low-code quiz generator**.  

---

## 🔄 Workflow  

1. **Content Input**  
   - Users provide **SPPU notes, PDFs, or question banks**.  
   - The content is stored in **Astra DB** for easy retrieval.  

2. **Preprocessing**  
   - Text is **cleaned, chunked, and indexed**.  
   - Each chunk represents a topic/concept from the syllabus.  

3. **Quiz Generation Pipeline (LangFlow)**  
   - **LangFlow** connects Astra DB with an **LLM (OpenAI/Anthropic, etc.)**.  
   - The pipeline transforms syllabus text → into **exam-style MCQs**.  

4. **Output (MCQs)**  
   - Each MCQ has **4 options** with one correct answer.  
   - The quizzes are generated **unit-wise** or **subject-wise**.  

5. **Interactive Usage**  
   - Students can select number of questions.  
   - Quiz can be delivered via CLI, Web UI, or mobile integration.  

---

## 🛠️ Tech Stack  

- **LangFlow** → Workflow orchestration (no-code/low-code AI pipeline)  
- **Astra DB** → Cloud-native NoSQL database for storing syllabus & notes  
- **Python** → Preprocessing and integration scripts  
- **LLM** → Question generation engine (OpenAI GPT, Anthropic Claude, etc.)  

---

## 📂 Directory Structure  

```bash
Tech-Quiz-Generator/
│── docs/
│   └── project_details.md       # Detailed documentation
│── data/
│   └── sppu_notes/              # Raw notes & question banks
│── langflow_pipeline.json       # Exported LangFlow workflow
│── scripts/
│   └── preprocess.py            # Prepares text for database ingestion
│── README.md                    # Project overview
