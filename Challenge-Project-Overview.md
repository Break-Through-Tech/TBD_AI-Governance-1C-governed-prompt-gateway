---

> ## Challenge Advisor: Update & Finalize Your Project Overview
>
> > 💡 **These grey text instructions are just for you, the team's Challenge Advisor; please delete them once you have completed the steps below.**
>
> We've pre-populated this Challenge Project Overview page — which is what will be shared with your Break Through Tech student team in August — using the details from your submission form. You should have received an email inviting you to join this repo as a Collaborator, enabling you to add files and make edits.
> 
> In order for your project to be finalized and assigned to a team, please:
> 1. **Review all sections below** and update or expand any content as needed, making sure to address the SME Feedback in the section immediately below. Look for square brackets to find the places below that require additional inputs from you (e.g., "About [Company / Org Name]").
> 2. **Add your dataset** to the [data folder](data) in this repo.
> 3. **Close the Issue assigned to you in this repo** to let us know that you have made your edits and the overview page is ready for final review. You can do this by going to the _Issues_ tab in the top left section of the menu above, add a comment that says "CA review complete", and click the button to Close the Issue. 
>
> If you're unfamiliar with how to edit a page like this in GitHub, check out [this tutorial](https://ubc-lib-geo.github.io/gis-workshop-waml-template/content/handson/edit-readme.html) for a quick overview (start with step 2 and only edit this page), and [this guide](https://ubc-lib-geo.github.io/gis-workshop-waml-template/content/markdown.html) on how to use Markdown to compose text.
>
>
> ❌ Remember that this is a public repo. Do NOT include: Proprietary data, PII, API keys, credentials, or anything confidential.

---

## 📋 BTT Internal Evaluation Notes
*(This section is for BTT staff and CAs only — remove before sharing with students)*

### Technical Vetting
| Check | Status | Notes |
| :--- | :--- | :--- |
| Python Compatibility | 🟢 | Project utilizes standard Python NLP libraries (HuggingFace, Scikit-learn, Pandas). No exotic frameworks requested. |
| Data Readiness | 🟡 | Data sources are clean but disparate across multiple repositories. Students will need to normalize heterogeneous schemas from LMSYS and JailbreakBench. |
| Resource Check | 🟡 | Potential risk if students attempt to use local LLMs for inference; project must enforce API-call-only or lightweight local embedding models to fit Colab memory constraints. |

### Internal Scores
- **Student Fit Score:** 6.5/10
- **Technical Depth Score:** 8/10
- **Overall Recommendation:** REVISE

### Advisor Feedback Draft
This project offers a compelling real-world application of AI governance. To succeed, first, pivot the focus from a 'Gateway' infrastructure (which risks becoming a DevOps exercise) to an 'Evaluation Pipeline' that labels and categorizes prompt safety. Second, strictly limit the model selection to a maximum of two endpoints to prevent excessive boilerplate code. Please submit a refined data pipeline schema by EOW to finalize the scope.

---

# Governed Prompt Gateway: Token Efficient and safety aware LLM routing for regulated customer

**Company / Org:** Other  
**Challenge Advisor:** Bhavana Unnam, [Email address]    
**Program:** Break Through Tech AI Studio - Fall 2026  

---

## 🏢 About Other
Other operates within the specialized domain of enterprise AI governance, focusing on the secure and cost-efficient deployment of generative models in high-stakes industries. The team is dedicated to building robust frameworks that bridge the gap between experimental AI capabilities and the rigorous compliance standards required by regulated customer service environments.

---

## 🎯 The Challenge
### Project Summary
This team will develop a governed prompt gateway that intercepts user queries to perform real-time safety screening, prompt optimization, and intelligent model routing. By utilizing public insurance and customer service datasets, the project applies NLP classification and RAG techniques to ensure high-reliability outputs while significantly reducing token consumption. The final solution provides a scalable, auditable layer that optimizes LLM spend and minimizes hallucination risks for enterprise-grade applications.

### Success Criteria
Safety and governance accuracy (80%+ F1 score on prompt-risk classification), Token reduction and cost efficiency (30–50% reduction in input tokens), Cache effectiveness (measured by cache-hit rate)

### Project Milestones
Use these milestones to guide your work. Your team will create a GitHub Projects board to track tasks within each milestone.
| Month | Milestone | Key Activities |
|-------|-----------|----------------|
| **September** | Data Exploration & Preprocessing | Standardize schemas across LMSYS and JailbreakBench datasets; perform initial EDA to identify prompt toxicity patterns and insurance-specific query distributions. |
| **October** | Feature Engineering & Baseline Modeling | Implement semantic similarity and prompt classification modules; develop a caching prototype to store and reuse common query responses. |
| **November** | Model Optimization & Evaluation | Execute iterative hyperparameter tuning on the classification layer; validate routing efficiency against the 80% F1 target using held-out test prompts. |
| **December** | Insights, Deliverables & Presentation | Finalize the evaluation dashboard and project documentation; prepare architecture diagrams and a comprehensive demo script demonstrating cost and safety metrics. |

> **Note for the team:** Please create a GitHub Projects board in this repository to break these milestones into weekly tasks. Go to the **Projects** tab → **New project** → Choose **Board** → Add columns for each month.

---

## 📊 Dataset
**Name and Source:** [LMSYS Toxic Chat](https://huggingface.co/datasets/lmsys/toxic-chat), [JailbreakBench](https://huggingface.co/datasets/JailbreakBench/JBB-Behaviors)  
**Format:** CSV/TSV  
**Size:** under 1gb  
**Location:** Hosted on HuggingFace Datasets  

### Key Details
- Publicly available customer-service, insurance question answering, toxic prompt, jailbreak, and hallucination datasets.
- Preprocessing must address the heterogeneity of inputs; normalization of schema formats is required to create a unified training set for the governance classifier.

---

## 🛠️ Suggested Approach
**ML Problem Type:** NLP & RAG  
**Recommended Libraries:**
- Scikit-learn, Transformers (HuggingFace), Pandas, Sentence-Transformers, LangChain
**Evaluation Metrics:** F1-Score for safety classification, Token throughput, Cache-hit percentage, Cost-per-request ratio

---

## 📚 Resources to Get Started
The following resources will help your team understand the problem space and potential technical approaches for this project:
**Background Reading:**
- [OWASP Top 10 for LLMs](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
**Technical Tutorials:**
- [HuggingFace NLP Course](https://huggingface.co/learn/nlp-course/)
**Code Examples:**
- [LangChain Prompt Engineering & Routing Documentation](https://python.langchain.com/)

---

## 🤝 How We'll Work Together
**Check-ins:** During our biweekly 60-min AI Studio Lab Section meeting block (2nd and 4th week of every month)  
**Communication:** Slack and GitHub Issues/Discussions  
**Response time:** 24-48 business hours  
**Recommended Tools:**
- **Coding:** Google Colab Free Tier  
- **Collaboration:** GitHub, Notion  
- **Virtual Meetings:** Zoom, Google Meet  

---

## 🚀 Getting Started
1. **Review this overview document** and note any questions for our first meeting.
2. **Begin reviewing the dataset** using the link provided in the Dataset section.
3. **Read the GitHub Projects documentation** [here](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects).

I'm excited to work with you!

---

## ❓ Questions?
Please bring any questions to our first meeting during the week of August 24th (Break Through Tech's Bridge to Studio - Session B).
