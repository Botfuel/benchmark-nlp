# NLP benchmark test sentences and full results

These are the results of the tests we conducted in July 2017 to write our NLP Benchmark article.
Please note that, though the choice of sentences used is arbitrary, we have used common language entities to best fit all services.

## Entity Extractor

### FR
1. Je veux partir demain matin a 8h.
2. Je serais a Paris de 8h ce soir jusqu'a 15h demain.
3. Je veux acheter une voiture rose.
4. Je voudrais deux croissants.
5. J'ai rendez-vous demain entre 14h et 15h au 9 rue Dareau a Paris.
6. Je veux une salle pour demain 7h avec 3 chaises.
7. Il me faut un moteur de 50 cm3 pour couvrir le terrain avec une bache de 10m sur 3.
8. Aujourd'hui le cours du dollar a chute de 15%, pour atteindre 1 dollars et 27 cents pour 1 euro.
9. Sa fortune est estimee a trois milliards 5 cent quarante sept million deux dollar
10. Hier midi j'ai mange avec Jean, Andrew, Andreas, Kumiko et Abdullah
11. Nous avons marche sur 5 kilometres
12. J'aimerais parier 100€ sur le match de demain entre Paris et Lyon

#### Recast:.ai
1. Time NOT OK
2. City OK | Time NOT OK
3. Color OK | Quantity NOT REC
4. Quantity NOT REC
5. Time OK | Address OK
6. Quantity NOT REC | Time OK | Quantity NOT REC
7. Quantity NOT REC | Volume OK | Quantity NOT REC | Area NOT OK
8. Time OK | Percent OK | Money NOT OK | Money NOT OK
9. Money NOT OK
10. Time OK | Forename OK (x5)
11. Distance OK
12. Money OK | Time NOT OK | City OK | City OK

#### Wit.ai
1. Time OK
2. City OK | Time OK
3. Color NOT REC | Quantity NOT OK
4. Quantity NOT OK
5. Time OK | Address NOT OK
6. Quantity NOT OK | Time OK | Quantity NOT OK
7. Quantity NOT OK | Volume NOT OK | Quantity NOT OK | Area NOT OK
8. Time OK | Percent NOT OK | Money OK | Money OK
9. Money OK
10. Time OK | Forename NOT OK (⅖)
11. Distance OK |
12 Money OK | Time OK | City NOT OK | City NOT OK

#### LUIS

1. Time NOT OK
2. City NOT REC | Interval NOT OK
3. Color NOT REC | Quantity NOT REC
4. Quantity NOT REC
5. Time NOT OK | Address NOT REC
6. Quantity NOT REC | Time NOT OK | Quantity NOT REC
7. Quantity NOT REC | Volume NOT OK | Quantity NOT REC | Area NOT OK
8. Time NOT OK | Percent NOT OK | Money NOT OK | Money NOT OK
9. Money NOT OK
10. Time NOT OK | Forename NOT REC (x5)
11. Distance NOT OK
12. Money OK | Time NOT OK | City NOT REC | City NOT REC

#### SNIPS
1. Time OK
2. City NOT REC | Interval OK
3. Color NOT REC | Quantity NOT REC
4. Quantity NOT REC
5. Time NOT OK | Address NOT REC
6. Quantity NOT REC | Time NOT OK | Quantity NOT REC
7. Quantity NOT REC | Volume NOT REC | Quantity NOT REC | Area NOT REC
8. Time NOT OK | Percent NOT REC | Money NOT REC (x2)
9. Money NOT OK
10. Time OK | Forename NOT REC (x5)
11. Distance NOT REC
12. Money NOT REC | Time NOT OK | City NOT REC | City NOT REC

#### API.ai
1. Time OK
2. City OK | Interval NOT OK
3. Color OK | Quantity NOT REC
4. Quantity NOT REC (Number OK)
5. Time NOT OK | Address OK
6. Quantity NOT REC (Number OK) | Time OK | Quantity NOT REC
7. Quantity NOT REC | Volume OK | Quantity NOT REC | Area OK
8. Time NOT OK | Percent OK | Money NOT OK | Money OK
9. Money OK
10. Time NOT OK | Forename OK (x5)
11. Distance NOT OK
12. Money OK | Time OK | City OK | City OK

