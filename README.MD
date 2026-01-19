# Entry projekt - Seznam Flutter Vývojář

Toto jsou instrukce pro kandidáty na flutter vývojáře v Seznamu. Jde o velmi malý projekt určený pro otestování základních dovedností. Projekt je navržen tak, aby byl zpracovatelný pro všechny úrovně od juniora po seniora, vypracujte jej dle vlastních schopností. Není očekáváno, že každý zvládne vše na 100%.


## Popis

Vytvořte repozitář na [GitHubu](https://github.com/) s Flutter aplikací pracující s [Rick & Morty API](https://rickandmortyapi.com/). Na tomto úkolu demonstrujte dobrou práci s Rest Api, Dartem a Flutterem. Primárně je třeba vypracovat **povinné zadání** a až poté doporučuji pracovat na bonusových bodech. Bonusové body nejsou povinné, ovšem mohou významně pomoci vaší šanci. Úkol lze pojmout jednoduše a vypracovat velmi rychle, zároveň je možné na něm prokázat porozumění architektuře a design patternům. Jak řešení, tak architekturu vyberte vhodně vůči projektu, ovšem zamyslete se i nad teoretickým rozšířením ("není vhodné vše overengineerovat, ale ukažte, že chápete softwarové principy"). Tento úkol bude velmi pravděpodobně součástí dalšího kola výběrového řízení a proto důrazně doporučuji vypracovat jej samostatně. Tento úkol se primárně zaměřuje a hodnotí kvalitu kódu, pochopení softwarových principů a Flutteru jako takového, ale za příjemný design a především za dobře uchopene UX získáte bonusové body.


## Povinné zadání

Vytvořte mobilní aplikaci fungující jako katalog postav z populární show Rick & Morty. Použití již existujícího Dart klienta je zakázáno.

### Požadavky

- Obrazovka umožňující procházet jednotlivé postavy `https://rickandmortyapi.com/api/character`
- Obrazovka s detailem, zobrazující meta data postavy
- Možnost postavu označit jako oblíbenou a přidat k ní poznámku
- Vyhledávání v charakterech (alespoň podle jednoho atributu)
- V detailu je povinné uživateli zobrazit přinejmenším: Obrázek postavy, jméno, status, druh, list episod v kterých se objevil 


### Poznámky a tipy

- Zamyslete se nad vhodným řešením stavu - [Riverpod](https://pub.dev/packages/flutter_riverpod) je silně doporučen, ale jakékoliv jiné řešení, včetně použití pouze built-in primitiv je akceptováno
- Oblíbené a poznámky v povinném zadání není nutné mít persistentně, ale během jedné session (dokud je aplikace běžící) musí být stav zjevný (Pokud dám like na postavu, chci vidět, že je v oblíbených i na výpise a i když detail zavřu a znovu otevřu)
- Vzhledem k velkému množství postav je třeba se zamyslet nad přístupem k jejich vykreslování (pages / infinite scroll) - oboje má své pro a proti 
- Pro animace je výborná knihovna [Flutter Animate](https://pub.dev/packages/flutter_animate)
- Pro neprimitivní tipy v Hive je vhodné použít type adaptéry
- Zamyslete se nad ošetřením erroru a loading stavu
- Co se knihoven týka méně je více. Dobrý developer ví, že není třeba znovu vynalézt kolo, ale zároveň také fakt, že všechen kód, který přimo nespravujete je potenciální riziko.
  

## Bonusové body

- Debouncing vyhledávání
- Animace jakékoliv formy (implicitní, explicitní, [Rive](https://pub.dev/packages/rive), [Lottie](https://pub.dev/packages/lottie),...) 
- Lokální ukládání like a poznámek - [Hive](https://pub.dev/packages/hive_ce) je silně doporučen, ale samozřejmě je možné si obhájit i jiné
- Použití interceptorů (například logování komunikace)
- Využití dalších endpointů (například práce s episodami a lokacemi)
- Vyhledávání postav podle všech dostupných atributů
- Cokoliv dalšího, co vás napadne a chcete ukázat

## Výstup

Výstupem by měl být Github repozitář, obsahující kód a **README.MD s instrukcemi pro spuštění aplikace**. Nezapomeňte uvést všechny potřebné kroky (například v případě použití generování souborů). README by také měl obsahovat stručný popis všeho, co jste použili a to zejména všeho nad rámec zadání. Formalita ani rozsah Readme není relevantní, ale snažte se obsáhnout vše a pokud možno stručně (Aby se to lépe kontrolovalo). Veškeré postřehy a komentáře můžete rovněž uvést do README. Pokud jste některé kroky nesplňili nebo některé částí vědomě udělali neoptimálně, rovněž je uveďte do README pro kontext.
