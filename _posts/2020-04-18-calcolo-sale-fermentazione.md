---
layout: post
title:  "La quantità di sale per la fermentazione acido-lattica"
categories: [ fermentazione ]
image: assets/images/fermentazione-carote-05.jpg
tags: [featured]
comments: false
---
Il calcolo corretto della quantità di sale per preparare la salamoia di una [fermentazione acido-lattica](../fermentazione-acido-lattica) è importante per consentire ai microrganismi di poter lavorare al meglio.

> Ma anche il tipo di sale è rilevante, infatti esistono in commercio molte tipologie di sale. Il migliore per la fermentazione è quello **marino integrale**. Meglio evitare il sale iodato, perché lo iodio inibisce l'azione dei microrganismi, anche quelli necessari al processo di fermentazione acido-lattica.

Se una ricetta per la fermentazione richiede il 3% di sale, significa che il sale deve costituire il 3% del peso totale di verdura/frutta, acqua, aromi, ... e anche sale, cioè **tutto quello che mettiamo nel vaso**.

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

#### Come NON si fa questo calcolo?
Non è corretto calcolare il 3% del peso degli ingredienti senza il sale.

Infatti, riprendendo l'esempio precedente, avendo 1500g di verdura/frutta, aromi e acqua senza sale, se calcolassi il 3% otterrei 45g.
Quindi nel vaso metterei in tutto 1545g di materiale.

45 è il 2,91% di 1545.

Quindi questo calcolo **sbagliato** ci avrebbe portato a fare una salamoia al 2,91% di sale, **NON** al 3%.

