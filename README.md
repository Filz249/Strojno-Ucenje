# Strojno-Ucenje

<details>
<summary><strong>1. Što je umjetna inteligencija? Što je strojno učenje? Koja je razlika između eksplicitnog programiranja računala i strojnog učenja? Navedite kakvi problemi se rješavaju pojedinim pristupom (primjeri).</strong></summary>

**Umjetna inteligencija** odnosi se na simulaciju ljudske inteligencije u sustavima koji sud izajnirani da „misle” i djeluju upoput ljudi. Ovi su sustavi osposobljeni za obavljanje zadataka koji obično zahtijevaju ljudsku inteligenciju, kao što je prepoznavanje govora, donošenje odluka i rješavanje problema.

**Strojno učenje** je način programiranja računala s ciljem optimiziranja određenog kriterija uspješnosti koristeći podatke ili prošlo iskustvo. NPR: Spam filter

**Eksplicitno programiranje** tradicionalna je metoda rješavanja određenog zadatka na način da se eksplicitno definiranju koraci ili pravila koje bi računalo trebalo slijediti. NPR: Sortiranje niza 

Razlika između strojnog učenja i eksplicitnog programiranja je ta da kod strojnog učenja, računalo uči iz podataka, dok kod eksplicitnog programiranja programer specificira na koji način se zadatak izvršava.



</details>

---
<br>
<br>

<details>
<summary><strong>2. Navedite vrste strojnog učenja te za svaki tip minimalno dva primjera.</strong></summary>

**1. Nadzirano učenje** - Nadzirano oučenje je način strojnog učenja gdje je ciljo drediti nepoznatu funkcionalnu ovisnost između ulaznih veličina (atributa,značajki) i izlazne veličine (ciljnevarijable) na temelju podatkovnih primjera.

- NPR: procjena cijena kuća, automobila, spam/notspam (true/false).

**2. Nenadzirano učenje** - kod problema nenadziranog učenja n araspolaganju su samo podaci o ulaznim veličinama, a izlazna veličina nepostoji.
primjeri:

- grupiranje podataka: segmentacija tržišta/kupaca, grupiranje sličnih dokumenata,kompresija slike

- smanjivanje dimenzionalnosti: kompresija podataka, vizualizacija podataka, hibridizacija s modelima koji se dobivaju nadziranim učenjem.

- detekcija nepravilnosti u podacima.

**3. Podržano učenje** - Podržano učenje omogućava agentu da samostalno otkrijeo ptimalno ponašanje metodom pokušaja i pogreški u određenoj okolini.

- Primjeri: stroj koji igra šah, mobilni robot koji traži izlaz iz labirinta



</details>

---
<br>
<br>

<details>
<summary><strong>3. Nacrtajte blok dijagram procesa izgradnje modela primjenom strojnog učenja te objasnite svaki njegov dio.</strong></summary>

<img width="1038" height="729" alt="image" src="https://github.com/user-attachments/assets/50422cf3-64c0-493a-9899-419a7839a2de" />

  


</details>

---
<br>
<br>

<details>
<summary><strong>4. Što je eksplorativna analiza podataka (EDA)? Koji grafički prikazi se koriste prilikom EDA? Objasnite ih.</strong></summary>

**EDA** je set korisnih tehnika i pruža važne uvide u podatke, uključujući distribuciju značajki, prisutnosti zostalih vrijednosti (engl.missing values) ili stršećih vrijednosti (engl.outliers), te odnos između različitih ulaznih veličina.

Koriste se: 
**Histogram** - graf koji predstavlja distribuciju skupa kontinuiranih ili diskretnih podataka. Sastoji se od stupaca koji se nalazena x-osi kako bi predstavili raspon vrijednosti u skupu podataka, a visina svakog stupca predstavlja učestalost podatkovnih točaka unutar tog raspona.

