---
title: "Subprograme"
date: 2018-08-20T03:16:20+03:00
weight: 6
draft: false
---

<html>
  <body>
    <div class="wiki" id="content_view" style="display: block;">
<strong>PREZENTARE TEORETICA</strong><br />
<h1 id="toc0"><a name="x1. Introducere"></a><strong>1. Introducere</strong></h1>
 <span style="display: block; text-align: justify;"><strong>Subprogramele</strong> sunt părţi ale unui program, identificabile prin nume, care se pot activa la cerere prin intermediul acestor nume.Prezenţa subprogramelor implică funcţionarea în strânsă legătură a două noţiuni: <strong>definiţia</strong> unui subprogram şi <strong>apelul</strong> unui subprogram.<strong>Definiţia unui subprogram</strong> reprezintă de fapt descrierea unui proces de calcul cu ajutorul variabilelor virtuale (parametri formali) iar <strong>apelul</strong> unui subprogram nu este altceva decât execuţia procesului de calcul pentru cazuri concrete (cu ajutorul parametrilor reali, (efectivi, actuali) ).<strong>2. Structura unui subprogram C++</strong>Un subprogram (funcţie) are <em>o <strong>definiţie</strong></em> şi atâtea <strong><em>apeluri</em></strong> câte sunt necesare.</span><br />
<strong><em>Definiţia unei funcţii are forma generală:</em></strong><br />
<br />
<strong><span style="color: #ff0000;">tip_returnat nume_funcţie (lista parametrilor formali)</span></strong><br />
<strong><span style="color: #ff0000;">{</span></strong><br />
<strong><span style="color: #ff0000;">instrucţiune; // corpul funcţiei</span></strong><br />
<strong><span style="color: #ff0000;">}</span></strong><br />


<table class="wiki_table">
    <tr>
        <td style="text-align: left;"><strong>Tip_returnat</strong><br />
</td>
        <td><span style="display: block; text-align: justify;">Reprezintă tipul rezultatului calculat şi returnat de funcţie şi poate fi: <strong>int, char, char*, long, float, void, etc.</strong></span><br />
<br />
<span style="display: block; text-align: justify;">În cazul în care tipul rezultatului este <strong>diferit de void</strong>, corpul funcţiei trebuie să conţină cel puţin o instrucţiune <strong>return</strong>.</span><br />
<span style="display: block; text-align: justify;">Înstrucţiunea return va specifica valoarea calculată şi returnată de funcţie care trebuie să fie de acelaşi tip ca şi <strong>tip_returnat.</strong></span><br />
</td>
    </tr>
    <tr>
        <td><strong>Nume_funcţie</strong><br />
</td>
        <td><span style="display: block; text-align: justify;">Reprezintă numele dat funcţiei de către cel ce o defineşte, pentru a o putea apela.</span><br />
</td>
    </tr>
    <tr>
        <td><strong>Lista_parametrilor_formali</strong><br />
</td>
        <td><span style="display: block; text-align: justify;">Reprezintă o listă de declaraţii de variabile separate prin virgulă. Această listă poate să fie şi vidă.</span><br />
</td>
    </tr>
    <tr>
        <td><strong>Instrucţiune</strong><br />
</td>
        <td><span style="display: block; text-align: justify;">Este o instrucţiune vidă, simplă sau compusă.</span><br />
</td>
    </tr>
</table>

<br />
<br />
<h1 id="toc1"><a name="x3. Apelul unei funcţii . Revenirea dintr-o funcţie"></a><a name="x3. Apelul unei funcţii . Revenirea dintr-o funcţie"></a><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">3. Apelul unei funcţii . Revenirea dintr-o funcţie</span></strong></h1>
 <h1 id="toc2"> </h1>
 <span style="font-family: 'Times New Roman',serif; font-size: 16px;">3.1 Apelul <strong>unei</strong> funcţii care nu returnează o valoare are forma generală:</span><br />
