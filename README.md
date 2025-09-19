# Tech-Quiz-Generator
This a Test Generator Quiz for My SPPU Exams
# 📘 SPPU Exam Quiz Generator  

This project generates **multiple-choice quizzes (MCQs)** from **SPPU exam content** (notes, unit-wise question banks, or textbooks) using a **no-code/low-code GenAI pipeline in LangFlow**.  
The quizzes help students revise concepts quickly in an **interactive, exam-oriented** way.  

---

## ✨ Key Features  
- 📚 **Syllabus-driven quizzes** – MCQs generated from **SPPU subjects** like Cloud Computing, AI, Web Tech, etc.  
- 🔄 **Unit-wise selection** – Generate quizzes for any Unit (I–VI).  
- ⚙️ **Configurable difficulty** – Choose number of questions & difficulty level.  
- 🎯 **Exam-oriented** – Matches **SPPU question patterns**.  
- 🔄 **Extendable** – Can adapt to any topic or university content.  

---

## 🛠️ Architecture  

```mermaid
flowchart TD
    A[SPPU Content (PDF/Notes/Questions)] -->|Upload| B[Astra DB]
    B --> C[LangFlow Pipeline]
    C --> D[LLM Quiz Generator]
    D --> E[Generated MCQs]
    E --> F[Student/Exam Prep App]

👉 For details of the project, go here → [docs/project_details.md](docs/project_details.md)