**Dijagram raspršenja** (engl.scatterplot) -  To je graf koji prikazuje odnos između dvije kontinuirane ili diskretne veličine i crtavanje podatkovnih primjera u dvije dimenzionalnoj ravnini. Svaka je podatkovna točka predstavljena kao točka na grafikonu, pri čemu x-os predstavlja vrijednost jedne veličine, a y-os druge. Može se dobiti uvid u odnos između dvije veličine, jačina odnosa, smjer odnosa i prisutnost stršećih vrijednosti.

**Matrica dijagrama raspršenja** - Dijagrami raspršenja između svih veličina.

**Kutijasti dijagram** (engl.boxplot) - Kompaktan prikaz distribucije kontinuiranih ili diskretnih podataka. Sastoji se od okvira koji predstavlja srednjih 50% podataka, što je interkvartilni raspon(IQR). Okvir je nacrtan između prvog (donjeg) kvartila i trećeg (gornjeg) kvartila podataka. Medijan je označen linijom unutar okvira. Linije prikazuju raspon podataka, isključujući stršeće vrijednosti. Stršeće vrijednosti ako postoje su predstavljene kao pojedinačne točke izvan linija.

**Stupčasti dijagram** (engl.barplot) - U stupčastom dijagramu svaka je kategorija predstavljena stupcem, pri čemu duljina stupca predstavlja učestalost ili broj podatkovnih primjera unutar kategorije. Kategorije su obično predstavljene na x-osi, a učestalost ili broj na y-osi. Daje uvid u distribuciju kategoričkih veličina, uključujući učestalost ili broj svake kategorije.


</details>

---
<br>
<br>

<details>
<summary><strong>5. Što je korelacija između veličina? Navedite primjere.</strong></summary>
  
**Korelacija** je statistička mjera koja predstavlja snagu i smjer odnosa između dvije varijable, koristi za procjenu odnosa između varijabli i za prepoznavanje bilo kakvih obrazaca ili trendova u podacima.

<ins>Primjer</ins>: Visina i težina ljudi

- Varijabla X: visina (u cm)

- Varijabla Y: težina (u kg)


</details>

---
<br>
<br>

<details>
<summary><strong>6. Objasnite osnovne postupke u predobradi podataka (podatkovnog skupa).</strong></summary>

- Odabrati relevantne ulazne veličine od svih dostupnih.

- Stršeće i izostale vrijednosti je potrebno ukloniti ili nadomjestiti.

- Kategoričke varijable potrebno je transformirati u oblik koji zahtijeva algoritam strojnog učenja.

- Numeričke varijable je potrebno skalirati.
  

</details>

---
<br>
<br>

<details>
<summary><strong>7. Što su to izostale vrijednosti ili stršeće vrijednosti? Kako ih u praksi pronalazimo? Kako postupamo s takvim vrijednostima?</strong></summary>

**Stršeće vrijednosti** - podatkovne vrijednosti koje znatno odstupaju od ostalih vrijednosti u skupu podataka. One mogu iskriviti analize ili modele.

U CSV formatu jednostavno ne bude upisana vrijednost, ili je upisana nekatipična vrijednost koja predstavlja nepostojeću vrijednost, kao što je NULL, NaN, NA i slično.

Njih možemo:

- Nadomjestiti – postoje razne metode (npr. zamijeniti sa srednjom vrijednošću veličine, najčešćom vrijednošću i slično).
  
- Izbaciti podatkovne primjere ili veličine gdje se pojavljuju izostale vrijednosti.


</details>

---
<br>
<br>

<details>
<summary><strong>8. Objasnite kakve su to kategoričke veličine i načine njihovog kodiranja. Napišite jednostavne primjere.</strong></summary>

**Nominalne veličine** – ne postoji odnos između mogućih vrijednosti (npr. boja očiju osobe, spol i slično).

```
bill_length_mm: bill length (mm)

bill_depth_mm: bill depth (mm)

flipper_length_mm: flipper length (mm)

body_mass_g: body mass (g)
```

