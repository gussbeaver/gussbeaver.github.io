---
layout: post
title:  "Il sale nella fermentazione acido-lattica"
categories: [ fermentazione ]
image: assets/images/sale-integrale.jpg
tags: [featured]
comments: false
---
La corretta quantità di sale nella [fermentazione acido-lattica](../fermentazione-acido-lattica) è importante per:
- estrarre l'acqua da verdura e frutta;
- creare un ambiente che consenta ai microrganismi di lavorare al meglio;
- mantenere una buona croccantezza degli ingredienti.

> Il tipo di sale impiegato è fondamentale. Ne esistono in commercio molte tipologie, ma il migliore per la fermentazione è il **sale marino integrale**. Da evitare il sale iodato, perché lo iodio inibisce l'azione dei microrganismi, anche quelli necessari al processo di fermentazione acido-lattica.

La maggior parte delle ricette prevede la seguente quantità di sale:
- con salamoia: **da 30 a 50 grammi di sale** per ogni **litro di acqua**
- senza salamoia: **10 grammi di sale** per ogni **Kg di prodotto**

Attenzione perché alcune ricette esprimono la quantità di sale in percentuale sul totale. Ad esempio richiedono che il sale corrisponda al 3% del peso totale di tutto ciò che viene messo nel barattolo: verdura/frutta, acqua, aromi, ... e anche il sale stesso.

#### Come si fa questo calcolo?
- Pesare il vaso vuoto, e segnarsi tale peso in grammi
{% highlight ruby %}
pesoVaso
{% endhighlight %}
- Sistemare tutti gli ingredienti da fermentare nel vaso
- Inserire nel vaso la giusta quantità di acqua
- Pesare il vaso riempito sino ad ora, e segnarsi tale peso in grammi
{% highlight ruby %}
pesoVasoIngredientiAcqua
{% endhighlight %}
- Calcolare il peso di ingredienti e acqua escludendo quello del vaso vuoto:
{% highlight ruby %}
pesoIngredientiAcqua = pesoVasoIngredientiAcqua - pesoVaso
{% endhighlight %}
- Il peso in grammi del sale da aggiungere (nell'ipotesi di salamoia al 3%) sarà pari a:
{% highlight ruby %}
pesoIngredientiAcqua * 3 : (100 - 3)
{% endhighlight %}

> In generale, se la ricetta per la salamoia indica l'**x%** di sale, la formula per calcolare la quantità di sale in grammi è:
**pesoIngredientiAcqua * x : (100 - x)**



#### Vediamo un esempio
- Ho un vaso da 500 g
{% highlight ruby %}
pesoVaso = 500
{% endhighlight %}
- Peso il vaso con tutti gli ingredienti e l'acqua: 2000 g
{% highlight ruby %}
pesoVasoIngredientiAcqua = 2000
{% endhighlight %}
- Calcolo il peso di ingredienti e acqua togliendo il peso del vaso
{% highlight ruby %}
Calcolo 2000 - 500, quindi
pesoIngredientiAcqua = 1500
{% endhighlight %}
- Calcolo il peso del sale (nell'ipotesi di salamoia al 3%)
{% highlight ruby %}
1500 * 3 : (100 - 3)
cioè 4500 : 97
cioè 46,39 grammi
{% endhighlight %}

