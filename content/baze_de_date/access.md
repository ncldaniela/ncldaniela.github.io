---
title: "Access"
date: 2018-08-20T03:16:20+03:00
weight: 4
draft: false
---

<html>
  <body>
    <div class="wiki" id="content_view" style="display: block;">
<a href="/files/Microsoft%20Access%202007.ppt">Microsoft Access 2007.ppt</a><br />
<h3 id="toc0"><a name="x--Interogări (Query)"></a><span style="font-family: 'Times New Roman';">Interogări (Query)</span></h3>
 <span style="display: block; font-family: 'Times New Roman'; font-size: medium;"><span style="display: block; text-align: justify;">Interogările reprezintă modalităţi de selecţie şi afişare a informaţie din unul sau mai multe surse (tabele sau alte interogări), formulate cu ajutorul unor condiţii logice. </span></span><br />
<h4 id="toc1"><a name="x--Interogări (Query)-Tipuri de interogări"></a><span style="font-family: 'Times New Roman'; font-size: medium;">Tipuri de interogări</span></h4>
 <span style="display: block; font-family: 'Times New Roman'; font-size: medium;"><span style="display: block; text-align: justify;">În funcţie de modul de definire şi rezultatele acţiunii, interogarile pot fi clasificate astfel:</span><br />
<ol><li>interogări simple sau de selecţie (folosind condiţii logice);</li><li>interogări pentru actualizare - delete query, update query şi append query;</li><li>interogări încrucişate sau bidimensionale.</li></ol><span style="display: block; text-align: justify;">Rezultatul interogării este un nou set de date, numit set dinamic (engl: <em>Dynaset</em>). Setul dinamic (rezultalul interogării) conţine doar câmpurile specificate ale înregistrarilor din tabelele specificate care satisfac condiţiile specificate. Denumirea '"Set dinamic" este legată de faptul că orice modificări ale datelor din tabelele specificate în interogare implică modificări corespunzătoare ale rezultatului interogării (la o nouă executare a ei) şi invers, orice modificări în setul dinamic implică modificări în tabelele respective (cu condiţia respectării integrităţii datelor). Seturile de date dinamice nu se memorează; ele se formează din nou de fiecare dată când executăm o interogare. Dacă în tabelele bazei de date intervin modificări, rezultatele executării a două interogari identice pot fi diferite.</span></span><br />
<h3 id="toc2"><a name="x--Crearea unei interogări simple (de selecţie a înregistrărilor -Select Query)"></a><span style="font-family: 'Times New Roman';">Crearea unei interogări simple (de selecţie a înregistrărilor -Select Query)</span></h3>
 <span style="display: block; font-family: 'Times New Roman'; font-size: medium;"><br />
<span style="display: block; text-align: justify;"> Pentru a defini o interogare de selecţie selectăm opţiunea Queries din fereastra Database, apoi butonul <em>Create query in design view</em>.<br />
<span style="display: block; text-align: center;"><img src="http://www.competentedigitale.ro/access/imagini/cerc52.jpg" alt="external image cerc52.jpg" title="external image cerc52.jpg" style="height: 396px; width: 545px;" /></span><br />
Ca efect, va apărea fereastra alăturată, din care selectăm consecutiv (în orice ordine) tabelele necesare şi pentru fiecare acţionăm butonul <strong>Add</strong>. După selectarea tabelelor / interogărilor acţionăm butonul <strong>Close</strong>.<br />
<span style="display: block; text-align: center;"><img src="http://www.competentedigitale.ro/access/imagini/cerc53.jpg" alt="external image cerc53.jpg" title="external image cerc53.jpg" style="height: 343px; width: 544px;" /></span><br />
În situaţia în care, după ce au fost stabilite sursele care vor fi interogate, dorim să revenim asupra lor şi să le schimbăm, avem la dispoziţie opţiunile meniului Query, cu menţiunea că pentru a înlătura o sursă trebuie mai întâi să o selectăm şi apoi să alegem Remove:</span><br />


<table class="wiki_table">
    <tr>
        <td><img src="http://www.competentedigitale.ro/access/imagini/cerc54.jpg" alt="external image cerc54.jpg" title="external image cerc54.jpg" style="height: 239px; width: 224px;" /><br />
</td>
        <td>sau dăm clic dreapta pe sursă şi alegem Remove:<br />
<img src="http://www.competentedigitale.ro/access/imagini/cerc55.jpg" alt="external image cerc55.jpg" title="external image cerc55.jpg" style="height: 114px; width: 214px;" /><br />
</td>
    </tr>
</table>