**Ordinalne veličine** – postoji odnos između mogućih vrijednosti te je moguće ovakve vrijednosti poredati odnosno sortirati (npr. stupanj obrazovanja osobe, dobna skupina, ocjena iz kolegija, zadovoljstvo korisnika usluge i slično).

```
island: island name

species: penguin species

sex: penguin sex
```
  

</details>

---
<br>
<br>

<details>
<summary><strong>9. Objasnite načine skaliranja numeričkih veličina. Napišite jednostavan primjer.</strong></summary>

**1. Min-Max skaliranje** (normalizacija) - Min-max skaliranje transformira vrijednosti ulazne veličine xˇj na željeni raspon, tipično `[0, 1]`.
  
<img width="386" height="104" alt="image" src="https://github.com/user-attachments/assets/a414e602-936a-4f8d-8b9a-529117caa35e" />


**2. Standardizacija (Z-score)** - Standardizacija ulaznih veličina predstavlja skaliranje gdje podaci za svaku ulaznu veličinu imaju srednju vrijednost 0 i varijancu jednaku 1:

<img width="913" height="135" alt="image" src="https://github.com/user-attachments/assets/345b5553-3b84-480c-b8c5-56fc2cbc0af9" />

<ins>Primjer</ins>

| Originalne vrijednosti | Min-max skaliranje | Standardizacija |
|-----------------------|---------------------|-----------------|
| 100                   | 0                   | -1.44280393     |
| 120.2                 | 0.202               | -0.94528533     |
| 180.8                 | 0.547               | 0.54727045      |
| 190.9                 | 0.796               | 0.79602975      |
| 201                   | 1.000               | 1.04478905      |



</details>

---
<br>
<br>

<details>
<summary><strong>10. Objasnite nadzirano učenje i princip označavanja dostupnog skupa podataka. Koja dva glavna tipa problema postoje u okviru nadziranog učenja?</strong></summary>

**Nadzirano učenje** - Nadzirano oučenje je način strojnog učenja gdje je cilj odrediti nepoznatu funkcionalnu ovisnost između ulaznih veličina (atributa,značajki) i izlazne veličine (ciljnevarijable) na temelju podatkovnih primjera.

Obično podatke predstavljamo u obliku matrica i vektora. 

Postoje regresijski i klasifikacijski problemi.


</details>

---
<br>
<br>

<details>
<summary><strong>11. Objasnite jednostavnu linearnu regresiju. Objasnite kriterijsku funkciju, skicirajte prikladni primjer.</strong></summary>

**Jednostavna linearna regresija** opisuje odnos između jedne ulazne veličine \(x\) i jedne izlazne veličine \(y\) pomoću pravca.

Model:

y = θ₀ + θ₁x

gdje su:
- x – ulazna veličina  
- y – izlazna veličina  
- θ₀ – odsječak na osi  
- θ₁ – nagib pravca

**Kriterijska funkcija** mjeri koliko dobro model opisuje podatke.  
Najčešće se koristi **srednja kvadratna pogreška (MSE)**:

J(θ) = (1/n) Σ (yᵢ − ŷᵢ)²

Cilj je pronaći parametre koji minimiziraju pogrešku između stvarnih i predviđenih vrijednosti.

Primjer: procjena plaće osobe na temelju radnog staža.

</details>

---
<br>
<br>

<details>
<summary><strong>12. Objasnite postupak procjene parametara linearnog regresijskog modela gradijentnom metodom. Koje su razlike između batch metode, stohastičke metode i mini-batch stohastičke metode?</strong></summary>

Parametri modela mogu se odrediti **gradijentnim spustom (gradient descent)**.

Algoritam:
1. Odabiru se početne vrijednosti parametara
2. Izračuna se gradijent kriterijske funkcije
3. Parametri se ažuriraju u smjeru negativnog gradijenta

