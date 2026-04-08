# Iteratív pszeudocímkézés és kalibrációs kísérletek
![Python](https://img.shields.io/badge/Python-3.12.13-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.19.0-orange)
![NumPy](https://img.shields.io/badge/NumPy-2.0.2-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.2.2-purple)
![SciPy](https://img.shields.io/badge/SciPy-1.16.3-darkblue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.6.1-f7931e)
![Joblib](https://img.shields.io/badge/Joblib-1.5.3-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.10.0-red)
![Colab](https://img.shields.io/badge/Google%20Colab-H100-yellow)
![GPU](https://img.shields.io/badge/GPU-NVIDIA%20H100-76B900)

Ieratív tanár-diák alapú pszeudocímkézési kísérleti keretrendszer képosztályozási adathalmazokra.  
A cél annak vizsgálata, hogy a különböző kalibrációs módszerek és az entrópia alapú mintakiválasztás hogyan befolyásolják a pszeudocímkék minőségét és a modell teljesítményét.

## Támogatott adathalmazok
- CIFAR-10
- CIFAR-100
- SVHN

A kísérletek Google Colab környezetben, NVIDIA H100 GPU használatával futottak. 
A megvalósítás Python 3.12.13 programozási nyelven történt. A tanítási és kiértékelési folyamatok TensorFlow 2.19.0 keretrendszerre épültek. A numerikus műveletekhez és tömbkezeléshez a NumPy 2.0.2, az eredmények táblázatos feldolgozásához és mentéséhez a Pandas 2.2.2, a statisztikai próbákhoz a SciPy 1.16.3, az adatfelosztáshoz és a kiértékelési mutatók számításához a scikit-learn 1.6.1, a párhuzamosított részfeladatokhoz és egyes kalibrációs modellek mentéséhez a Joblib 1.5.3, az ábrák elkészítéséhez pedig a Matplotlib 3.10.0 könyvtárverzió került felhasználásra. 

## Főbb funkciók
- tanár-diák iteratív tanítás
- pszeudocímke-generálás konfidencia és entrópia alapján
- többféle utólagos kalibrációs módszer összehasonlítása
- metrikák, statisztikai összesítések és CSV kimenetek mentése
- futás folytatása korábban mentett állapotból