<span style="display: block; text-align: justify;">Dacă tabelele au câmpuri comune (definite în procesul creării lor), Access stabileşte în mod automat legăturile respective. În continuare indicăm, în partea de jos a ferestrei, câmpurile din fiecare tabel (în ordinea dorită), care urmează a fi afişate sau pentru care se vor specifica condiţii de selecţie şi / sau de sortare. Includerea câmpurilor se face prin "tragerea" lor cu ajutorul mouse-ului din tabelele din caseta de sus în rândul Field al casetei de jos sau prin executarea unui dublu-clic pe denumirile respective. După aceasta, specificăm condiţiile selecţiei şi / sau ordinea sortării, în acest fel interogarea se consideră definită.<br />
<span style="display: block; text-align: center;"><img src="http://www.competentedigitale.ro/access/imagini/cerc56.jpg" alt="external image cerc56.jpg" title="external image cerc56.jpg" style="height: 321px; width: 320px;" /></span><br />
<span style="display: block; text-align: justify;">În rândul <strong>Criteria</strong> din partea de jos a ferestrei specificăm condiţia selecţiei. Dacă dorim ca înregistrările să fie afişate într-o anumită ordine (crescătoare / alfabetică sau descrescătoare), pentru câmpurile respective specificăm opţiunile Ascending sau Descending în rândul Sort.</span></span><br />
</span><br />
<span style="display: block; text-align: justify;"><a name="1"></a>Interogarea astfel definită poate fi executată imediat în scopul obţinerii rezultatului, sau salvată pentru a fi executată ulterior. În primul caz, actionăm butonul <img src="http://www.competentedigitale.ro/access/imagini/cerc57.jpg" alt="external image cerc57.jpg" title="external image cerc57.jpg" style="height: 18px; width: 20px;" />(<strong>Datasheet View</strong>) din bara cu instrumente sau opţiunea Datasheet View din meniul View, în al doilea caz executăm comanda <strong>Save</strong> din meniul <strong>File</strong>. La salvarea interogării indicăm numele ei, care nu trebuie să coincidă cu numele unor tabele sau ale unor interogări definite anterior.</span><span style="display: block; font-family: 'Times New Roman'; font-size: medium;"><br />
<h4 id="toc3"><a name="x--Crearea unei interogări simple (de selecţie a înregistrărilor -Select Query)-Interogări de acţiune: Delete Query, Update Query şi Append Query"></a>Interogări de acţiune: Delete Query, Update Query şi Append Query</h4>
 <h4 id="toc4"><a name="x--Crearea unei interogări simple (de selecţie a înregistrărilor -Select Query)-Interogari de excludere (ştergere) a unor înregistrări (Delete Query)"></a>Interogari de excludere (ştergere) a unor înregistrări (Delete Query)</h4>
 <ol><li>Creăm interogarea în modul Design View: selectăm Query din fereastra Database şi alegem modul de proiectare Design View.</li><li>Includem tabela pentru care se execută interogarea.</li><li>Selectăm Delete Query din meniul Query. Ca rezultat, titlul ferestrei se schimbă în Delete Query, iar în partea de jos a ferestrei apare rândul Delete.</li><li>Din lista câmpurilor tabelei, care apare afisată în partea de sus a ferestrei, selectăm câmpurile care vor fi afişate în interogaresau pentru care vor fi specificate condiţii de selecţie şi le "tragem" în celulele respective ale liniei Field din partea de jos. Ca rezultat, în celulele respective apare automat, pentru fiecare câmp, opţiunea Where (din engleza - Unde, ín care).</li><li>Introducem în celulele liniei Criteria condiţiile selecţiei (condiţiile pe care trebuie să le îndeplinească înregistrările care vor fi şterse, în dreptul câmpului corespunzător).</li><li>Pentru a obţine lista înregistrărilor care urmează a fi excluse (dar încă n-au fost excluse), vizualizăm interogarea în modul Datasheet View.</li><li>Dacă rezultatele obţinute sunt cele dorite, revenim în modul Design View pentru a elimina realmente înregistrările, selectând comanda Run din meniul Query. Ca rezultat, pe ecran apare un mesaj de informare despre numărul total al inregistrarilor care urmează a fi eliminate. Dacă acţionăm butonul Yes, înregistrările vizate sunt eliminate definitiv. Pentru renunţare, acţionam butonul No.</li><li>Salvăm interogarea.</li></ol><span style="display: block; text-align: justify;">Exemplu:Pentru tabela următoare:<img src="http://www.competentedigitale.ro/access/imagini/cerc_61.jpg" alt="external image cerc_61.jpg" title="external image cerc_61.jpg" style="height: 95px; width: 522px;" /><br />
Eliminarea persoanelor care au studii "Liceale":<img src="http://www.competentedigitale.ro/access/imagini/cerc_62.jpg" alt="external image cerc_62.jpg" title="external image cerc_62.jpg" style="height: 79px; width: 409px;" /></span><br />
<h4 id="toc5"><a name="x--Crearea unei interogări simple (de selecţie a înregistrărilor -Select Query)-Interogări de actualizare a înregistrărilor (Update Query)"></a>Interogări de actualizare a înregistrărilor (Update Query)</h4>
 <span style="display: block; text-align: justify;">Se utilizează în cazul în care este necesară modificarea unui număr mare de înregistrari, respectând aceeaşi modalitate de modificare. Vom descrie în continuare modul de definire a unei interogări de actualizare.</span><br />
