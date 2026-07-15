### OWASP  top 10 for LLMs ([odkaz](https://genai.owasp.org/llm-top-10/))

1. [Prompt Injection](./red-teaming#Prompt-Injection)

##### [Prompt Injection](https://genai.owasp.org/llmrisk/llm01-prompt-injection/)
Pomocí promptů (a další médií včetné dokazů jiné stránky, obrázky atd) útočník zmanipuluje AI aby dělala věci které má zakázany dělat.Prompt Injection se dělí na dva podruhy:
1. **Direct Prompt Injections** - útočník přímo napíše AI prompt, využívá k tomu jen text
2. **Indirect Prompt Injections** - útok se skrývá v externích zdrojích jako svou obrázky, dokumenty nebo jiné weby
