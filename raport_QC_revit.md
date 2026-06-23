# RAPORT QC MODELU REVIT

**Projekt:** Budynek biurowy XYZ  
**Lokalizacja:** Warszawa  
**Data kontroli:** 23.06.2026  
**Wersja modelu:** Revit 2024  
**Autor kontroli:** Tomasz Olechowski  
**Dział:** BIM / QC  

---

## 1. CEL RAPORTU

Celem niniejszego raportu jest ocena jakości modelu BIM (Revit) pod kątem:
- zgodności ze standardami BIM,
- poprawności geometrii,
- kompletności danych,
- przygotowania do dalszych etapów (koordynacja / eksport / dokumentacja).

---

## 2. ZAKRES KONTROLI

Zakres kontroli obejmował:
- model architektoniczny (AR)
- model konstrukcyjny (ST)
- model instalacji (MEP – w zakresie podstawowym)

---

## 3. NARZĘDZIA KONTROLNE

- Autodesk Revit (przegląd manualny)
- Navisworks Manage (kolizje)
- Dynamo (kontrola parametrów)
- BIM Interoperability Tools

---

## 4. PODSUMOWANIE

| Kategoria              | Status      | Uwagi                     |
|----------------------|------------|--------------------------|
| Geometria            | ⚠️ Uwaga   | Drobne błędy             |
| Nazewnictwo          | ❌ Błędy   | Niezgodności             |
| Parametry            | ⚠️ Uwaga   | Braki części danych      |
| Kolizje              | ❌ Błędy   | Wykryte konflikty        |
| Poziomy i siatki     | ✅ OK      | Bez uwag                 |

---

## 5. SZCZEGÓŁOWE UWAGI

### 5.1 Geometria
- Występują duplikaty elementów (np. ściany w osi A-1)
- Niektóre elementy nie są przypisane do właściwych poziomów
- Modele instalacyjne częściowo niespójne z architekturą

---

### 5.2 Nazewnictwo
- Nieprzestrzeganie standardu nazewnictwa rodzin:
  - np. `Wall_01` zamiast `AR_WALL_EXT_200`
- Brak spójności w nazwach widoków

---

### 5.3 Parametry
- Brak uzupełnionych parametrów:
  - `Mark`
  - `Type Comments`
  - `Phase`
- Niespójne wartości parametrów materiałowych

---

### 5.4 Kolizje (Navisworks)

**Najważniejsze kolizje:**
- Instalacje HVAC vs belki konstrukcyjne
- Kanały wentylacyjne vs sufity podwieszane
- Rury sanitarne vs ściany nośne

**Szacowana liczba kolizji:** ~45

---

### 5.5 Poziomy i siatki

- Poprawnie zdefiniowane poziomy
- Spójność pomiędzy modelami branżowymi
- Brak duplikatów

---

## 6. REKOMENDACJE

1. Ujednolicić nazewnictwo zgodnie ze standardem BIM
2. Uzupełnić brakujące parametry w modelu
3. Usunąć zduplikowane elementy
4. Przeprowadzić pełną koordynację międzybranżową
5. Ponownie wykonać analizę kolizji po poprawkach

---

## 7. STATUS KOŃCOWY

**Model wymaga poprawek przed kolejnym etapem projektu.**

---

## 8. ZAŁĄCZNIKI

- Raport kolizji (Navisworks)
- Zrzuty ekranu błędów
- Lista elementów do korekty

---

## 9. PODPIS

..............................................  
*Tomasz Olechowski*  
Senior Technician / BIM QC