<br />
<span style="display: block; text-align: center;"><strong><span style="color: #ff0000; font-size: 16px;">nume_funcţie (lista parametrilor efectivi);</span></strong></span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">unde:</span><br />
<ul><li><span style="font-family: 'Times New Roman',serif; font-size: 16px;">parametru efectiv = parametru actual = parametru real = parametru de apel </span></li><li><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">lista parametrilor efectivi = </span></strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">poate fi vidă, poate fi o expresie sau mai multe despărţite prin virgulă</span></li></ul><br />
<strong>Efectul instructiunii de apel este:</strong><br />
<ul><li>crearea tabelei de parametrii actuali;</li><li>crearea variabilelor locale functiei;</li><li>executarea corpului de instructiuni al functiei;</li><li><span style="color: #ff0000;">desfintarea tabelei de parametrii si a variabilelor locale;</span></li><li>revenirea la instruciunea urmatoare din program</li></ul><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">O funcţie care returnează o valoare </span></strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">poate fi apelată fie printr-o instrucţiune de apel simplă (cazul funcţiilor care nu returnează valori) şi în plus poate fi apelată ca operand al unei expresii. În cazul în care funcţia se apelază print-o instrucţiune de apel simplă, rezultatul funcţiei se pierde.</span><br />
<br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">Când funcţia se apelează ca operand, valoarea returnată va fi utilizată în expresie. </span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">La apelul unei funcţii, valorile parametrilor efectivi se atribuie parametrilor formali corespunzători. În cazul în care unul din tipul unui paramatru efectiv diferă de tipul parametrului formal corespunzător, parametrul efectiv va fi convertit spre parametru formal (dacă este posibil, altfel compilatorul generează eroare). </span><br />
<strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">În momentul în care se întâlneşte un apel de funcţie</span></strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">, controlul execuţiei programul este transferat primei instrucţiuni din funcţie, urmând a se executa secvenţial instrucţiunile funcţiei.</span><br />
<strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Revenirea </span></strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">dintr-o funcţie se face în unul din următoarele cazuri: </span><br />
<ul><li><span style="font-family: 'Times New Roman',serif; font-size: 16px;">după execuţia ultimei instrucţiuni din corpul funcţiei </span></li><li><span style="font-family: 'Times New Roman',serif; font-size: 16px;">la întâlnirea unei instrucţiuni <strong>return</strong> </span></li></ul><span style="display: block; text-align: left;"><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Instrucţiunea return </span></strong></span><br />
are formatele:<br />
<br />
<ul><li><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">return ; </span></strong></li><li><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">return expresie ; </span></strong></li></ul><br />


<table class="wiki_table">
    <tr>
        <td><span style="display: block; text-align: left;"><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Exemplul 3.1 </span></strong></span><br />
</td>
        <td><span style="display: block; text-align: left;"><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Exemplul 3.2 </span></strong></span><br />
</td>
    </tr>
    <tr>
        <td><ol><li>include <iostream></li></ol>using namespace std;<br />
void f1 ()<br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">cout << "abc";</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int main ()</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;"> f1();</span><br />
}<br />
</td>
        <td>#include <iostream><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">using namespace std;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">void f1 (int k)</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">for (int i=1; i<=k ; i++)</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">cout << "abc"<< " ";</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
int main ()<br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">f1(5);</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
</td>
    </tr>
    <tr>
        <td>Se va afisa:abc<br />
</td>
        <td>Se va afişa:abc abc abc abc abc<br />
</td>
    </tr>
    <tr>
        <td>Funcţia nu returnează o valoareFuncţia nu are parametriApelul funcţiei este o instrucţiune de apel simplă<br />
</td>
        <td>Funcţia nu returnează o valoareFuncţia are un parametru formal de tip intApelul funcţiei este o instrucţiune de apel simplă şi se face cu ajutorul unui parametru actual care este de acelaşi tip cu tipul parametrului formal corespunzător<br />
</td>
    </tr>
</table>

<br />


<table class="wiki_table">
    <tr>
        <td><span style="display: block; text-align: left;"><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Exemplul 3.3 </span></strong></span><br />
</td>
        <td><span style="display: block; text-align: left;"><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Exemplul 3.4 </span></strong></span><br />
</td>
    </tr>
    <tr>
        <td>#include <iostream><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">using namespace std;</span><br />
