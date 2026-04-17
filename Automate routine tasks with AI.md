# Automate routine tasks with AI

## 🍳 Automation analogy: routine tasks as recipes
– **Making coffee** analogy maps to IT work: repeatable steps triggered by predictable events (e.g., waking up → start coffee; alerts/tickets → same remediation steps).
– Implication: repeatability and consistent triggers identify strong candidates for automation.
– Benefit: **saves time** and **frees staff** for higher-value work.

## 🤖 Role of generative AI in automation
– **Gen AI tools** can accept natural-language instructions and produce scripts or step-by-step automation without requiring the user to write code from scratch.
– Example tool referenced: **Gemini**, which can outline requirements, structure, enhancements, and considerations for a script.
– Advantage: tools often explain reasoning and cite sources, enabling better understanding and learning from the generated output.

Let's go through an example to bring this to life.

A machine has files that need to be backed up in case there's a drive failure or other issue, but manually backing them up takes a long time.

A gen AI tool like **Gemini** can help you automate this.

We can start by writing a prompt like this.

" I'm a Tech Support Specialist.
Help me identify key components of a script to automate data backup and recovery processes."

<img width="1237" height="460" alt="image" src="https://github.com/user-attachments/assets/38dbe83a-1ed8-46ea-8acb-5218fd02c2a0" />


Gemini gives us some general guidance on where to start with the script, including requirements, basic structure, enhancements, and important considerations.
<img width="1215" height="448" alt="image" src="https://github.com/user-attachments/assets/132f9113-f3cd-490a-ba4e-0aecafbb62b6" />
<img width="1213" height="401" alt="image" src="https://github.com/user-attachments/assets/452755aa-68c0-4d47-b4c2-1804519685a6" />
<img width="1213" height="397" alt="image" src="https://github.com/user-attachments/assets/d71ce87d-25ab-446b-893c-ecb56bec0524" />


## 🧭 Prompt framework and stages highlighted

– Reference to framework **T-C-R-E-I** with emphasis on **E = Evaluate** and **I = Iterate** as active steps in prompt development.

– Practical use: generate an initial script outline, then **evaluate** its alignment to needs and **iterate** prompts to refine behavior.

## 📝 Practical example: automating backups

– Use case: a machine with files that need backing up to protect against drive failure; manual backups are time-consuming.

– Workflow shown: prompt gen AI to **identify key components** of a backup-and-recovery script and produce working code or instructions.

– Concrete iteration: follow up by specifying environment details such as **Linux** and **back up home directory to a network share** to get tailored script output.

## 🛠️ Iteration techniques and prompt refinement

– If output mismatches expectations, add **specific guidance** and more contextual detail.

– Use **references/examples**: provide a sample of the expected format or analysis to steer the result.

– Improve phrasing: break instructions into **shorter sentences** to increase clarity.

– Provide feedback on liked/disliked elements: tell the model why some suggestions worked and others did not to shape subsequent outputs.

<img width="811" height="481" alt="image" src="https://github.com/user-attachments/assets/35fb4f5a-ea9d-40b6-821f-d6e2d7633ecf" />

## 🔎 Evaluation and testing requirements

– **Always test** AI-generated scripts first in a controlled environment; each deployment environment has unique differences.

– Expect to **adjust parts** of generated scripts for environment-specific commands, paths, permissions, or services.

– Scripts may contain **errors or bugs** despite AI generation; use a safe testing environment to mitigate risk.

## ⚠️ Limitations and cautionary notes

– Not everything should be automated; **repetitive tasks** are primary candidates, but consider complexity, risk, and exceptions.

– While AI can **reduce some syntax or command errors**, it is not infallible—validation and human oversight remain necessary.

– Environment variability and edge cases can cause generated automation to fail without tailoring.

## 🔁 Practical checklist for prompt-driven automation development

– Start with a clear role/context (e.g., **Tech Support Specialist**) and desired outcome.

– Request **requirements, basic structure, enhancements, and considerations** from the AI.

– Iterate by adding environment-specific constraints (OS, directories, network shares, permissions).

– Provide examples or expected output formats to improve alignment.

– Test in a sandbox, revise based on failures, and re-run iterations until stable.

## 📈 Operational implications for support teams

– Use automation to **streamline operations** and **deliver more consistent support experiences** by removing repetitive manual steps.

– Analyze common tickets and recurring issues to prioritize automation candidates.

– Start experimenting with small, low-risk automations and expand as confidence and test coverage grow.