#### IBM
1. Time OK
2. Interval OK (Time OK | TIme OK) | City NOT OK
3. Quantity NOT REC (Number OK) | Color NOT OK.
4. Quantity NOT REC (Number OK)
5. Time NOT OK | Address NOT OK
6. Qantity NOt REC | Time OK | Quantity NOT REC
7. Quantity NOT REC | Volume NOT REC | Quantity NOT REC | Area NOT REC
8. Time OK | Percent NOT OK | Money NOT OK | Money NOT OK
9. Money NOT OK
10. Time OK | Forename NOT REC (x5)
11. Distance NOT REC
12. Money NOT OK | Time OK | City NOT OK | City NOT OK

#### Botfuel
1. Time OK
2. Time NOT OK | Location OK
3. Quantity OK | Color OK
4. Quantity OK
5. Interval OK | Address OK
6. Quantity OK | Time OK | Quantity OK
7. Quantity OK | Volume OK | Quantity OK | Area OK
8. Time OK | Percentage OK | Money NOT OK | Money OK
9. Money OK
10. Time OK | Forename OK (x5)
11. Distance OK
12. Money OK | Time OK | City OK

### EN
1. I am leaving tomorrow at 5am for Los Angeles
2. I am going to 142 Pleasance street Edinburgh
3. I live on 3436 Aylmer St Montreal
4. I ate chocolate for the last 2 hours
5. Yesterday at 8pm, I was eating 10 dollars worth of chocolate
6. In two weeks I will be in Paris
7. Where will you be this summer
8. 2 days after tomorrow, I will leave Moscow
9. This item costs 3 dollars and 55 cents
10. I pay 1000 dollars per month for my flat in Washington DC.
11. I need to rent a car for two weeks near Berlin.
12. I want to book two plane tickets to Madrid tomorrow.

#### Recast.ai
1. Time OK | Location OK
2. Address OK
3. Address OK
4. Time NOT OK
5. Time OK | Money OK
6. Time NOT OK | City OK
7. Time NOT OK
8. Time NOT OK | City OK
9. Money NOT OK
10. Money OK | Set (per month) OK | Location OK
11. Quantity NOT REC | Time OK | Location OK
12. Quantity NOT REC (recognized a number) | Location OK | Time OK

#### Wit.ai
1. Time OK | Location OK
2. Address OK
3. Address OK
4. Interval OK
5. Time OK | Money OK
6. Time OK | City OK
7. Time OK
8. Time OK | City OK
9. Money OK
10. Money OK | Set (per month) NOT REC | Location OK
11. Quantity NOT OK | Duration OK | Location OK
12. Quantity NOT OK | Location OK | Time OK

#### LUIS
1. Time OK | Location OK
2. Address NOT OK
3. Address NOT OK
4. Interval OK
5. Time OK | Money OK
6. Time NOT OK | City OK
7. Time OK
8. Time NOT OK | City OK
9. Money NOT OK
10. Money OK | Set (per month) NOT REC | Location OK
11. Quantity  NOT REC | Duration OK | Location OK
12. Number OK | Location NOT OK | Datetime OK

#### SNIPS
1. Time OK | Location NOT REC
2. Address NOT REC
3. Address NOT REC
4. Interval NOT OK
5. Time OK | Money OK
6. Time OK | City NOT REC
7. Time OK
8. Time OK | City NOT REC
9. Money OK
10. Money OK | Set (per month) NOT REC | Location NOT REC
11. Quantity NOT REC |Duration NOT OK | Location NOT REC
12. (Quantity NOT REC) Number OK | Location NOT REC | Datetime OK

#### API.ai
1. Time OK | Location OK
2. Address OK
3. Address OK
4. Interval OK
5. Time OK | Money OK
6. Time NOT OK | City OK
7. Time OK
8. Time OK | City OK
9. Money OK
10. Money OK | Set (per month) NOT REC | City OK
11. Quantity NOT REC (Number OK)  | Duration OK | City OK
12. Quantity NOT REC (Number OK) | City OK | Time OK

#### IBM
1. Time OK | Location OK
2. Address NOT OK
3. Address NOT OK
4. Interval OK
5. Time OK | Money OK
6. Time OK | City OK
7. Time NOT OK
8. Time NOT OK | City OK
9. Money OK
10. Money OK | Set (per month) NOT REC | Location OK
11. Quantity NOT REC | Interval NOT OK | Location OK
12. Quantity NOR REC (Number NOT OK) | Location OK | Time OK

#### Amazon Lex
1. Time OK | City OK
2. Address OK
3. Address OK
4. Duration NOT OK
5. Time OK | Money NOT REC
6. Time NOT OK | City OK
7. Time OK
8. Time OK | City OK
9. Money NOT REC
10. Money NOT REC | Set (per month) NOT REC | City OK
11. Quantity NOT REC | Duration OK | City OK
12. Quantity NOT OK (Number NOT OK) | City OK | Date OK