<em><span style="font-family: 'Times New Roman',serif; font-size: 16px;">int prim (int x)</span></em><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{int nr_div;</span><br />
<span style="font-family: "Times New Roman",serif; font-size: 16px;">nr_div=0;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">for (int i=2; i<=x/2; i++)</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">if (x%i==0)</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">nr_div++;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">if (nr_div==0)</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">return 1;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">else</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">return 0;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
<strong>int main ()</strong><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{int N;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">cout << "N="; cin >> N;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">if (prim(N))</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">cout << "PRIM";</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">else</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">cout << "NU E PRIM";</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
</td>
        <td>include <iostream><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">using namespace std;</span><br />
<em><span style="font-family: 'Times New Roman',serif; font-size: 16px;">int prim (int x)</span></em><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{int i;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;"> for ( i=2; i<=x/2; i++)</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;"> if (x%i==0)</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;"> return 0;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;"> return 1;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
<strong>int main ()</strong><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{int N;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;"> cout << "N="; cin >> N;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;"> if (prim(N))</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;"> cout << "PRIM";</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;"> else</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;"> cout << "NU E PRIM";</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
</td>
    </tr>
    <tr>
        <td><span style="display: block; text-align: left;"><em><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Funcţia returnează o valoare de tip int </span></em><em><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Funcţia are un parametru formal de tip int </span></em><em><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Rezultatul funcţiei este este utilizat în cadrul unei expresii.</span></em></span><br />
</td>
        <td><em><span style="font-family: 'Times New Roman',serif; font-size: 16px;"> În cazul în care se întâlneşte un divizor a lui x se execută instrucţiunea return 0. Astfel apelul funcţiei se încheie. </span></em><br />
<em><span style="font-family: 'Times New Roman',serif; font-size: 16px;"> Dacă x este număr prim, instrucţiunea return 0 nu se execută niciodată şi în acest caz, după terminarea execuţiei instrucţiunii for, se execută instrucţiunea return 1 (care determină încheierea execuţiei funcţiei).</span></em><br />
</td>
    </tr>
</table>

<span style="font-family: 'Times New Roman',serif; font-size: 16px;">OBS: În cazul în care <strong>tipul returnat de funcţie lipseşte</strong> din definiţia funcţiei, acesta este implicit </span><br />
<strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;"> int </span></strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">şi nu <strong>void.</strong></span><br />


<table class="wiki_table">
    <tr>
        <td><strong>Exemplul 3.5</strong><br />
</td>
        <td><strong>Exemplul 3.6</strong><br />
</td>
        <td><strong>Exemplul 3.7</strong><br />
</td>
    </tr>
    <tr>
        <td>#include <iostream><br />
using namespace std;<br />
p( )<br />
{<br />
cout << " abcd";<br />
}<br />
int main ()<br />
{<br />
cout << p();<br />
}<br />
</td>
        <td>#include <iostream><br />
using namespace std;<br />
p( )<br />
{<br />
return 25;<br />
}<br />
int main ()<br />
{<br />
cout << p( );<br />
}<br />
</td>
        <td>#include <iostream><br />
using namespace std;<br />
void p( )<br />
{<br />
cout << "void";<br />
}<br />
int main ()<br />
{<br />
cout << p();<br />
}<br />
</td>
    </tr>
    <tr>
        <td>Compilatorul generează eroare deoarece lipseste tipul returnat de functie<br />
</td>
        <td>Compilatorul generează eroare deoarece lipseste tipul returnat de functie<br />
</td>
        <td><span style="color: #ff0000; display: block; text-align: justify;">Compilatorul generează eroare deoarece o functie cu tipul returnat</span><span style="display: block; text-align: justify;"><strong><span style="color: #ff0000;">void</span></strong></span><span style="color: #ff0000; display: block; text-align: justify;">nu se poate apela in cadrul unei functii, in cazul de fata cout</span><br />
</td>
    </tr>
    <tr>
        <td><br />
</td>
        <td>#include <iostream><br />
using namespace std;<br />
<span style="color: #ff0000;">int</span> p( )<br />
{<br />
return 25;<br />
}<br />
int main ()<br />
{<br />
cout << p( );<br />
}<br />
</td>
        <td>#include <iostream><br />
using namespace std;<br />
void p( )<br />
{<br />
cout << "abcd";<br />
}<br />
int main ()<br />
{<br />
p();<br />
}<br />
</td>
    </tr>
    <tr>
        <td><br />
</td>
        <td><span style="font-size: 14.6667px;">Se afişează 25 </span><br />
</td>
        <td><span style="font-size: 14.6667px;">Se afişează abcd</span><br />
</td>
    </tr>
</table>

<h1 id="toc3"><a name="x4. Prototipul unei funcţii"></a><a name="x4. Prototipul unei funcţii"></a><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">4. Prototipul unei funcţii </span></strong></h1>
 <span style="font-family: 'Times New Roman',serif; font-size: 16px;">Pentru a apela o funcţie, aceasta trebuie initial definită. Astfel apelul unei funcţii trebuie precedat de definiţia funcţiei respective. </span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">O a doua posibilitate de apelare a funcţiei constă în scrierea prototipului funcţiei înainte ca acesta să fie apelată. </span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">Prototipul funcţiei conţine informaţii asemănătoare cu cele din antetul funcţiei. Pot lipsi numele parametrilor formali (contează doar tipul şi ordinea acestora), în plus acesta este urmat de “;”. </span><br />
<strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Exemplul 4.1.</span></strong><br />


<table class="wiki_table">
    <tr>
        <td><span style="font-family: 'Times New Roman',serif; font-size: 16px;"># include <iostream></span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">using namespace std;</span><br />
<br />
<strong><span style="color: #ff0000; font-family: 'Times New Roman',serif; font-size: 16px;">int max (int, int);</span></strong><br />
<br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int main ()</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;"> cout << max(10, 20);</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
<br />
<strong><span style="color: #548dd4; font-family: 'Times New Roman',serif; font-size: 16px;">int max (int a, int b)</span></strong><br />
<strong><span style="color: #00b050; font-family: 'Times New Roman',serif; font-size: 16px;">{</span></strong><br />
<strong><span style="color: #00b050; font-family: 'Times New Roman',serif; font-size: 16px;"> if (a>b)</span></strong><br />
<strong><span style="color: #00b050; font-family: 'Times New Roman',serif; font-size: 16px;"> return a;</span></strong><br />
<strong><span style="color: #00b050; font-family: 'Times New Roman',serif; font-size: 16px;"> else</span></strong><br />
<strong><span style="color: #00b050; font-family: 'Times New Roman',serif; font-size: 16px;"> return b;</span></strong><br />
<strong><span style="color: #00b050; font-family: 'Times New Roman',serif; font-size: 16px;">}</span></strong><br />
</td>
        <td><span style="color: #ff0000; font-family: 'Times New Roman',serif; font-size: 16px;">PROTOTIPUL FUNŢIEI </span><br />
<br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">APELUL FUNCŢIEI</span><br />
<br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">DEFINIŢIA FUNCŢIEI </span><br />
<strong><span style="color: #548dd4; font-family: 'Times New Roman',serif; font-size: 16px;">antetul funcţiei </span></strong><br />
<br />
<strong><span style="color: #00b050; font-family: 'Times New Roman',serif; font-size: 16px;">corpul functiei</span></strong><br />
</td>
    </tr>
</table>

<strong><span style="font-family: 'Times New Roman',serif; font-size: 21.3333px;">5. Variabile locale şi variabile globale </span></strong><br />
<strong><span style="font-family: 'Times New Roman',serif; font-size: 18.6667px;">5.1 . Funcţia main</span></strong><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">În C++ funcţia </span><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">main</span></strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;"> determină prima instrucţiune pe care o va executa programul. Aceasta este unica diferenţă dintre main şi celelalte funcţii. Din acest motiv se poate spune că “orice se poate face în main se poate face şi în celelalte funcţii”.</span><br />
<strong><span style="font-family: 'Times New Roman',serif; font-size: 18.6667px;">5.2. Variabile locale </span></strong><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">La fel cum se declară variabilele în cadrul funcţiei main, la fel se pot declara varibile si în cadrul celorlalte funcţii. Aceste variabile se numesc <strong>locale</strong> şi sunt accesibile doar in funcţia in care au fost declarate.</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">In cadrul unei funcţii se pot apela şi alte funcţii, cu conditia ca acestea sa fi fost definite înaintea eventualului apel sau este prezent un prototip de funcţie înaintea funcţiei apelate </span><br />
<span style="display: block; text-align: left;"><strong><span style="font-family: 'Times New Roman',serif; font-size: 18.6667px;">5.3. Variabile globale </span></strong></span><br />
<strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Variabilele globale </span></strong><br />
sunt declarate în afara oricărei funcţii şi sunt vizibile (pot fi utilizate) în tot programul (în programul principal şi în subprograme) din momentul declarării lor.<br />
<br />


<table class="wiki_table">
    <tr>
        <td><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Exemplul 5.1 </span></strong><br />
</td>
        <td><span style="display: block; text-align: left;"><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Exemplul 5.2 </span></strong></span><br />
</td>
        <td><span style="display: block; text-align: left;"><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Exemplul 5.3 </span></strong></span><br />
</td>
    </tr>
    <tr>
        <td><ol><li>include <iostream></li></ol><span style="font-family: 'Times New Roman',serif; font-size: 16px;">using namespace std;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int N;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">void f1()</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int x=5;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">N=10;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">cout << endl<<N;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">cout << endl << x;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int main ()</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">N=4;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">cout << N;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">f1();</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
</td>
        <td><ol><li>include <iostream></li></ol><span style="font-family: 'Times New Roman',serif; font-size: 16px;">using namespace std;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int N;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">void f1()</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int x=5;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">cout << endl << x;</span><br />
<span style="color: #ff0000; font-family: 'Times New Roman',serif; font-size: 16px;">P=2; </span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
int P=9;<br />
int main ()<br />
{f1();<br />
cout << x;<br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">P=7; </span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
</td>
        <td><ol><li>include <iostream></li></ol><span style="font-family: 'Times New Roman',serif; font-size: 16px;">using namespace std;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int N;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">void f1(int p)</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int x=p;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">cout << x;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int main ()</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">f1(77);</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
</td>
    </tr>
    <tr>
        <td><span style="font-family: 'Times New Roman',serif; font-size: 16px;">N este variabilă globală si poate fi accesată în cadrul oricărei funcţii. </span><br />
<br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">x este variabilă locală, vizibilă doar în cadrul funcţiei f1() </span><br />
<br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">Se va afişa: </span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">4 </span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">10 </span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">5 </span><br />
</td>
        <td><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Compilatorul generează eroare deoarece </span><br />
<ul><li><em><span style="font-family: 'Times New Roman',serif; font-size: 16px;">funcţia main încearcă să acceseze variabila locala x care este vizibilă doar în funcţia f1(). </span></em></li><li><em><span style="color: #ff0000; font-family: 'Times New Roman',serif; font-size: 16px;">variabila P este accesată în f1() înainte de a fi </span></em><em><span style="color: #ff0000; font-family: 'Times New Roman',serif; font-size: 16px;">declarată.</span></em></li></ul></td>
        <td><em><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Se afişează 77 </span></em><br />
<br />
<em><span style="font-family: 'Times New Roman',serif; font-size: 16px;">N este variabilă globală. Poate fi accesată în cadrul oricărei funcţii. </span></em><br />
<em><span style="font-family: 'Times New Roman',serif; font-size: 16px;">x este variabilă locală. Poate fi accesată doar în cadrul funcţiei f1() </span></em><br />
<em><span style="font-family: 'Times New Roman',serif; font-size: 16px;">p este parametru formal. Poate fi accesat doar în f1(). </span></em><br />
</td>
    </tr>
</table>

<strong><span style="font-size: 21.3333px;">5.4. Regula de omonimie </span></strong><br />
În cazul în care există o variabilă locală care are acelaşi nume cu o variabilă globală, aceste două variabile se numesc <strong>variabile omonime</strong>.<br />
Variabilele locale sunt prioritare (ascund) variabilele globale omonime.<br />


<table class="wiki_table">
    <tr>
        <td colspan="2"><strong>Exemplul 5.4</strong><br />
</td>
    </tr>
    <tr>
        <td><ol><li>include <iostream></li></ol>using namespace std;<br />
int N=10;<br />
void f1()<br />
{<br />
int N=2;<br />
cout << N<<" ";<br />
}<br />
int main ()<br />
{<br />
f1();<br />
cout << N;<br />
}<br />
</td>
        <td>Variabila N este definită atât ca variabilă globală cât şi ca variabilă locală în f1().<br />
Se va afisa: 2 10<br />
Funcţia f1() acţionează asupra variabilei locale N.<br />
Funcţia main() acţionează supra variabilei globale N.<br />
</td>
    </tr>
</table>

<br />
<strong>Întrebare</strong>. Cum gestionează compilatorul cele două variabile omonime ?<br />
<strong>Răspuns:</strong><br />
<span style="display: block; text-align: justify;">Variabilelor <strong>globale</strong> li se rezervă spaţiu de memorie la începutul execuţiei programului, într-o zonă de memorie numită “zonă de date”. Acest spaţiu va fi ocupat până la încheierea execuţiei programului.</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">Variabilelor <strong>locale</strong> li se rezervă spaţiu într-o zonă specială de memorie numită <strong>“stiva”.</strong> La încheierea execuţiei subprogramului, conţinutul stivei este eliberat. Din acest motiv, variabilele locale sunt vizibile doar în interiorul subprogramului în care au fost declarate.</span><br />
<strong><span style="font-family: 'Times New Roman',serif; font-size: 21.3333px;">6. Parametrii formali şi parametrii actuali </span></strong><br />
<strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Parametrii formali </span></strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">apar în antetul subprogramului şi sunt utilizaţi de subprogram pentru descrierea abstractă a unui proces de calcul . </span><br />
<strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Parametrii actuali </span></strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">apar în instrucţiunea de apelare a uni subprogram şi sunt folosiţi la execuţia unui proces de calcul pentru valori concrete. </span><br />
Parametrii formali nu sunt variabile. O variabilă este caracterizată de nume, tip, şi adresă. Legarea unui parametru formal la o adresă se realizează în timpul execuţiei instrucţiunii de apelare a subprogramului.<br />
<strong><span style="font-family: 'Times New Roman',serif; font-size: 21.3333px;">7. Apel prin valoare şi apel prin referinţă</span></strong><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">Există două tipuri de apel al subprogramelor: </span><br />
<ul><li><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Apel prin valoare </span></strong></li><li><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Apel prin referinţă </span></strong></li></ul><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">7.1. Apel prin valoare </span></strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">– se transmite o copie a parametrului actual. </span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">Valorile transmise la apelul unui subprogram sunt memorate în stivă. Datorită faptului că, după terminarea execuţiei unui subprogram, stiva este eliberată, în cazul apelului prin valoare parametrul actual <strong>nu se modifică (se operează asupra unei copii a parametrului efectiv)</strong> </span><br />
<span style="color: #ff0000; font-size: 16px;"><strong>Parametrii transmisi prin valoare</strong> se pot modifica in corpul functiei dar dupa terminarea apelului functiei <strong>au aceasi valoare</strong> pe care au avut-o inainte de apel.</span><br />
Se utilizează atunci când dorim ca subprogramul să lucreze cu acea valoare, dar să nu poată modifica parametrul efectiv corespunzător din blocul apelator.<br />
<br />
<u><span style="font-family: 'Times New Roman',serif;">Se pot transmite prin valoare:</span></u><br />
<strong><span style="font-family: 'Times New Roman',serif;">a)Valorile reţinute de variabile</span></strong>. În acest caz parametrii efectivi trebuie să fie numele variabilelor.<br />
<br />
<span style="font-family: 'Times New Roman',serif;"> Exemplu:</span><br />

```c++
#include <iostream.h>
void test(int n) {
  n++;
  cout << n << endl;  // tipăreşte n=8
}
void main() {
  int n = 7;
  test(n);
  cout << n << endl;  // tipăreşte n=7
}
```
Parametrul n este transmis prin valoare. În funcţia main() acest parametru este iniţializat cu valoarea 7. Când apelăm funcţia test(), se rezervă spaţiu pe stivă, spaţiu care are numele parametrului formal (în acest caz, tot n) şi care este iniţializat cu valoarea memorată de variabila n a programului principal. Altfel spus, pe stivă se copie valoarea parametrului efectiv de apel. În funcţie, variabila n (care este locală acestei funcţii) este incrementată şi devine 8, valoare care va fi tipărită. La ieşirea din funcţie, variabila n din stivă se pierde, adică nu mai are spaţiu alocat, prin urmare valoarea 8 este pierdută. În main() se tipăreşte valoarea variabilei n (locală acesteia) care are valoarea 7.<br />
Se observă că, în momentul apelului funcţiei test(), pe stivă sunt alocate două variabile cu acelaşi nume n. Prima variabilă este variabila locală funcţiei main() care se salvează pe stivă în momentul apelului pentru a putea reface contextul funcţiei main() după încheierea apelului. A doua variabilă este parametrul formal tip valoare n, vizibil numai în funcţia test() şi iniţializat în momentul apelului cu valoarea 7. Indiferent ce valori primeşte acest n în corpul funcţiei test(), după încheierea execuţiei acestei funcţii, spaţiul său este de alocat din stivă, adică variabila respectivă este distrusă. Din acest motiv, după execuţia funcţiei test(), conţinutul stivei este cel din dreapta. Se reface contextul din care s-a lansat apelul funcţiei test(), adică se recuperează din stivă valoarea variabilei locale n=7 şi adresa de revenire, adică adresa instrucţiunii cout.<br />
<span style="font-size: 9pt;"><strong>b)</strong> </span><strong>Expresii.</strong> În acest caz, parametrii efectivi sunt expresii, care pot conţine şi funcţii şi care mai întâi se evaluează. Exemplu:<br />

```c++
#include <iostream.h>
#include <math.h>

void test(int n) {
  cout << n << endl; 
}

void main() {
  test(5);                  // se va tipări 5
  test(7 + (int)sqrt(45));  // se va tipări 13
}
```

<span style="display: block; text-align: justify;">În funcţie se creează o variabilă numită</span><span style="display: block; text-align: justify;">n</span><span style="display: block; text-align: justify;">, reţinută pe stivă, care la primul apel va primi valoarea 5 şi la al doilea apel valoarea 13.</span><br />
<span style="display: block; text-align: justify;">La ieşirea din funcţie conţinutul acestei variabile se pierde.</span><br />
<span style="display: block; text-align: justify;"><em>Transmiterea parametrilor prin valoare</em></span><span style="display: block; text-align: justify;">se utilizează când nu dorim ca subprogramul apelat să poată modifica parametrii efectivi de apel. Acesta este modul implicit de transmitere a parametrilor în limbajul C. Dacă nu ar exista decât transmiterea prin valoare, ar fi imposibil să modificăm valoarea anumitor valori care sunt declarate în blocul apelator.</span><br />
<br />
<br />
<strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">7.2. Apel prin referinţă </span></strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">- se transmite adresa parametrului actual.</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">În cazul apelului prin referinţă, subprogramul, cunoscând adresa parametrului actual, <strong>acţionează direct asupra locaţiei de memorie</strong> indicată de aceasta, <strong>modificând</strong> valoarea parametrului actual. </span><br />
<span style="color: #ff0000; font-size: 16px;"><strong>Parametrii transmisi prin referinta</strong> se folosesc pentru transmiterea de rezultate in afara functiei. Ei se pot modifica in corpul functiei dar dupa terminarea apelului functiei au valoarea pe care au primit-o in timpul apelului functiei.</span><br />
În C++, implicit, apelul se face prin valoare. Pentru a specifica un apel prin referinţă, în lista parametrilor formali, numele parametrului formal va trebui precedat de <strong><span style="color: #ff0000; font-size: 16px;">simbolul &amp;</span></strong><br />
<br />


<table class="wiki_table">
    <tr>
        <td>#include <iostream><br />
using namespace std;<br />
int a,b;<br />
void afis<span style="color: #ff0000;">(int a, int b)</span><br />
{<br />
a=a+1;<br />
b=b+4;<br />
cout<<a<<" "<<b<<endl;<br />
}<br />
<br />
int main()<br />
{<br />
a=1;<br />
b=2;<br />
afis(a,b);<br />
cout <<a<<" " <<b<< endl;<br />
}<br />
</td>
        <td><br />
</td>
        <td>#include <iostream><br />
using namespace std;<br />
int a,b;<br />
void afis<span style="color: #ff0000;">(int &amp;a, int &amp;b)</span><br />
{<br />
a=a+1;<br />
b=b+4;<br />
cout<<a<<" "<<b<<endl;<br />
}<br />
<br />
int main()<br />
{<br />
a=1;<br />
b=2;<br />
afis(a,b);<br />
cout <<a<<" " <<b<< endl;<br />
}<br />
</td>
        <td><br />
</td>
        <td>#include <iostream><br />
using namespace std;<br />
int a,b;<br />
void afis(<span style="color: #ff0000;">int &amp;m, int n)</span><br />
{<br />
m=m+1;<br />
n=n+4;<br />
cout<<m<<" "<<n<<endl;<br />
}<br />
<br />
int main()<br />
{<br />
a=1;<br />
b=2;<br />
cout <<a<<" " <<b<< endl;<br />
afis(a,b);<br />
cout <<a<<" " <<b;<br />
}<br />
</td>
    </tr>
    <tr>
        <td><strong>Se va afisa:</strong><br />
2 6 <em>(rezultatul apelului functiei afis)</em><br />
1 2 <em>(rezultatul de dupa apelul functiei afis)</em><br />
</td>
        <td><br />
</td>
        <td><strong>Se va afisa:</strong><br />
2 6 <em>(rezultatul apelului functiei afis)</em><br />
2 6 <em>(rezultatul de dupa apelul functiei afis)</em><br />
</td>
        <td><br />
</td>
        <td><strong>Se va afisa:</strong><br />
1 2 <em>(rezultatul inaintea apelului functiei afis)</em><br />
<em>2 6</em> <em>(rezultatul apelului functiei afis)</em><br />
2 2 <em>(rezultatul de dupa apelul functiei afis: variabila a isi pastreaza</em><br />
<em>valoarea dupa apel fiind parametru transmis prin referinta pe cand</em><br />
<em>variabila b revine la valoarea pe care o avea inainte de apel fiind</em><br />
<em>parametru transmis prin valoare)</em><br />
</td>
    </tr>
</table>

<br />


<table class="wiki_table">
    <tr>
        <td colspan="2"><span style="display: block; text-align: left;"><strong><span style="font-family: 'Times New Roman',serif; font-size: 16px;">Exemplul 7.1 </span></strong></span><br />
</td>
    </tr>
    <tr>
        <td><ol><li>include <iostream></li></ol><span style="font-family: 'Times New Roman',serif; font-size: 16px;">using namespace std;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">void schimba_valoare (int x, int y)</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int z=x;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">x = y;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">y = z;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">void schimba_referinta (int &amp;a, int &amp;b)</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int aux=a;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">a=b;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">b=aux;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int main ()</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">{</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">int M=1, N=5;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">schimba_valoare(M,N);</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">cout << "M="<<M<< " " << "N="<<N<<endl;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">schimba_referinta(M,N);</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">cout << "M="<<M<< " " << "N="<<N<<endl;</span><br />
<span style="font-family: 'Times New Roman',serif; font-size: 16px;">}</span><br />
</td>
        <td>APEL PRIN VALOARE<br />
<br />
APEL PRIN REFERINŢĂ<br />
<br />
Se va afişa:<br />
<br />
M=1 N=5<br />
<br />
M=5 N=1<br />
</td>
    </tr>
</table>

<a href="/files/FISA%20DE%20LUCRU%201.doc">FISA DE LUCRU 1.doc</a><br />
<br />
<strong>FISE DE LUCRU</strong> <a href="/files/3_FISEdincapitolulsubprograme2009_2010.doc">3_FISEdincapitolulsubprograme2009_2010.doc</a><br />
<br />
<br />
<strong>TESTE<a href="/files/TEST_SUBPROGRAME.doc">TEST_SUBPROGRAME.doc</a></strong><br />
<br />
<br />
<strong>APLICATII</strong> <a class="wiki_link_ext" href="http://info.mcip.ro/?cap=Subprograme" rel="nofollow">http://info.mcip.ro/?cap=Subprograme</a>
    </div>
  </body>
</html>