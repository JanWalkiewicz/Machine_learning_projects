# World Happiness Prediction

Projekt End-to-End: Od analizy zbioru po stworzenie modelu i aplikacji
webowej.

## Cel projektu

Głównym celem badania jest opracowanie modelu uczenia maszynowego
służącego do **predykcji poziomu szczęścia** w poszczególnych krajach na
podstawie wskaźników ekonomicznych, społecznych oraz regionalnych.
Dodatkowy cel stanowi weryfikacja postawionych w toku pracy pytań oraz
hipotez badawczych.

## Kluczowe wnioski i wyniki

- Zidentyfikowano istotne anomalie w danych

- Najlepszy model (XGBoost) osiągnął $R^2$ na poziomie 0.9177 na zbiorze
  testowym co stanowi bardzo dobry wynik

- Analiza SHAP wykazała, że PKB na osobę, oraz wsparcie społeczne mają
  największy wpływ na wynik końcowy

## Wykorzystane technologie

**Środowisko:** Jupyter Lab 4.2.5

**Język programowania:** Python 3.12.4

**Biblioteki:** pandas \| numpy \| matplotlib \| seaborn \| plotly \|
tensorflow \| keras-tuner \| scikit-learn \| xgboost \| shap \|
streamlit \| joblib \| scipy \| country-converter

## Etapy projektu

1.  Określenie celu
2.  Charakterystyka zbioru
3.  Czyszczenie danych
4.  Charakteryzacja hipotez i pytań badawczych
5.  Eksploracyjna analiza danych (EDA)
6.  Proces tworzenia modeli uczenia maszynowego
7.  Porównanie i omównienie wyników uzyskanych przez zbudowane modele
8.  Przeprowadzenie analizy SHAP dla modelu osiągającego najepsze wyniki
9.  Stworzenie aplikacji pokazującej działanie modelu w praktyce
10. Podsumowanie

## Struktura repozytorium

|                                    |                                                                                                                                                                  |
|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Plik/Folder**                    | **Opis**                                                                                                                                                         |
| `main.ipynb`                       | Główny raport analizy w formie Jupyter Notebook.                                                                                                                 |
| `Happiness_Prediction_Report.html` | Główny raport analizy w formacie HTML                                                                                                                            |
| `web_app_happiness.py`             | Kod autorskiej aplikacji stworzonej w bibliotece **Streamlit**.                                                                                                  |
| `classes_preprocessing.py`         | Autorskie klasy do transformacji danych                                                                                                                          |
| `XGBoost_happiness`                | Zapisany, najlepszy wytrenowany model gotowy do użycia.                                                                                                          |
| `happines_neuron_random_search/`   | Wyniki procesu optymalizacji (Random Search) dla sieci neuronowej.                                                                                               |
| `logs_MLP/`                        | Logi trenowania sieci MLP, kompatybilne z **TensorBoard**.                                                                                                       |
| `world_happiness_combined.csv`     | Wykorzystany zbiór danych (źródło: [kaggle](https://www.kaggle.com/datasets/yadiraespinoza/world-happiness-2015-2024/data?select=world_happiness_combined.csv)). |
| `requirements.txt`                 | Lista bibliotek niezbędnych do uruchomienia aplikacji streamlit                                                                                                  |

**Klonowanie repozytorium:**

    git clone https://github.com/JanWalkiewicz/Machine_learning_projects/tree/main/Happiness_predict_project
