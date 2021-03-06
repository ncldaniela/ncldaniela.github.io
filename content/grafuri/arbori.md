---
title: "Arbori"
date: 2018-08-20T03:16:20+03:00
weight: 7
draft: false
---

<html>
  <body>
    <div class="wiki" id="content_view" style="display: block;">
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">Fie un graf neorientat <em>G</em>=(<em>V</em>,<em>U</em>), unde <em>V</em> e mulțimea vârfurilor, iar <em>U</em> cea a muchiilor sale. Următoarele afirmații sunt echivalente:</span><br />
<span style="display: block; text-align: justify;"><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">1. G</span></em><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> este arbore.</span></em></span><br />
<span style="display: block; text-align: justify;"><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">2. G</span></em><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> este un graf conex minimal („minimal” se numește proprietatea unui graf, că dacă i se elimină orice muchie, se obține un graf neconex).</span></em></span><br />
<span style="display: block; text-align: justify;"><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">3. G</span></em><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> este un graf fără cicluri maximal („maximal” se numește proprietatea unui graf, că dacă i se adaugă orice muchie, se obține un graf care are măcar un ciclu, și deci nu e arbore).</span></em></span><br />
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">Un arbore cu <em>n</em> ≥ 2 vârfuri conține cel puțin două vârfuri terminale. Orice arbore cu <em>n</em> vârfuri are <em>n</em>-1 muchii.</span><br />
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">Un <strong><em>arbore</em></strong> este o structura ramificata formata dintr-un nod A (radacina) si un numar finit de arbori (subarbori) ai lui A.</span><br />
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">- orice nod din arbore este radacina pentru un subarbore iar orice arbore poate deveni subarbore;</span><br />
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">- doi subarbori pot fi în relatie <em>de incluziune</em>, când un subarbore este inclus în celalalt sau <em>de excluziune</em>, când nu au noduri comune.</span><br />
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">Definitii:</span><br />
<span style="display: block; text-align: justify;"><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">nod </span></em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">= punct în care se întâlnesc doi subarbori;</span></span><br />
<span style="display: block; text-align: justify;"><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">nivel </span></em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">= numarul de noduri parcurse de la radacina pâna la un nod;</span></span><br />
<span style="display: block; text-align: justify;"><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">r</span></em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">a<em>d</em>a<em>cin</em>a = nivel 1;</span></span><br />
<span style="display: block; text-align: justify;"><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">descendent </span></em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">= primul nod al unui subarbore;</span></span><br />
<span style="display: block; text-align: justify;"><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">nod terminal </span></em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">= nod fara descendenti;</span></span><br />
<span style="display: block; text-align: justify;"><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">în</span></em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">a<em>l</em>t<em>imea unui arbore</em> = numarul maxim de niveluri;</span></span><br />
<strong><em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">arbore binar </span></em><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">= arbore în care toate nodurile au maximum 2 descendenti</span></strong><br />
<span style="display: block; font-size: 70%; text-align: justify;">Dacă avem în vedere faptul că un arbore binar este un arbore, care înainte de toate este un graf, putem spune că printre metodele de reprezentare a arborilor binari se numără şi metodele de reprezentare a grafurilor, cum ar fi:</span><br />
<span style="display: block; font-size: 70%; line-height: 1.5; text-align: justify;">-reprezentarea prin matricea de adiacenţă;</span><span style="display: block; font-size: 70%; line-height: 1.5; text-align: justify;">-reprezentarea prin listele de adiacenţă;</span><span style="display: block; font-size: 70%; line-height: 1.5; text-align: justify;">-reprezentarea prin şirul muchiilor;</span><span style="display: block; font-size: 70%; line-height: 1.5; text-align: justify;">Modalităţile de reprezentare specifice arborilor binari sunt:</span><span style="display: block; font-size: 70%; line-height: 1.5; text-align: justify;">1.cu ajutorul vectorilor</span><span style="display: block; font-size: 70%; line-height: 1.5; text-align: justify;">2.folosind alocarea dinamică</span><br />
<span style="font-size: 130%;">Se numeşte arbore binar complet un arbore binar în fiecare nod, care nu este frunză, are exact doi descendenţi.</span><br />
<span style="font-size: 130%;">Propoziţie:Un arbore binar complet care are p noduri terminale, toate situate pe acelaşi nivel, are în total 2p-1 noduri.</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"><a title="View Parcurgerea arborilor binari on Scribd" href="http://www.scribd.com/doc/82538401/Parcurgerea-arborilor-binari?secret_password=17xxh5a5rrxrs5s8rwnh" style="margin: 12px auto 6px auto; font-family: Helvetica,Arial,Sans-serif; font-style: normal; font-variant: normal; font-weight: normal; font-size: 14px; line-height: normal; font-size-adjust: none; font-stretch: normal; -x-system-font: none; display: block; text-decoration: underline;" rel="nofollow">Parcurgerea arborilor binari</a><iframe class="scribd_iframe_embed" src="http://www.scribd.com/embeds/82538401/content?start_page=1&amp;view_mode=list&amp;access_key=key-x1b5d83m53kl5lavr36&amp;secret_password=17xxh5a5rrxrs5s8rwnh" data-auto-height="true" data-aspect-ratio="0.772727272727273" scrolling="no" id="doc_3463" width="100%" height="600" frameborder="0" name="doc_3463"></iframe></span><br />
<strong><span style="color: #008000;">ARBORI GENERALIZATI/BINARI</span></strong><br />
<a class="wiki_link_ext" href="http://bigfoot.cs.upt.ro/~chirila/teaching/upt/lectures/2id-aa/AA-ID-Cap08-1.pdf" rel="nofollow">http://bigfoot.cs.upt.ro/~chirila/teaching/upt/lectures/2id-aa/AA-ID-Cap08-1.pdf</a><br />
<span style="color: #008000; font-size: 150%;">Vezi</span><br />
<br />
<a class="wiki_link_ext" href="http://informaticasite.ro/probleme-rezolvate-c++/arbori/" rel="nofollow">http://informaticasite.ro/probleme-rezolvate-c++/arbori/</a><br />
<h1 id="toc0"><a name="Probleme propuse"></a><span style="color: #008000; font-family: 'Times New Roman','serif'; font-size: 16px;">Probleme propuse</span></h1>
 <h2 id="toc1"><a name="Probleme propuse-file:test_grafuri_neorientate1.docx"></a><a href="/files/test_grafuri_neorientate1.docx">test_grafuri_neorientate1.docx</a></h2>
 <a href="/files/test_grafuri_neorientate2.docx">test_grafuri_neorientate2.docx</a><br />