![Formula](https://github.com/Filz249/Strojno-Ucenje/blob/main/formula)

gdje je α duljina koraka (learning rate).

**Batch gradient descent**
- koristi cijeli skup podataka u svakoj iteraciji

**Stohastički gradient descent (SGD)**
- parametri se ažuriraju nakon svakog podatkovnog primjera

**Mini-batch gradient descent**
- parametri se ažuriraju koristeći male skupine podataka

</details>

---
<br>
<br>

<details>
<summary><strong>13. Objasnite višedimenzionalnu linearnu regresiju. Navedite primjer.</strong></summary>

Višedimenzionalna linearna regresija koristi **više ulaznih veličina**.

Model:

![alt text](https://github.com/Filz249/Strojno-Ucenje/blob/main/formula2)

Primjer:

Procjena cijene kuće na temelju:
- površine
- broja soba
- starosti kuće
- lokacije.

</details>

---
<br>
<br>

<details>
<summary><strong>14. Objasnite polinomsku regresiju. Objasnite podusklađivanje (underfitting) i pretjerano usklađivanje na podatke (overfitting) na primjeru polinomske regresije.</strong></summary>

Polinomska regresija koristi se kada odnos između ulazne i izlazne veličine nije linearan.

Primjer modela:

y = θ₀ + θ₁x + θ₂x² + θ₃x³

**Underfitting** – model je prejednostavan i ne može dobro opisati podatke.

**Overfitting** – model je previše prilagođen podacima za učenje i loše generalizira na nove podatke.

</details>

---
<br>
<br>

<details>
<summary><strong>15. Što je evaluacija ili vrednovanje izgrađenog modela. Skicirajte princip evaluacije. Navedite metrike za vrednovanje regresijskih modela.</strong></summary>

Evaluacija modela predstavlja procjenu kvalitete modela.

Postupak:
1. Podaci se podijele na skup za učenje i testni skup
2. Model se trenira na skupu za učenje
3. Model se testira na testnom skupu

Skica:
![alt text](http://github.com/Filz249/Strojno-Ucenje/blob/main/evaluacija)

**Metrike za regresiju:**
- MAE (Mean Absolute Error)
- MSE (Mean Squared Error)
- RMSE (Root Mean Squared Error)

</details>

---
<br>
<br>

<details>
<summary><strong>16. Navedite tri primjera binarne klasifikacije i tri primjera višeklasne klasifikacije. Što su moguće ulazne veličine u model u svakom navedenom primjeru?</strong></summary>

**Binarna klasifikacija**
- spam / nije spam (ulaz: tekst emaila)
- bolest / zdravlje (ulaz: medicinski podaci)
- prevara / normalna transakcija (ulaz: podaci o transakciji)

**Višeklasna klasifikacija**
- prepoznavanje znamenki (0–9)
- klasifikacija vrsta cvijeća
- klasifikacija vrsta dokumenata

Ulazne veličine mogu biti:
- numeričke značajke
- tekst
- značajke slike.

</details>

---
<br>
<br>

<details>
<summary><strong>17. Objasnite logističku regresiju.</strong></summary>

Logistička regresija koristi se za **binarne klasifikacijske probleme**.

Model koristi funkciju:

![alt text](https://github.com/Filz249/Strojno-Ucenje/blob/main/formula3)

Rezultat je vrijednost između 0 i 1 koja predstavlja vjerojatnost pripadnosti klasi.

Ako je vjerojatnost veća od određenog praga (npr. 0.5), primjer se klasificira kao pozitivna klasa.

</details>

---
<br>
<br>

<details>
<summary><strong>18. Objasnite OvR i OvO pristup.</strong></summary>

Kod problema s više klasa koriste se dvije strategije.

**One-vs-Rest (OvR)**  
Za K klasa trenira se K klasifikatora.  
Svaki klasifikator razlikuje jednu klasu od svih ostalih.

**One-vs-One (OvO)**  
Trenira se klasifikator za svaki par klasa.

Broj klasifikatora:

K(K−1)/2

</details>

---
<br>
<br>

<details>
<summary><strong>19. Objasnite matricu zabune.</strong></summary>

Matrica zabune prikazuje rezultate klasifikacije.

Elementi:
- TP – true positive
- TN – true negative
- FP – false positive
- FN – false negative

**Accuracy**

(TP + TN) / (TP + TN + FP + FN)

**Precision**

TP / (TP + FP)

**Recall**

TP / (TP + FN)

**F1**

2 × (precision × recall) / (precision + recall)

</details>

---
<br>
<br>

<details>
<summary><strong>20. Što je precision-recall krivulja i ROC krivulja?</strong></summary>

**Precision-Recall krivulja** prikazuje odnos između preciznosti i odziva za različite pragove klasifikacije.

**ROC krivulja** prikazuje odnos između:
- True Positive Rate
- False Positive Rate

Koristi se za procjenu kvalitete klasifikatora.

</details>

---
<br>
<br>

<details>
<summary><strong>21. Kako se izračunavaju metrike za evaluaciju u slučaju višeklasne klasifikacije?</strong></summary>

Kod višeklasne klasifikacije metrike se računaju za svaku klasu posebno.

Zatim se koriste metode:
- **macro averaging** – prosjek metrika svih klasa
- **micro averaging** – globalni izračun metrika

</details>

---
<br>
<br>

<details>
<summary><strong>22. Objasnite algoritam K najbližih susjeda (KNN).</strong></summary>

KNN je algoritam klasifikacije temeljen na udaljenosti između primjera.

Postupak:
1. izračuna se udaljenost između novog primjera i svih podataka
2. odabere se K najbližih susjeda
3. klasa se određuje većinskim glasovanjem

Najčešća mjera udaljenosti je **Euklidska udaljenost**.

</details>

---
<br>
<br>

<details>
<summary><strong>23. Objasnite stablo odlučivanja.</strong></summary>

Stablo odlučivanja je model koji koristi strukturu stabla.

- unutarnji čvorovi predstavljaju uvjete
- grane predstavljaju odluke
- listovi predstavljaju klasifikaciju ili vrijednost

Prednosti:
- jednostavno za interpretaciju

Nedostatci:
- sklono overfittingu.

</details>

---
<br>
<br>

<details>
<summary><strong>24. Objasnite algoritam K srednjih vrijednosti.</strong></summary>

K-means je algoritam za grupiranje podataka.

Postupak:
1. odabere se broj grupa K
2. inicijaliziraju se centri grupa
3. svaki primjer se dodjeljuje najbližem centru
4. centri se ponovno izračunaju
5. postupak se ponavlja do konvergencije.

</details>

---
<br>
<br>

<details>
<summary><strong>25. Objasnite kvantizaciju boje digitalne slike pomoću algoritma K srednjih vrijednosti.</strong></summary>

Svaki piksel slike ima RGB vrijednosti.

K-means algoritam može grupirati slične boje u K grupa.

Svaki piksel se zamjenjuje bojom centra svoje grupe.

Time se smanjuje broj boja u slici i postiže **kompresija slike**.

</details>

---
<br>
<br>

<details>
<summary><strong>26. Objasnite hijerarhijsko aglomerativno grupiranje.</strong></summary>

Algoritam započinje tako da je svaki podatkovni primjer zasebna grupa.

Zatim se najbliže grupe postupno spajaju.

Rezultat se prikazuje **dendrogramom**.

</details>

---
<br>
<br>

<details>
<summary><strong>27. Što je smanjivanje dimenzionalnosti?</strong></summary>

Smanjivanje dimenzionalnosti je proces smanjenja broja značajki u skupu podataka.

Razlozi:
- brže treniranje
- manje memorije
- uklanjanje redundantnih značajki

Jedna od metoda je **PCA (Principal Component Analysis)**.

</details>

---
<br>
<br>

<details>
<summary><strong>28. Što je umjetni neuron?</strong></summary>

Umjetni neuron prima ulazne vrijednosti, množi ih s težinama i računa zbroj.

z = Σ(wᵢxᵢ) + b

Rezultat se zatim prosljeđuje kroz aktivacijsku funkciju.

</details>

---
<br>
<br>

<details>
<summary><strong>29. Aktivacijske funkcije umjetnog neurona.</strong></summary>

Primjeri:

- Sigmoid
- ReLU
- Tanh
- Softmax

Aktivacijske funkcije uvode nelinearnost u neuronsku mrežu.

</details>

---
<br>
<br>

<details>
<summary><strong>30. Potpuno povezane višeslojne neuronske mreže.</strong></summary>

U potpuno povezanoj mreži svaki neuron jednog sloja povezan je sa svim neuronima sljedećeg sloja.

Sastoji se od:
- ulaznog sloja
- skrivenih slojeva
- izlaznog sloja.

</details>

---
<br>
<br>

<details>
<summary><strong>31. Što je duljina koraka?</strong></summary>

Duljina koraka (learning rate) određuje koliko se parametri mijenjaju tijekom treniranja.

Premala vrijednost:
- sporo treniranje

Prevelika vrijednost:
- nestabilno treniranje.

</details>

---
<br>
<br>

<details>
<summary><strong>32. Osnovni koraci izgradnje neuronske mreže.</strong></summary>

1. priprema podataka  
2. definiranje arhitekture mreže  
3. inicijalizacija parametara  
4. treniranje modela  
5. evaluacija modela.

</details>

---
<br>
<br>

<details>
<summary><strong>33. Early stopping.</strong></summary>

Early stopping je metoda za sprječavanje overfittinga.

Treniranje se zaustavlja kada pogreška na validacijskom skupu počne rasti.

</details>

---
<br>
<br>

<details>
<summary><strong>34. Klasifikacija rukom pisanih znamenki.</strong></summary>

Slike znamenki pretvaraju se u vektore piksela.

Neuronska mreža ima:
- ulazni sloj (pikseli)
- skrivene slojeve
- izlazni sloj s 10 neurona (0–9).

</details>

---
<br>
<br>

<details>
<summary><strong>35. Dropout.</strong></summary>

Dropout je tehnika regularizacije.

Tijekom treniranja nasumično se isključuje dio neurona kako bi se smanjio overfitting.

</details>

---

<br>
<br>

<details>
<summary><strong>36. Što je 2D konvolucija?</strong></summary>

2D konvolucija je operacija filtriranja slike pomoću matrice filtera (kernel).

Filter se pomiče preko slike i računa se zbroj umnožaka piksela i elemenata filtera.

</details>

---
<br>
<br>

<details>
<summary><strong>37. Konvolucijski sloj.</strong></summary>

Konvolucijski sloj primjenjuje više filtera na ulaznu sliku.

**Stride** – korak pomicanja filtera.  
**Padding** – dodavanje nula oko slike.

Broj parametara ovisi o:
- veličini filtera
- broju filtera.

</details>

---
<br>
<br>

<details>
<summary><strong>38. Max pooling.</strong></summary>

Max pooling smanjuje dimenziju podataka.

Za svaki prozor uzima se **maksimalna vrijednost**.

Time se zadržavaju najvažnije značajke.

</details>

---
<br>
<br>

<details>
<summary><strong>39. Što je augmentacija skupa podataka za učenje? Zašto se koristi?</strong></summary>

Augmentacija podataka je tehnika povećanja skupa podataka umjetnim stvaranjem novih primjera.

Primjeri:
- rotacija slike
- zrcaljenje
- pomicanje
- promjena osvjetljenja

Koristi se kako bi se:
- povećala količina podataka
- smanjio overfitting
- poboljšala generalizacija modela.

</details>

---
<br>
<br>

<details>
<summary><strong>40. Što je učenjem prijenosom (transfer learning)?</strong></summary>

Transfer learning je tehnika u kojoj se koristi već trenirani model za novi problem.

Postupak:
1. koristi se model treniran na velikom skupu podataka
2. uklanja se završni sloj
3. dodaje se novi sloj za novi zadatak
4. model se dodatno trenira

Prednost je brže treniranje i potreba za manjim skupom podataka.

</details>

---
<br>
<br>
<br>
<br>
