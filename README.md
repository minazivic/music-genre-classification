# Music Genre Classification

## Cilj istraživanja

Cilj ovog projekta je razvoj modela mašinskog učenja za automatsku klasifikaciju muzičkih žanrova. 
Na osnovu numeričkih audio karakteristika i tekstualnih tagova, modeli pokušavaju da prepoznaju kojem muzičkom žanru pripada određeni audio zapis.

U okviru istraživanja analiziran je uticaj različitih algoritama klasifikacije i metoda redukcije dimenzionalnosti na tačnost modela. Poseban fokus stavljen je na kombinovanje audio karakteristika i tekstualnih informacija kako bi se poboljšala klasifikacija muzičkih zapisa.

---

## Metodologija

U projektu je primenjen standardni proces obrade podataka i treniranja modela mašinskog učenja:

1. Učitavanje i spajanje datasetova (`features` i `tracks`)
2. Obrada tekstualnih tagova
3. Transformacija tagova u numerički oblik korišćenjem **TF-IDF vektorizacije**
4. Podela podataka na **trening i test skup**
5. Primena metoda **redukcije dimenzionalnosti**:
   - SelectKBest
   - PCA (Principal Component Analysis)
6. Treniranje i poređenje više modela klasifikacije

Korišćeni algoritmi klasifikacije:

- LightGBM
- Random Forest
- Extra Trees
- HistGradientBoosting
- Linear SVM
- Logistic Regression

Performanse modela procenjene su korišćenjem **accuracy metrike** i **confusion matrix analize**.

---

## Skup podataka

Dataset korišćen u ovom projektu je Free Music Archive (FMA) dataset.

Fajlovi tracks.csv i features.csv preuzeti su iz zvaničnog repozitorijuma:

https://github.com/mdeff/fma

Dataset sadrži veliki broj audio zapisa zajedno sa numeričkim audio karakteristikama i metapodacima, uključujući muzičke žanrove i opisne tagove.

---

## Autor

Mina Živić 240/2019