#### Botfuel
1. Time OK | City OK
2. Address OK
3. Address OK
4. Interval OK
5. Time OK | Money OK
6. Time OK | City OK
7. Interval OK
8. Time OK | City OK
9. Money OK
10. Money OK | Set (per month) NOT REC | City OK
11. Quantity NOT OK | Time OK | City OK
12. Quantity NOT OK | City OK | Time OK

## Spell Checking

### FR_2
```
Voiic la phrse a corryjer
```
* ~~BING~~ : `voici la phrase à corner`
* BOTFUEL : `voici la phrase à corriger`
* X SPELL : `Voici la phrase a corriger`

```
Je voayge a Pariss
```
* BING : `Je voyage a paris`
* BOTFUEL : `Je voyage a paris`
* X SPELL : `Je voyage a Paris`

```
Je veux parier sur un amtch amica Paris-Lyno
```
* ~~BING~~ : `Je veux parler sur un match amical Paris-lyon`
* BOTFUEL : `Je veux parier sur un match amical Paris-lyon`
* X SPELL : `Je veux parier sur un match amical Paris-Lyon`

```
Je vais avoir selemnet vintg qatre asn dnas sept annees
```
* BING : `Je vais avoir seulement vingt quatre ans dans sept annees`
* BOTFUEL : `Je vais avoir seulement vingt quatre ans dans sept années`
* X SPELL : `Je vais avoir seulement vingt quatre asn dnas sept annees`

```
ma carosserie est intacte
```
* ~~BING~~ : `ma carrosserie est intact`
* BOTFUEL : `ma carrosserie est intacte`
* X SPELL : `ma carrosserie est intacte`

```
je veux manaer ce poulet
```
* ~~BING~~ : `je veux manager ce poulet`
* BOTFUEL : `je veux manger ce poulet`
* X SPELL : `je veux manger ce poulet`

```
Domain, je mange des pâtes
```
* ~~BING~~: `domain, je mange des pâtes`
* ~~BOTFUEL~~: `domaine, je mange des pâtes`
* ~~X SPELL~~ : `Domain, je mange des pâtes`


```
Lontgemps, je me suis couché de bonne huere
```
* BING : `longtemps, je me suis couche de bonne heure`
* BOTFUEL: `longtemps, je me suis couché de bonne heure`
* X SPELL : `Longtemps, je me suis couché de bonne heure`

```
Ctete baguette coûte un uero
```
* ~~BING~~ : `Ctete baguette coûte un uero`
* BOTFUEL: `cette baguette coûte un euro`
* X SPELL : `Cette baguette coûte un euro`

```
J’ai perdu un milleir d’euros
```
* BING : `J’ai perdu un millier d’euros`
* BOTFUEL: `J’ai perdu un millier d’euros`
* X SPELL : `J’ai perdu un millier d’euros`

### EN_2

```
hwo are yuo donig tonigth
```
* BING : `how are you doing tonight`
* BOTFUEL : `how are you doing tonight`
* X SPELL : `how are you doing tonight`

```
wheer have you bene all night
```
* BING : `where have you been all night`
* BOTFUEL : `where have you been all night`
* XSPELL : `where have you been all night`

```
why are yuo not here wiht us tongiht
```
* BING : `why are you not here with us tonight`
* BOTFUEL : `why are you not here with us tonight`
* X SPELL : `why are you not here with us tonight`

```
Wat are you gonan do
```
* BING : `what are you gonna do`
* ~~BOTFUEL~~ : `Wat are you conan do`
* X SPELL : `What are you gonna do`

```
I dont knwo anythign
```
* BING : `I don't know anything`
* BOTFUEL : `I dont know anything`
* X SPELL : `I don’t know anything`

```
I donot agre with yuo
```
* BING : `I do not agree with you`
* ~~BOTFUEL~~ : `I donor are with you`
* X SPELL : `I don’t agree with you`

```
I’ll leave aerlier today
```
* BING : `I’ll leave earlier today `
* BOTFUEL : `I’ll leave earlier today`
* X SPELL : `I’ll leave earlier today`

```
I’m very hnugry today
```
* BING : `I’m very hungry today `
* BOTFUEL : `I’m very hungry today`
* X SPELL : `I’m very hungry today`

```
I finihs work at 7pm
```
* BING : `I finish work at 7pm`
* BOTFUEL : `I finish work at 7pm`
* X SPELL : `I finish work at 7pm`