<ol><li>Creăm interogarea în modul Design View: selectăm Query din fereastra Database şi alegem modul de proiectare Design View.</li><li>Includem tabela pentru care se execută interogarea.</li><li>Selectăm Update Query din meniul Query. Ca rezultat, titlul ferestrei se modifică în Update Query, iar în partea de jos apare rândul Update To.</li><li>Includem (prin tragere) în celulele rândului Field câmpurile care dorim să apară în interogare sau cele pentru care vom stabili criterii de actualizare.</li><li>Pentru ca anumite câmpuri ale tabelei să fie afişate în interogarea de actualizare trebuie să introducem în rândul Update To numele câmpului cuprins între paranteze drepte, altfel acesta nu va fi afişat. De asemenea, putem completa automat un câmp calculat, care nu a fost completat iniţial în tabelă. De exemplu, dacă avem tabela Medii, care are câmpurile: Numele şi prenumele elevului, Media sem I, Media Sem II şi Media generală, iar câmpul Media generală nu a fost completat iniţial pentru nici o înregistrare, vom trece în dreptul câmpului Media generală de pe rândul Update: ([Media sem I]+[Media sem II])/2.<br />
<img src="http://www.competentedigitale.ro/access/imagini/cerc_63.jpg" alt="external image cerc_63.jpg" title="external image cerc_63.jpg" style="height: 78px; width: 475px;" /></li><li>Introducem în rândul Criteria condiţia pe care trebuie să o îndeplinească înregistrările care vor fi modificate.</li><li>Vizualizăm interogarea în modul Datasheet View pentru a vedea modificările care se vor face. Modificările propriu-zise vor fi operate numai la revenirea în modul Design View şi executarea comenzii Run din meniul Query. ín acest caz, pe ecran va apărea un mesaj despre numarul total al înregistrărilor care urmează a fi modificate. Acţionând butonul Yes, Access va efectua modificările. Pentru a renunţa la modificări, acţionăm butonul No .</li></ol><span style="display: block; text-align: justify;">Observaţie: Interogarile de tip Update se execută, de regulă, o singură dată. ín cazul executării repetate a interogării, de exemplu aplicarea unei scumpiri de 2% la pretul unor produse, această majorare va fi realizată la fiecare execuţie a interogării.</span><br />
<h4 id="toc6"><a name="x--Crearea unei interogări simple (de selecţie a înregistrărilor -Select Query)-Interogări de adăugare a înregistrărilor (Append Query)"></a>Interogări de adăugare a înregistrărilor (Append Query)</h4>
 <span style="display: block; text-align: justify;">Se utilizează în cazul în care este necesară adăugareavunui set de înregistrări dintr-o tabelă în altă tabelă. Aceasta va selecta datele care tebuie adăugate şi le va trimite în câmpurile tabelei destinaţie. Vom descrie în continuare modul de definire a unei interogări de adăugare.</span><br />
<ol><li>Creăm interogarea în modul Design View: selectăm Query din fereastra Database şi alegem modul de proiectare Design View.</li><li>Includem tabela pentru care se execută interogarea.</li><li>Includem (prin "tragere") în celulele rândului Field câmpurile care dorim să apară în interogare sau cele pentru care vom stabili criterii de adăugare.</li><li>Selectăm Append Query din meniul Query. Indicăm tabela destinaţie.<br />
<img src="http://www.competentedigitale.ro/access/imagini/cerc65.jpg" alt="external image cerc65.jpg" title="external image cerc65.jpg" style="height: 189px; width: 475px;" /><br />
Ca rezultat, titlul ferestrei se modifică în Append Query, iar în partea de jos apare rândul Append To.</li><li>Introducem în rândul Criteria condiţia pe care trebuie să o îndeplinească înregistrările care vor fi preluate.</li><li>Precizăm pe linia Append To numele câmpului destinaţie (doar în cazul în care nu au acelaşi nume).</li><li>Vizualizăm interogarea în modul Datasheet View pentru a vedea modificările care se vor face. Modificările propriu-zise vor fi operate numai la revenirea în modul Design View şi executarea comenzii Run din meniul Query.</li></ol><span style="display: block; text-align: center;"><img src="http://www.competentedigitale.ro/access/imagini/cerc64.jpg" alt="external image cerc64.jpg" title="external image cerc64.jpg" style="height: 320px; width: 425px;" /></span><br />
<h1 id="toc7"><a name="Interogari Access"></a><span style="color: #939346; font-size: 19px;"><u><span style="font-family: 'Times New Roman'; font-size: 12pt;">Interogari Access</span></u></span></h1>
 <br />