<a href="/files/test_grafuri_neorientate3.docx">test_grafuri_neorientate3.docx</a><br />
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">1. Elevii unei clase stau in banca cate doi sau cate unul singur. Cand este nevoie sa se faca un anunt urgent la sfarsit de saptamana sau in vacanta, ei au stabilit un sistem prin care un elev va anunta pe altii doi care sunt colegi de banca, sau pe unul singur, daca nu are coleg de banca (exista si elevi care nu vor da telefoane mai departe). Stiind ca doamna diriginta face primul anunt (anunta doi elevi care sunt colegi de banca) si apoi fiecare elev isi anunta alti doi colegi de banca (sau unul sau niciunul) de clasa si asa mai departe, se cere sa se scrie un program care realizeaza urmatoarele:</span><br />
<br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;">a) memorarea datelor intr-un arbore binar alocat in heap. Un elev inexistent se va marca cu * <a href="/files/ARBORE.cxx">ARBORE.cxx</a></span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> b) numara si afiseaza din cati elevi este formata clasa</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> c) afiseaza numele tuturor elevilor din clasa</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> d) sa se determine daca un elev face parte din clasa</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> e) sa se afiseze elevii anuntati de diriginta</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> f) sa se afiseze cologii de banca (perechi)</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> g) numara cati elevi au acelasi nume cu un nume dat de la tastatura</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> h) afiseaza numele elevilor care nu mai au de anuntat pe nimeni</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> i) sa se afiseze colegul de banca al lui Gigel (sau un nume citit de la tastatura)</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> j) cine ar fi trebuit sa il anunte pe Dan (sau un nume citit de la tastatura)</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> k) sa se afiseze elevii care stau in stanga in banci</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> l) elevul x si elevul y isi schimba locurile. Sa se afiseze.</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> m) cate banci sunt ocupate de un singur elev</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> n) cate banci sunt ocupate de doi elevi</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;">o) cate banci sunt ocupate</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;">2. Un arbore binar retine numere intregi.</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> a) sa se afiseze numerele utilizand una dintre metode.</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> b) sa se afiseze numerele pare din arbore</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> c) sa se determine cel mai mare numar din arbore</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> d) sa se determine suma cifrelor tuturor numerelor din arbore</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> e) afisati frunzele</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> f) sa se determine daca exista o anumita valoare in arbore</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> g) sa se determine daca arborele contine numere prime</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> h) sa se genereze oglinditul arborelui</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> i) sa se afiseze subordonatii stangi</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> j) sa se inlocuiasca o cheie cu o alta</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> k) sa se inverseze doua chei</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> l) sa se afiseze fratele lui x</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> m) sa se afiseze tatal lui x</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> n) sa se afiseze fii (fiul) lui x</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> o) sa se determine minimul din arbore</span><br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> p) sa se afiseze nodurile cu un singur subordonat</span><br />
<br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;">2. Fie un arbore binar memorat prin vectorii stang si drept. Sa se parcurga arborele prin cele trei metode.</span><br />
<br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;">3. Fiind dat un arbore binar memorat in heap, sa se genereze un nou arbore binar identic cu primul.</span><br />
<br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> 4. Fie un arbore binar memora in heap. </span><br />
<br />
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">a) Sa se afiseze cate niveluri are arborele</span><br />
<br />
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">b) Sa se afiseze nodurile de pe nivelul x</span><br />
<br />
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">c) sa se afiseze nodurile pe niveluri</span><br />
<br />
<span style="display: block; text-align: justify;"><span style="font-family: 'Times New Roman','serif'; font-size: 16px;">d)</span><span style="font-family: 'Times New Roman','serif';"> Calculati si afisati suma nodurilor de pe un nivel dat</span></span><br />
<br />
<span style="display: block; font-family: 'Times New Roman',serif; text-align: justify;">e) sa se afisese frunzele care nu se gasesc pe ultimul nivel</span><br />
<br />
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">5.Un arbore binar retine caractere.</span><br />
<br />
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">a) sa se determine cate vocale retine arborele</span><br />
<span style="display: block; font-family: 'Times New Roman',serif; font-size: 16px; text-align: justify;">b) se citeste un sir de caractere de la tastatura. Sa se determine daca sirul citit este egal cu sirul determinat de parcurgerea arborelui (svd, vsd sau sdv).</span><br />
<br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> 6. Fie un graf orientat memorat prin matricea de adiacenta. Sa se determine daca graful poate fi arbore binar. In caz afirmativ , pentru o solutie oarecare, sa se parcurga svd.</span><br />
<br />
<span style="font-family: 'Times New Roman','serif'; font-size: 16px;"> 7. Fie un arbore binar. Sa se completeze arborele astfel incat fiecare nod sa aiba 2 subordonati. Valoarea cu care se face completarea se citeste de la tastatura.</span><br />
<br />
8. Fie un arbore binar cu n noduri numerotate de la 1 la n cu radacina 1, in care cheia fiecarui nod este un numar intreg. Numarul de noduri se citeste de la tastatura. Reprezentarea in memorie se face inlantuit cu referinte descendente astfel: pe fiecare dintre cele n randuri ale fisierului text arbore.in se afla cate trei numere intregi, separate prin cate un spatiu reprezentand fiul stang, fiul drept si valoarea cheii fiecarui nod al arborelui. Sa se scrie cate un program C++ pentru fiecare dintre<br />
<br />
cerintele de mai jos:<br />
<br />
a) sa se afiseze nodurile care retin informatiile numere pare;<br />
<br />
b) sa se afiseze nodurile care au doar descendent stang;<br />
<br />
c) sa se afiseze cheile nodurilor care au doar descendent drept;<br />
<br />
d) sa se afiseze cheile din nodurile terminale;<br />
<br />
e) sa se afiseze fiii nodului x, furnizat de utilizator;<br />
<br />
f) sa se afiseze nodul tata al unui nod x, furnizat de utilizator;<br />
<br />
g) sa se scrie in fisierul noduri.out, nodurile ale caror chei sunt egale cu o valoare val,<br />
<br />
citita de la tastatura;<br />
<br />
h) sa se calculeze inaltimea arborelui binar dat;<br />
<br />
i) sa se determine nivelul maxim;<br />
<br />
j) sa se afiseze cheia maxima.
    </div>
  </body>
</html>