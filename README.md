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


  

</details>

---
<br>
<br>

<details>
<summary><strong>12. Objasnite postupak procjene parametara linearnog regresijskog modela gradijentnom metodom. Koje su razlike između batch metode, stohastičke metode i mini-batch stohastičke metode?</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>13. Objasnite višedimenzionalnu linearnu regresiju. Navedite primjer.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>14. Objasnite polinomsku regresiju. Objasnite podusklađivanje (underfitting) i pretjerano usklađivanje na podatke (overfitting) na primjeru polinomske regresije.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>15. Što je evaluacija ili vrednovanje izgrađenog modela. Skicirajte princip evaluacije. Navedite metrike za vrednovanje regresijskih modela.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>16. Navedite tri primjera binarne klasifikacije i tri primjera višeklasne klasifikacije. Što su moguće ulazne veličine u model u svakom navedenom primjeru?</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>17. Objasnite logističku regresiju: navedite odgovarajući matematički izraz (model) i skicirajte jednostavan binarni klasifikacijski problem s dvije ulazne veličine te što se dobiva primjenom logističke regresije.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>18. Objasnite OvR i OvO pristup na jednostavnom (2D) problemu s tri klase i dvije ulazne veličine. Koje su prednosti i nedostatci pojedinog pristupa?</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>19. Objasnite matricu zabune. Što predstavlja svaki njen element? Objasnite točnost, preciznost, odziv i F1 mjeru.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>20. Što je preciznost-odziv krivulja i ROC krivulja. Kako ih dobivamo?</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>21. Kako se izračunavaju metrike za evaluaciju u slučaju višeklasne klasifikacije? Pokažite na vlastitom primjeru s tri klase.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>22. Objasnite algoritam K najbližih susjeda (KNN). Kako se najčešće definira mjera udaljenosti? Kako broj susjeda utječe na rezultate KNN algoritma? Koje su prednosti i nedostatci algoritma KNN?</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>23. Objasnite stablo odlučivanja. Skicirajte jednostavan primjer. Navedite koje su prednosti i nedostatci stabla odlučivanja.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>24. Objasnite algoritam K srednjih vrijednosti na jednostavnom problemu s dvije ulazne veličine. Koji su načini inicijalizacije centara? Objasnite princip određivanja optimalnog broja grupa K.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>25. Objasnite kvantizaciju boje digitalne slike pomoću algoritma K srednjih vrijednosti i kako se može postići kompresija slike.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>26. Objasnite hijerarhijsko aglomerativno grupiranje na jednostavnom primjeru s dvije ulazne veličine (značajke). Na koje se sve načine može definirati udaljenost (sličnost) dva primjera ili grupe?</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>27. Što je smanjivanje dimenzionalnosti? Zašto se ono radi? Koja su dva glavna pristupa smanjivanju dimenzionalnosti? Na koji način analiza glavnih komponenti (PCA) radi smanjivanje dimenzionalnosti (načelno)?</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>28. Objasnite što je to umjetni neuron, skicirajte ga i navedite pripadne matematičke izraze.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>29. Navedite i skicirajte minimalno 4 aktivacijske funkcije umjetnog neurona. Koje su prednosti i nedostatci pojedine aktivacijske funkcije?</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>30. Objasnite kakve su to unaprijedne potpuno povezane višeslojne neuronske mreže. Skicirajte jednu takvu mrežu i navedite broj parametara te mreže.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>31. Što je duljina koraka? Kako može utjecati na proces treniranja neuronske mreže? Skicirajte.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>32. Navedite osnovne korake prilikom izgradnje neuronske mreže. Objasnite princip treniranja neuronske mreže.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>33. Objasnite princip sprječavanja pretjeranog usklađivanja na podatke za učenje pomoću ranog zaustavljanja (engl. early stopping).</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>34. Objasnite način predobrade podatkovnih primjera i strukturiranja mreže za problem klasifikacije rukom pisanih znamenki pomoću potpuno povezane neuronske mreže.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>35. Objasnite tehniku nasumičnog izbacivanja neurona tijekom učenja (engl. dropout).</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>36. Što je 2D konvolucija. Objasnite/skicirajte na jednostavnom primjeru filtriranja digitalne slike.</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>37. Što je konvolucijski sloj i zašto se koristi? Skicirajte primjer primjene konvolucijskog sloja na neki ulazni volumen, naznačite ulazne i izlazne dimenzije. Što je stride? Što je padding? O čemu ovisi broj parametara konvolucijskog sloja?</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>38. Što je sloj sažimanja po maksimalnoj vrijednosti (eng. max pooling) i zašto se koristi? Skicirajte primjer primjene ovog sloja na neki volumen, naznačite ulazne i izlazne dimenzije.</strong></summary>
 
</details>

---
<br>
<br>

<details>
<summary><strong>39. Što je augmentacija skupa podataka za učenje? Zašto se koristi?</strong></summary>

</details>

---
<br>
<br>

<details>
<summary><strong>40. Što je učenjem prijenosom (engl. transfer learning) i kako se odvija?</strong></summary>

</details>

---
<br>
<br>