<span style="background-color: #ffffff; color: #333333; display: block; font-family: Arial; font-size: 11px;"><span style="color: #000000; display: block; text-align: justify;"> Performantele unui SGBD depind în mare masura de capacitatea extragerii rapide a diferitor informatii în forma dorita. În multe cazuri este necesar de a selecta date din mai multe tabele simultan. De exemplu, pentru a selecta cartile din domeniul informaticii editate în Franta dupa anul 2001, utilizam 3 tabele: CĂRŢI, ŢĂRI si TEMATICI. Pentru a formula conditii de selectie, în MS Access exista o clasa speciala de obiecte (alaturi de tabel )numite <em>Interogari</em> (engl. <em>Queries).</em></span><span style="display: block; text-align: justify;"><em><span style="color: #000000;">nime: Interogari - Cereri - Interpelari.</span></em><strong><em><span style="color: #000000;">Interogarile</span></em></strong> <span style="color: #000000;">reprezinta modalitati de selectie si afisare a informatie din unu sau mai multe tabele, formulate cu ajutorul unor conditii logice.</span><strong><span style="color: #000000;">Tipuri de interogari</span></strong></span><br />
<span style="color: #000000; display: block; text-align: justify;"> În functie de modul de definire si rezultatele actiunii, interogarile pot fi clasificate astfel:<br />
a) <em>interogari de selectie</em> (folosind conditii logice);<br />
b) <em>interogari de sortare</em> (indicînd cîmpul/cîmpurile si ordinea sortarii);<br />
c) <em>interogari de excludere a unor înregistrari din BD</em> (de exemplu,<span style="line-height: 1.5;">excluderea tuturor cititorilor care nu au împrumutat carti în ultimii 2 ani);</span><br />
d<em>) interogari de modificare a unor înregistrari din BD</em> (de exemplu,<span style="line-height: 1.5;">majorarea preturilor tuturor car&amp;# 14114g616o 355;ilor cu 20%);</span><br />
e) <em>interogari de obtinerea a unor informatii rezultante</em> (în cîmpuri noi)<span style="line-height: 1.5;">în baza informatiei existente (de exemplu, obtinerea vîrstei cititorului prin scaderea anului de nastere din anul curent);</span><br />
f) <em>interogari de obtinere a unor totaluri, medii</em> etc.;<br />
g) <em>interogari încrucisate.</em><br />
În toate cazurile, cu exceptia ultimelor doua, rezultatul interogarii este un nou set de date, numit <em>set dinamic</em> (engl: <em>Dynaset). Setul dinamic</em> (rezultalul interogarii) contine doar cîmpurile specificate ale înregistrarilor din tabelele specificate care satisfac conditiilor specificate. Denumirea <em>'"Set dinamic"</em> este legata de faptul ca orice modificari ale datelor din tabelele specificate în interogare implica modificari respective ale rezultatului interogarii (la o noua executare a ei). si invers, orice modificari în setul dinamic implica modificari în tabelele respective (cu conditia respectarii integritatii datelor). Seturile dinamice nu se memorizeaza; ele se formeaza din nou de fiecare data cînd executam o interogare. Dac în tabelele BD intervin modificari, rezultatele executarii a doua interogari identice pot fi diferite, în cele ce urmeaza vom descrie modalitatile de definire si executare a interogarilor nominalizate.</span><br />
<span style="display: block; text-align: justify;"> <strong><span style="color: #000000;"> Interogari de selectie a înregistrarilor<em>(Select Query)</em></span></strong></span><span style="color: #000000; display: block; text-align: justify;">Exemplu:1Pentru a defini o interogare de selectie (de exemplu, afisarea emisiunilor cu desene animate), actionam fila <em>Queries</em> din fereastra <em>Database</em> (fig. 10), apoi butonul <em>New.</em></span><span style="display: block; text-align: justify;"><img src="http://www.scritub.com//files/informatica/access/16_poze/image002.jpg" alt="external image image002.jpg" title="external image image002.jpg" style="height: 255px; width: 420px;" /></span><br />
<br />
<span style="color: #000000; display: block; text-align: justify;"> fig.10 Fereastra cu clasele de obiecte Access<br />
<br />
În continuare indicam unul din cele 5 moduri de creare a interogarilor (în cazul nostru <em>Design View</em>)<br />
Din caseta care apare (fig. 11) selectam consecutiv (în orice ordine) tabelele necesare (în cazul nostru,Emisiuni,Genuri,Canale TV) si pentru fiecare actionam butonul <em>Add.</em></span><br />
<span style="display: block; text-align: justify;"> <img src="http://www.scritub.com//files/informatica/access/16_poze/image004.jpg" alt="external image image004.jpg" title="external image image004.jpg" style="height: 267px; width: 348px;" /></span><br />
<span style="color: #000000; display: block; text-align: justify;"> fig.11 Selectarea tabelelor pentru definirea interogarii<br />
Dupa selectarea tabelelor actionam butonul <em>Close.</em> Daca tabelele au cîmpuri comune (definite în procesul crearii lor), Access stabileste în mod automat legaturile respective (fig. 12). În continuare indicam, în partea de jos a ferestrei, cîmpurile din fiecare tabel (în ordinea dorita) care urmeaza a fi afisate sau pentru care se vor specifica conditii de selectie si/sau de sortare. Includerea cîmpurilor se face prin "tragerea" lor cu ajutorul mouse-ului din tabelele din caseta de sus în rîndul <em>Field</em> al casetei de jos sau prin executarea unui dublu-clic pe denumirile respective. Dupa aceasta specificam conditiile selectiei si/sauordinea sortarii, în acest fel interogarea se considera definita (fig. 12).</span><br />
<br />
<span style="display: block; text-align: justify;"> <img src="http://www.scritub.com//files/informatica/access/16_poze/image006.jpg" alt="external image image006.jpg" title="external image image006.jpg" style="height: 318px; width: 516px;" /></span><br />
<span style="color: #000000; display: block; text-align: justify;"> fig12.Specificarea conditiilor de selectie<br />
În rîndul Criteria din partea de jos a ferestrei specificam conditia selectiei Des* pentru cîmpul DenGen al tabelului Genuri. Daca dorim ca înregistrarile sa fie afisate într-o anumita ordine (crescatoare/alfabetica sau descrescatoare) pentru cîmpul respective specificam optiunile Ascending sau Descending în rîndul sort. Daca indicam Ascending pentru cîmpul DenEmisiunii al tabelului emisiuni denumirile emisiunilor vor fi afisate în ordenea alfabetica.<br />
Interogarea astfel definita poate fi executata imediat în scopul obtinerii rezultatului (fig. 13), sau salvata pentru a fi executata ulterior. În primul caz actionam butonul <img src="http://www.scritub.com//files/informatica/access/16_poze/image008.jpg" alt="external image image008.jpg" title="external image image008.jpg" style="height: 19px; width: 16px;" /> (Datasheet View) din bara cu instrumente în aldoile caz executam comanda Save din meniul File. La salvarea interogarii indicam numele ei, care nu trebuie sa coincida cu numele unor tabele sau ale unor interogari definite anterior. Setul dinamic (rezultatele interogarii) contine cîmpurile marcate cu simbolul <img src="http://www.scritub.com//files/informatica/access/16_poze/image010.jpg" alt="external image image010.jpg" title="external image image010.jpg" style="height: 14px; width: 11px;" /> în rîndul Show al ferestrei. Celelalte cîmpuri chiar daca sunt incluse în interogare, nu se afiseaza.<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image012.jpg" alt="external image image012.jpg" title="external image image012.jpg" style="height: 159px; width: 488px;" /><br />
fig.13 Rezultatele interogarii<br />
<br />
<br />
Exemplu 2. Lista emisiunilor cu durata mai mica de 30 de minute.<br />
<br />
Pentru afisarea emisiunilor cu durata mai mica de 30 minute actionam fila Queries din fereastra Database , apoi butonul New. În continuare indicam unul din cele 5 moduri de creare a interogarilor, în cazul nostru Design View (fig.14).<br />
<br />
fig.14<br />
<br />
Din caseta care apare (fig.15) selectam tabelul Emisiuni,Canale TV si Genuri si actionam butonul Add.<br />
<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image016.jpg" alt="external image image016.jpg" title="external image image016.jpg" style="height: 239px; width: 577px;" /><br />
fig.15<br />
<br />
Dupa selectarea tabelului actionam butonul Close. Apoi executam dublu clic pe denumirile câmpurilor si vor trece în rîndul Field din caseta de jos (fig.16).<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image018.jpg" alt="external image image018.jpg" title="external image image018.jpg" style="height: 245px; width: 450px;" /><br />
fig.16<br />
Dupa aceasta specificam conditiile selectiei. În rîndul Criteria scrim conditia <30 pentru câmpul Durata Emisiunii al tabelului Emisiuni si ne va afisa lista emisiunilor cu durata mai mica de 30 minute.<br />
<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image020.jpg" alt="external image image020.jpg" title="external image image020.jpg" style="height: 149px; width: 414px;" /><br />
fig.17. Rezultatul interogarii<br />
<br />
Exempul 3: Lista emisiunilor stiri<br />
Pentru afisarea emisiunilor stiri actionam fila Queries din fereastra Database , apoi butonul New. În continuare indicam unul din cele 5 moduri de creare a interogarilor, în cazul nostru Design View (fig.14).<br />
Din caseta care apare (fig.15) selectam tabelul Emisiuni , Genuri actionam butonul Add .Dupa selectarea tabelului actionam butonul Close.<br />
Apoi executam dublu clic pe denumirile câmpurilor si vor trece în rîndul Field din caseta de jos (fig.18).<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image022.jpg" alt="external image image022.jpg" title="external image image022.jpg" style="height: 232px; width: 324px;" /><br />
fig.18<br />
<br />
Dupa aceasta specificam conditiile selectiei. În rîndul Criteria scrim conditia "stiri" pentru câmpul DenGen al tabelului Genuri si ne va afisa lista emisiunilor stiri.<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image024.jpg" alt="external image image024.jpg" title="external image image024.jpg" style="height: 183px; width: 337px;" /><br />
fig.19. Rezultatul interogarii<br />
<br />
Exemplul 4: Lista emisiunilor în limba rusa<br />
Fie ca dorim sa afisam lista emisiunilor în limba rusa. Pentru aceasta executam urmatorii pasi:<br />
Definim o interogare în care includem tabelele Emisiuni, Limbi, Canale TV din care selectam câmpurile DenEmisiunii, DenCanal, DenLimba (fig.20)<br />
<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image026.jpg" alt="external image image026.jpg" title="external image image026.jpg" style="height: 255px; width: 400px;" /><br />
fig.20<br />
Dupa aceasta specificam criteriul de selectie în rîndul Criteria pentru câmpul DenLimba din tabelul Limbi si ne va afisa lista emisiunilor în limba rusa.<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image028.jpg" alt="external image image028.jpg" title="external image image028.jpg" style="height: 192px; width: 313px;" /><br />
fig.21<br />
<br />
<strong>Interogari de sortare a înregistrarilor</strong><br />
<br />
Dupa ce am definit conditiile de selectie, putem stabili conditii de sortare pentru unul sau mai multe câmpuri.<br />
<strong>Exemplu 1:</strong> Pentru afisarea emisiunilor în ordine alfabetica executam un clic în rîndul <em>Sort</em> al casetei (fig.22) în dreptul câmpului DenEmisiuni si din lista derulanta alegem optiunea Ascending.<br />
<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image030.jpg" alt="external image image030.jpg" title="external image image030.jpg" style="height: 270px; width: 582px;" /><br />
fig.22<br />
<br />
Pentru a afisa rezultatul interogarii (fig.23), actionam butonul <img src="http://www.scritub.com//files/informatica/access/16_poze/image008.jpg" alt="external image image008.jpg" title="external image image008.jpg" style="height: 19px; width: 16px;" /> (Datasheet View) din bara cu instrumente.<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image032.jpg" alt="external image image032.jpg" title="external image image032.jpg" style="height: 296px; width: 480px;" /><br />
fig.23<br />
<br />
Sortarea datelor poate fi facuta si fara a specifica conditii de selectie. În acest caz se vor afisa toate înregistrarile, dar ordinea lor va corespunde conditiilor stabilite în rîndul <em>Sort</em> pentru câmpurile respective.</span><br />
<br />
<span style="display: block; text-align: justify;"> <strong><span style="color: #000000;">Exemplu 2</span></strong><span style="color: #000000;">: Lista emisiunilor în ordinea duratei lor.</span></span><br />
<br />
<span style="color: #000000; display: block; text-align: justify;"> Pentru afisarea emisiunilor în ordine duratei lor executam un clic în rîndul <em>Sort</em> al casetei (fig.24) în dreptul câmpului Durata emisiunii si din lista derulanta alegem optiunea Ascending.<br />
<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image034.jpg" alt="external image image034.jpg" title="external image image034.jpg" style="height: 270px; width: 565px;" /><br />
fig.24<br />
Pentru a afisa rezultatul interogarii (fig.25), actionam butonul <img src="http://www.scritub.com//files/informatica/access/16_poze/image008.jpg" alt="external image image008.jpg" title="external image image008.jpg" style="height: 19px; width: 16px;" /> (Datasheet View) din bara cu instrumente.<br />
<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image036.jpg" alt="external image image036.jpg" title="external image image036.jpg" style="height: 273px; width: 444px;" /><br />
fig.25</span><br />
<span style="display: block; text-align: justify;"> <strong><span style="color: #000000;"> Interogari de actualizare a înregistrarilor (Update Query)</span></strong></span><br />
<span style="color: #000000; display: block; text-align: justify;"> În cazul cînd este necesar de a modifica un numar mare de înregistrari conform unuia si aceluiasi algoritm, putem defini o interogare de modificare (<em>Update Query</em>)<br />
Vom descrie în continuare modul de definire a unei interogari pentru care stirile se maresc cu 5 minute.<br />
1. Definim interogarea în modul descris în p.5.1.<br />
2. Includem tabelul <strong>Emisiuni</strong> si <strong>Genuri.</strong><br />
3. Selectam <em>Update</em> din meniul <strong>Query</strong> sau actionam butonul din bara de instrumente.Ca rezultat titlul ferestrei se modifica în <em>Update Query,</em> iar în partea de jos apare rîndul <em>Update To</em> (fig.26).<br />
<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image038.jpg" alt="external image image038.jpg" title="external image image038.jpg" style="height: 262px; width: 409px;" /><br />
fig.26<br />
<br />
4. Includem (prin "tragere") în celulele rîndului <em>Field</em> câmpurile <em>DenEmisiunii, DenGen, Durata emisiunii.</em><br />
5. Introducem în rîndul <em>Update To</em> pentru câmpul <em>DenEmisiunii</em> expresia <em>[DenEmisiunii], DenGen</em> expresia <em>[DenGen],</em> <em>Durata emisiunii</em> expresia <em>[Durata emisiunii]+5</em><br />
6. Introducem în rîndul <em>Criteria</em> pentru câmpul <em>DenGen</em> conditia <em>Stiri</em>.<br />
7. Actionam butonul <img src="http://www.scritub.com//files/informatica/access/16_poze/image008.jpg" alt="external image image008.jpg" title="external image image008.jpg" style="height: 19px; width: 16px;" /> din bara cu instrumente, pentru a obtine valorile curente ale câmpului <em>Durata emisiunii</em> care urmeaza a fi modificate (fig.27).<br />
<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image040.jpg" alt="external image image040.jpg" title="external image image040.jpg" style="height: 172px; width: 338px;" /><br />
fig.27<br />
<br />
Modificarile propriu-zise vor fi operate numai dupa trecerea în regimul <strong>Design View</strong> si actionarea butonului din bara cu instrumente sau executarea comenzii <strong>Run</strong> din meniul <strong>Query</strong>. În acest caz pe ecran va aparea un mesaj despre numarul total al înregistrarilor care urmeaza a fi modificate. Actionînd butonul <em>Yes</em> , Access va efectua modificarile (fig.28). Pentru a renunta la modificari, actionam butonul <em>No</em> .<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image042.jpg" alt="external image image042.jpg" title="external image image042.jpg" style="height: 163px; width: 313px;" /></span><br />
<span style="display: block; text-align: justify;"> fig.28<br />
<strong><span style="color: #000000;">Remarca:</span></strong><span style="color: #000000;"> <em>Interogarile de tip <strong>Update</strong> se executa de regula o singura data. În cazul executarii repetate a interogarii definite în exemplul de mai sus, vom obtine de fiecare data marirea emisiunilor stiri cu 5 minute.</em></span><br />
<br />
<strong><span style="color: #000000;"> Interogari de excludere a înregistrarilor (Delete Query)</span></strong></span><br />
<span style="color: #000000; display: block; text-align: justify;"> Fie, de exemplu, ca dorim sa excludem din tabelul <strong>Emisiuni</strong> toate emisiunile între ora 1000 -1200. Pentru aceasta, executam urmatoarele actiuni:<br />
1. Definim interogarea în modul descris în p 5.1.<br />
2. Includem tabelul <strong>Emisiuni</strong>.<br />
3. Selectam <strong><em>Delete</em></strong> <em><strong>Query</strong></em> din meniul <strong><em>Query</em></strong> sau actionam butonul<br />
<br />
(daca este afisat) din bara cu instrumente. Ca rezultat, titlul ferestrei se<br />
<br />
schimaг în <em>Delete Query</em> iar în partea de jos a ferestrei apare rîndul <em>Delete.</em><br />
4. Din lista cîmpurilor tabelului <strong>Emisiuni,</strong> afisata în partea de sus a ferestrei (fig. 8.12), selectam câmpurile care vor fi afisate sau pentru care vor fi specificate conditii de selectie <em>DenEmisiunii</em> si <em>Timpul începerii</em> si le "tragem" în celulele respective ale rîndului <em>Field</em> din partea de jos. Ca rezultat, în celulele respective pentru fiecare câmp apare optiunea<br />
Where (din engleza - <em>Unde, In care).</em><br />
5. Introducem în celulele rîndului <em>Criteria</em> conditiile selectiei. În cazul nostru pentru cîmpul <em>Timpul începerii</em> scriem conditia <em>Between</em> 1000 <em>And</em> 1200.<br />
<br />
<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image044.jpg" alt="external image image044.jpg" title="external image image044.jpg" style="height: 265px; width: 468px;" /><br />
fig.29<br />
6. Pentru a obtine lista înregistrarilor care urmeaza a fi excluse (dar înca n-au fost excluse), actionam butonul <img src="http://www.scritub.com//files/informatica/access/16_poze/image008.jpg" alt="external image image008.jpg" title="external image image008.jpg" style="height: 19px; width: 16px;" /> <em>(Datasheet View)</em> din bara cuinstrumente. Ca rezultat, obtinem fereastra, reprezentata în figura 8.13.<br />
<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image046.jpg" alt="external image image046.jpg" title="external image image046.jpg" style="height: 121px; width: 321px;" /><br />
fig.30<br />
7. Daca rezultatele obtinute în p.6 sunt cele dorite, revenind la regimul<em>Design View,</em> putem elimina realmente înregistrarile, executînd comanda <strong><em>Run</em></strong> din meniul <strong><em>Query</em></strong> sau actionînd butonul <em>(Run)</em> din bara cu instrumente. Ca rezultat, pe ecran apare un mesaj despre numarul total al înregistrarilor care urmeaza a fi eliminate. Daca actionam butonul <em>Yes,</em> înregistrarile vizate sunt eliminate definitiv. Pentru renuntare, actionam butonul <em>No.</em><br />
8. Salvam interogarea, executînd comanda <strong><em>Save</em></strong> <strong><em>As</em></strong> din meniul <em>File s</em>i<br />
<br />
indicînd numele interoga<br />
<br />
<br />
<strong>Interogari de grupare si totalizare a înregistrarilor</strong><br />
<br />
În multe cazuri apare necesitatea de a obtine valori rezumative referitoare la toate înregistrarile din tabel sau pentru o submultime a lor. De exemplu, ar putea sa ne intereseze cîte emisiuni de fiecare gen sunt. În acest scop în Access pot fi definite interogari în care sunt specificate conditii de grupare si totalizare.<br />
Pentru obtinerea valorilor rezumative, sunt prevazute urmatoarele functii:</span><br />
<span style="display: block; text-align: justify;"> <strong><span style="color: #000000;">-Sum,</span></strong> <span style="color: #000000;">pentru calcularea sumei valorilor cîmpului;</span><br />
<strong><span style="color: #000000;">-<em>Avg,</em></span></strong> <span style="color: #000000;">pentru calcularea mediei valorilor cîmpului;</span></span><br />
<span style="color: #000000; display: block; text-align: justify;"> -<strong>Min</strong>, pentru gasirea valorii minime;<br />
-<strong>Max</strong>, pentru gasirea valorii maxime;</span><br />
<span style="display: block; text-align: justify;"> <strong><em><span style="color: #000000;">-</span></em></strong><strong><span style="color: #000000;">Count<em>,</em> </span></strong><span style="color: #000000;">calculeaza numarul de valori ale cîmpului (excluzînd cele vide);</span><br />
<strong><span style="color: #000000;">-StDev</span></strong><em><span style="color: #000000;">, </span></em><span style="color: #000000;">pentru calcularea abatem standard;</span><br />
<strong><span style="color: #000000;">-Var</span></strong><em><span style="color: #000000;">, </span></em><span style="color: #000000;">pentru calcularea dispersiei.</span></span><br />
<span style="color: #000000; display: block; text-align: justify;"> Valorile rezumative pot fi obtinute atît pentru toate înregistrarile din tabel cît si pentru grupuri de înregistrari.<br />
Fie ca dorim sa obtinem informatii despre cîte emisiuni de fiecare gen sunt. Pentru aceasta executam urmatoarele actiuni:<br />
1. Definim o interogare în care includem tabelele Emisiuni si Genuri din care selectam cîmpurile DenGen si DenEmisiunii (fig)<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image048.jpg" alt="external image image048.jpg" title="external image image048.jpg" style="height: 260px; width: 268px;" /><br />
fig.31</span><br />
<span style="display: block; text-align: justify;"> <strong><span style="color: #000000;">2. </span></strong><span style="color: #000000;">Selectam optiunea <em>Totals</em> din meniul View; ca rezultat în caseta de jos apare rîndul <em>Total,</em> iar în celulele respective ale cîmpurilor selectate optiunea Group By<br />
3. Din lista derulanta a cîmpului DenEmisiunii (rîndul <em>Total)</em> selectam optiunea <em>Cou</em></span><em><span style="color: #000000;">nt.</span></em></span><span style="color: #000000; display: block; text-align: justify;">4. Actionam butonul <img src="http://www.scritub.com//files/informatica/access/16_poze/image008.jpg" alt="external image image008.jpg" title="external image image008.jpg" style="height: 19px; width: 16px;" /> pentru a obtine valorile cautate (fig)<br />
<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image050.jpg" alt="external image image050.jpg" title="external image image050.jpg" style="height: 171px; width: 280px;" /><br />
fig.32</span><br />
<span style="display: block; text-align: justify;"><strong><span style="color: #000000;"> Interogari încrucisate (Crosstab Query)</span></strong></span><br />
<span style="color: #000000; display: block; text-align: justify;"> In multe cazuri rezultatele unei interogari sunt greu de perceput din cauza volumului mare de informatii selectate. In figura sunt prezentate datele despre cîte emisiuni de fiecare gen sunt, obtinute cu ajutorul unei interogari de grupare si totalizare.<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image050.jpg" alt="external image image050.jpg" title="external image image050.jpg" style="height: 171px; width: 280px;" /><br />
fig<br />
Access permite gruparea si reprezentarea datelor într-o forma compacta, forma care se aseamana cu un tabel electronic.În acest scop se definesc interogari speciale, numite interogari încrucisate (<em>Crosstab Query</em>).<br />
Pentru a defini o interogare încrucisata procedam initial ca în cazul unei interogari de selectie obisnuita, adica selectam tabelele <strong>Emisiuni, Canale TV, Genuri,</strong> din care selectam câmpurile <em>DenGen, DenCanal, DenEmisiunii</em> (fig)<br />
<img src="http://www.scritub.com//files/informatica/access/16_poze/image052.jpg" alt="external image image052.jpg" title="external image image052.jpg" style="height: 275px; width: 408px;" /><br />
fig<br />
În continuare parcurgem urmatorii pasi:<br />
1. Selectam optiunea <strong><em>Crosstab</em></strong> din meniul <strong><em>Query.</em></strong> Ca rezultat, titlul ferestrei<br />
<br />
se schimba în <em>Crosstab Query,</em> iar în partea de jos apare rîndul <em>Crosstab.</em><br />
2. Definim câmpul <em>DenGen,</em> valorile caruia vor servi în calitate de denumiri ale rîndurilor tabelului<em>.</em> Pentru aceasta actionam butonul cu sageata din rîndul<em>Crosstab</em> pentru câmpul <em>DenGen</em> si din lista derulanta care apare selectam optiunea <em>Row Heading.</em><br />
3. In mod analogic definim câmpul <em>DenCanal</em>, valorile caruia vor servi în calitate de denumiri ale coloanelor tabelului <em>.</em> Pentru aceasta actionam butonul cu sageata din rîndul <em>Crosstab</em> pentru câmpul <em>DenCanal</em> si din lista derulanta care apare selectam optiunea <em>Column Heading.</em><br />
4. În rîndul <em>Total</em> înlocuim optiunea <em>Group By</em> din câmpul <em>DenEmisiunii</em> prin<br />
<br />
operatorul <em>Count.</em><br />
5. Pentru câmpul <em>DenEmisiunii</em> în rîndul <em>Crosstab</em> stabilim optiunea <em>Value</em> pe<br />
<br />
care o selectam din lista derulanta prin analogie cu actiunile descrise mai sus.<br />
6. Actionam butonul <img src="http://www.scritub.com//files/informatica/access/16_poze/image008.jpg" alt="external image image008.jpg" title="external image image008.jpg" style="height: 19px; width: 16px;" /> pentru vizualizarea rezultatelor (fig)</span><br />
<br />
<span style="display: block; text-align: justify;"> <img src="http://www.scritub.com//files/informatica/access/16_poze/image054.jpg" alt="external image image054.jpg" title="external image image054.jpg" style="height: 171px; width: 502px;" /></span></span><br />
<br />
</span>
    </div>
  </body>
</html>