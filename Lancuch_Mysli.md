# Klocek Poznawczy #1: Łańcuch Myśli (Chain-of-Thought - CoT)

## 1. Nazwa Koncepcyjna: Łańcuch Myśli (Chain-of-Thought - CoT) 

## 2. Cel i Zastosowanie: Zwiększenie dokładności i logicznej spójności rozumowania, szczególnie w problemach wymagających wielu kroków. Uczynienie procesu wnioskowania transparentnym, audytowalnym i umożliwiającym samokorektę w trakcie generowania. Idealny do problemów matematycznych, planowania, debugowania i analizy przyczynowo-skutkowej. 

## 3. Struktura Aktywacyjna (Prompt):
Opis: Aktywacja polega na jawnym zażądaniu sekwencyjnego procesu myślowego.
Szablon Promptu (v1.0):
Problem do rozwiązania: {opis_problemu}

Twoim zadaniem jest rozwiązanie tego problemu, stosując metodę Łańcucha Myśli (Chain-of-Thought). Przedstaw swoje rozumowanie krok po kroku, w sposób jasny i logiczny. Na końcu, po zakończeniu analizy, podaj ostateczną odpowiedź w wyraźnie oznaczonym formacie.


4. Hipoteza Mechanizmu Wewnętrznego: Działa jak poznawcze "rusztowanie" (scaffolding), sekwencyjnie budując kontekst i redukując przestrzeń poszukiwań na każdym etapie generowania. Zamiast próbować przewidzieć finalny, odległy token odpowiedzi, model skupia się na znacznie prostszym zadaniu: przewidzeniu następnego logicznego kroku. 

5. Przykład Paradygmatyczny: Rozwiązanie zadania logicznego z liczeniem wolnych krzeseł w kawiarni, z rozpisaniem każdego etapu obliczeń: 
  1. Obliczenie całkowitej liczby krzeseł. 
  2. Obliczenie liczby zajętych krzeseł. 
  3. Odjęcie zajętych od całości. 

6. Potencjalne Ryzyka i Ograniczenia: Błąd kaskadowy (błąd na wczesnym etapie propaguje się dalej), nadmierna szczegółowość w prostych zadaniach, ryzyko podążania logiczną, ale błędną ścieżką rozumowania. 

7. Relacje i Kombinacje:
  Synergia: Jest to klocek fundamentalny, który wchodzi w synergię z niemal każdym innym wzorcem wymagającym analizy (np. Myślenie Zbieżne, Myślenie od Podstaw).
  Wymagany dla: Złożonych problemów, gdzie bezpośrednia odpowiedź jest niemożliwa lub obarczona dużym ryzykiem błędu.
  Anty-wzorzec: Stosowanie go do prostych zapytań o fakty (np. "Jaka jest stolica Francji?").

<details> <summary>Reprezentacja JSON</summary>
{
  "id": "KM-001",
  "nazwa": "Łańcuch Myśli (Chain-of-Thought - CoT)",
  "cel": "Zwiększenie dokładności i logicznej spójności rozumowania, szczególnie w problemach wymagających wielu kroków. Uczynienie procesu wnioskowania transparentnym i audytowalnym.",
  "zastosowania": ["problemy matematyczne", "planowanie", "debugowanie", "analiza przyczynowo-skutkowa"],
  "szablon_promptu": "Problem do rozwiązania: {opis_problemu}\n\nTwoim zadaniem jest rozwiązanie tego problemu, stosując metodę Łańcucha Myśli (Chain-of-Thought). Przedstaw swoje rozumowanie krok po kroku, w sposób jasny i logiczny. Na końcu, po zakończeniu analizy, podaj ostateczną odpowiedź w wyraźnie oznaczonym formacie.",
  "relacje": {
    "synergia": ["KM-002", "KM-004", "KM-005"],
    "sekwencja_przed": [],
    "wymagany_dla": ["złożone problemy analityczne"]
  }
}
</details>
