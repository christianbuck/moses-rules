# moses-rules
===========

translate marked up text and numbers with moses

## Translation of markup

We want to translate stuff like this:

> I ate an <b> apple </b>

> Ich habe einen <b> Apfel </b> gegessen

while paying attention to detail:

> I <b> ate </b> an apple

> Ich <b> habe </b> einen Apfel <b> gegessen </b>

Todo: Reconstruct original markup using alignment


## Translation of numbers, dates etc.

Some things are better translated by rules than by looking them up in a table. These include dates and numbers. Thus we would like to translate:

> Pay $1,000 by September 5th 

> Zahle 1.000 $ bis zum 5. September

possibly by annotating the source

> Pay $ &lt;NUMBER&gt; by &lt;DATE&gt; 

> Zahle &lt;NUMBER&gt; $ bis zum &lt;DATE&gt;

and 'translating' the bit with rules and reconstructing the values from the alignment.

