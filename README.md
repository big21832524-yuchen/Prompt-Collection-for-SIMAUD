# Prompt Engineering for Building Energy Rating (SAP 10.2)

This repository contains the prompts and reference materials used in the research paper:

The study evaluates the effectiveness of different prompt engineering strategies in performing building energy calculations based on the UK Government's Standard Assessment Procedure (SAP 10.2).

## 📁 Repository Structure
- `/prompts`: Contains four levels of prompt designs (Baseline to CoT).
- `/docs`: Reference documents and calculation standards.
- `building_data.md`: Detailed geometry and opening information of the test building.

## 🔬 Prompt Strategies
We compared four prompting strategies to evaluate LLM performance:

| ID | Strategy | Description | Link |
| :--- | :--- | :--- | :--- |
| **A** | **Baseline** | Direct instruction to calculate TER without specific constraints. | [View](./prompt-A-ZeroShot.md) |
| **B** | **Doc-Grounded** | Grounding the model using the SAP 10.2 PDF as the sole knowledge source. | [View](./prompt_b_doc_grounded.md) |
| **C** | **Step-Augmented** | Guiding the model through 15 specific calculation steps. | [View](./prompt_c_step_augmented.md) |
| **D** | **Chain-of-Thought** | Forcing sequential reasoning and outputting intermediate values. | [View](./prompt_d_cot.md) |

## 📄 Reference Document
The calculations are based on the following official standard included in this repo:
* **SAP 10.2 (Version 14-03-2025)**: [SAP_10_2_14-03-2025.pdf](./docs/SAP_10_2_14-03-2025.pdf)

## 🛠️ Experimental Setup
- **Model:** GPT-4o / GPT-o3 /GPT-4.5
- **Parameters:** Temperature 0.7, Top P 1.0
