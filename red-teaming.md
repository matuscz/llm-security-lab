### OWASP  top 10 for LLMs ([odkaz](https://genai.owasp.org/llm-top-10/))

Jejich seznam:
1. [Prompt Injection](./red-teaming#Prompt-Injection)
2. [Sensitive Information Disclosuren](./red-teaming#Sensitive-Information-Disclosure)
3. [Supply Chain](./red-teaming#Supply-Chain)
4. [Data and Model Poisoning](./red-teaming#Data-and-Model-Poisoning)
5. [Improper Output Handling](./red-teaming#Improper-Output-Handling)
6. [Excessive Agency](./red-teaming#Excessive-Agency)
7. [System Prompt Leakage](./red-teaming#System-Prompt-Leakage)
8. [Vector and Embedding Weaknesses](./red-teaming#Vector-and-Embedding-Weaknesses)
9. [Misinformation](./red-teaming#Misinformation)
10. [Unbounded Consumption](./red-teaming#Unbounded-Consumption)

#### [Prompt Injection](https://genai.owasp.org/llmrisk/llm01-prompt-injection/)
Pomocí promptů (a další médií včetné dokazů jiné stránky, obrázky atd) útočník zmanipuluje AI tak, aby dělala věci které má zakázany dělat.Prompt Injection se dělí na dva podruhy:
1. **Direct Prompt Injections** - útočník přímo napíše AI prompt, využívá k tomu jen text
2. **Indirect Prompt Injections** - útok se skrývá v externích zdrojích jako svou obrázky, dokumenty nebo jiné weby
