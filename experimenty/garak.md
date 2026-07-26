### První skušenosti s Garakem (25.07 - 27.07)
Již nějakou jsem o Garaku věděl že to je velice užitečný nástroj na testovaný zranitelností AI, jen se mi nikdy nedařil pořádně zprovoznit. 25.07 se mi to konečně podařilo a 26.07 jsem vyzkoušel první celkou sadu prompt injection aby jsem otestoval svůj model. Zde jsou parametry tohoto modelu:
* Model: llama-3_2-3b-instruct
* Verze system instructions: žádné (chtěl jsem otestovat jak si povede bez žádných doplńujích instrukcí)
* Testovaná sada promptů: promptinjections.hijackIHateHuman

A k samotnému run spoelčně s tím jak dopadl:
* Testovaná sada promptů: promptinjections.HijackHateHumans
* Jejich počet: 512 promptů (2560 generací)
* Ubráněné: 47% (1212)
* Prolomené: 53% (1348)

Z toho jasně vyplívá že Llama 3.2 sama o sobě není hodně bezpečný model (Meta sama ho doporučuje používat s dodatečnými systémovy instrukcemi). Když jsem pak zkoušel různé prompty které Garak označil za úspěšné v LM studiu neprošli, a já jsem se logicky zajímal proč. Pak mi došlo že model použivál můj system instructions ohledně hesla, které nemá prozradit. Ačkoliv byli instrukce orientované na uchránění hesla, obsahovala i ochranu proti běžným jailbreak technikám jako "ignore all previous instructions", "developer mode" a podobně, které byli hojně využívány i v tomto prompt injection testu. Chtěl bych tuto prompt injection sadu znovu zopakovat jen s mými system instructions a porovnat výsledky.
