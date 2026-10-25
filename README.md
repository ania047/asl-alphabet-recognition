# Recunoașterea alfabetului ASL din imagini, cu augmentare generativă

Proiect de semestru - Computer Vision 3
**Student:** Ioniță Ana-Maria, SIVA

## Descriere
Clasificare de imagini pentru alfabetul limbajului semnelor american (29 de clase),
cu un CNN propriu în PyTorch, într-un regim cu date limitate. Setul de antrenare este
augmentat ulterior cu imagini generate de un model generativ condițional (cGAN / VAE),
iar efectul este analizat într-un raport de optimizare.

## Set de date
ASL Alphabet (Kaggle, grassknoted):
https://www.kaggle.com/datasets/grassknoted/asl-alphabet

### Descărcare
```bash
# necesită contul Kaggle și token-ul API (kaggle.json)
kaggle datasets download -d grassknoted/asl-alphabet -p data/ --unzip
```
Pe Kaggle Notebooks, setul se atașează direct din meniul "Add data".

## Instalare
```bash
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```