```
Where can i take a braekfast
```
* BING : `Where can i take a breakfast`
* BOTFUEL : `Where can i take a breakfast`
* X SPELL : `Where can i take a breakfast`

## Spell-checking and Entity Extraction:

### EN
```
I am leaving tomorro at 5am for Lo Angeles
```
* Botfuel : Time OK
* Microsoft : Time OK
* Recast : Time NOT OK (5am)
* API.AI : Time NOT OK
* SNIPS : Time NOT OK
* Lex : Time OK
* Wit : NO
* IBM : NO

```
Yestrday at 8pm, I was eating 10 dlolars worth of chocolate
```
* Botfuel : Time OK
* Microsoft : Time OK
* Recast : Time NOT OK (8pm)
* API.AI : Time NOT OK (8pm)
* Snips : Time NOT OK
* Lex : Time NOT OK
* Wit : NO
* IBM : NO

```
I want to book two plane tickets to Madrid tomorow.
```
* Botfuel : OK
* Microsoft : OK
* Recast : NO (spell failed)
* API.AI : OK
* Lex : OK
* Snips : OK
* Wit : OK
* IBM : NO

```
At eight o’clck, I need someone to keep my dog.
```
* Botfuel : OK
* Recast : NO
* Microsoft : OK
* API.AI : NO
* Lex : NO
* Snips : NO
* Wit : OK
* IBM : OK

```
Next moday, I won’t be home
```
* Botfuel : NO (spell failed)
* Microsoft : OK
* Recast : NO
* API.AI : NO
* Lex : NO
* Snips : NO
* Wit : NO
* IBM : NO

```
I will need a car in two hoaurs
```
* Botfuel : NO (entity failed)
* Microsoft : OK
* Recast : NO
* API.AI : NO
* Lex : NO
* Snips : NO
* Wit : NO
* IBM : NO

```
I need to a plane ticket for the 3rd Agust
```
* Botfuel : OK
* Microsoft : NO (spell failed)
* Recast : NO
* API.AI : OK
* Lex : NO
* Snips : NO
* Wit : OK
* IBM : NO

```
I leave the town next mounth
```
* Botfuel : NO (spell failed)
* Microsoft : NO (entity failed)
* Recast : NO
* API.AI : NO
* Lex : NO
* Snips : NO
* Wit : NO
* IBM : NO

```
I won’t be there on satrday
```
* Botfuel : OK
* Microsoft : OK
* Recast : NO
* API.AI : NO
* Lex : NO
* Snips : NO
* Wit : NO
* IBM : NO

```
I will come back at nin o’clock
```
* Botfuel : NO (spell failed)
* Microsoft : OK
* Recast : NO
* API.AI : NO
* Lex : NO
* Snips : NO
* Wit : NO
* IBM : NO

### FR
```
Je pars deman à 5h pour Los Angeles
```
* Botfuel : OK
* Recast : NO
* API.AI : OK
* Wit : NO
* IBM :NO

```
Hir à 8h, j’ai mangé pour 10 dollars de chocolat
```
* Botfuel : NO (spell failed)
* Recast : NO
* API.AI : NO
* Wit : NO
* IBM :NO

```
Je voudrais réserver deux billets d’avion pour Madrid domain
```
* Botfuel : NO (spell failed)
* Recast : NO
* API.AI : NO
* Wit : NO
* IBM :NO

```
À huit heuures, j’ai besoin de quelqu’un pour garder mon chien
```
* Botfuel : OK
* Recast : NO
* API.AI : NO
* Wit : NO
* IBM : OK

```
Ludi prochain, je ne serai pas à la maison
```
* Botfuel : NO (spell failed)
* Recast : NO
* API.AI : NO
* Wit : NO
* IBM :NO

```
j’aurai besoin d’une voiture dans deux heurs
```
* Botfuel : NO (spell failed)
* Recast : NO
* API.AI : NO
* Wit : NO
* IBM :NO

```
j’ai besoin d’un ticket d’avion pour le 3 out
```
* Botfuel : NO (spell failed)
* Recast : NO
* API.AI : NO
* Wit : OK
* IBM :NO

```
Je quitte la ville le mois prochin
```
* Botfuel : OK
* Recast : NO
* API.AI : NO
* Wit : NO
* IBM :NO

```
Je ne serai pas là ce samdi
```
* Botfuel : OK
* Recast : NO
* API.AI : NO
* Wit : NO
* IBM :NO

```
Je reviendrai à neuf hures
```
* Botfuel : OK
* Recast : NO
* API.AI : NO
* Wit : NO
* IBM : OK
