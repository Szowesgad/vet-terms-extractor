# VET-TERMS-EXTRACTOR

Automatyczny system ekstrakcji i zarządzania terminologią weterynaryjną z wykorzystaniem Brave Search i LLM.

## Opis

System służy do automatycznego wzbogacania słownika terminologii weterynaryjnej, wykorzystując API Brave Search oraz modele językowe (LLM) do ekstrakcji, przetwarzania i walidacji specjalistycznych terminów.

## Główne funkcje

- Automatyczne wyszukiwanie i ekstrakcja terminów weterynaryjnych z sieci
- Przetwarzanie wyników wyszukiwania przy użyciu modeli językowych
- Walidacja i weryfikacja terminów pod kątem poprawności merytorycznej
- Zapisywanie ustrukturyzowanych danych w formacie JSON
- Możliwość rozszerzenia o interfejs webowy (Django)

## Wymagania

- Python 3.8+
- Klucz API dla Brave Search
- Klucz API dla OpenAI/Anthropic/innego modelu LLM

## Instalacja

```bash
# Klonowanie repozytorium
git clone https://github.com/Szowesgad/vet-terms-extractor.git
cd vet-terms-extractor

# Instalacja zależności
pip install -r requirements.txt

# Konfiguracja zmiennych środowiskowych
export BRAVE_API_KEY=twój_klucz_api
export OPENAI_API_KEY=twój_klucz_api
```

## Użycie

```bash
# Uruchomienie podstawowego extractora terminów
python src/extractor.py

# Uruchomienie interfejsu webowego
python src/webapp/manage.py runserver
```

## Struktura projektu

```
vet-terms-extractor/
├── dataset/           # Katalog na dane słownikowe
├── src/               # Kod źródłowy
│   ├── extractor.py   # Główny skrypt ekstrakcji
│   ├── utils.py       # Funkcje pomocnicze
│   └── webapp/        # Aplikacja Django (opcjonalna)
├── tests/             # Testy jednostkowe
└── requirements.txt   # Zależności
```

## Licencja

MIT
