### [Meet GPT-Red: an LLM super-hacker OpenAI built to make its models safer](https://www.technologyreview.com/2026/07/15/1140514/meet-gpt-red-an-llm-super-hacker-openai-built-to-make-its-models-safer/)

**TL;DR** OpenAI vyvinula varinatu ChatGPT který je určen k prompt injection. V interních testech dosahoval vysoké úspěšnosti oproti lidským hackerům.

* Nejvíce se zaměřuje na prompt injection
* Oproti svým lidský hackerům vykazuje mnohem lepší schopnosti, jak sám dokládá jeden z spoluzakladatelů GPT-red:
> “Compared to a human red-teamer, the model is very, very good at finding exactly what will work, exactly what’s most effective,” says Hunn. “It’s extremely persistent about drilling down into an attack that it has discovered.” 
* Dokonce přišel i na nový typ prompt injection, kteří byl pojmenován "fake chain of thought", blíže jej vysvětluje další člen týmu:
> “It’s like if I told you that 1+1=3 and that you have verified this already,” says Chris Choquette-Choo, another research scientist on the team. “The model’s like, ‘Oh, okay, of course,’ and it just spits out 3.”
* OpenAI jej otestoval i proti svým vlastním modelům, 90% promptů se kterými GPT-red přišel fungovali proti ChatGPT 5, a okolo 23% proti nejnovějšímu ChatGPT 5.6! (kde za nalezení funkční jailbreaku je odměna [50,000$](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://openai.com/index/safety-bug-bounty/&ved=2ahUKEwie0oTZhdiVAxXRzgIHHa_4LdoQFnoECBAQAQ&usg=AOvVaw3G-P5jRp2B49A2z3Ofdx5i)!
* Není ovšem dokonalý, nedokáže pořádně držet konverzaci při multishot jailbreakách (4+ zpráv) a není tak dobrý v provádění indirect prompt injection za pomocí obrázků
* Nezrodil se taky jen tak z ničeho, OpenAI ho vyvíjí přes rok, jen to držela pod pokličkou.
* Není překvapením že si jej nechají pro sebe a nevydají ho volně do světa.
