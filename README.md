Med hjälp av passagerardata från Titanic var målet att bygga en maskininlärningsmodell för att förutsäga passagerarnas överlevnadsgrad baserat på deras egenskaper, såsom klass, ålder, kön etc. Målet var att bestämma vilka faktorer som mest påverkade överlevnadsförmågan, och förutsäga om huruvida passagerare kan överleva ett skeppsvrak.
Dataset är hämtat från Kaggles Dataset: https://www.kaggle.com/datasets/yasserh/titanic-dataset

Resultat:
Data om passagerarna på Titanic-fartyget har laddats ner och förbehandlats.
En Decision Tree and Random Forest maskininlärningsmodell byggdes för att förutsäga passagerares överlevnad.
Den resulterande modellen visade en prediktionsnoggrannhet på cirka 77,65 % för beslutsträd och 81,56 % för Random Forest på testdata.
Anledningar till varför resultatet av modellering med Random Forest kan vara bättre:
-	Fylla i saknade ”Age”: Saknade åldrar ersattes med medelvärden baserade på passagerarklass. Detta kan hjälpa modellen att bättre tolka ålderssignaturen och i slutändan förbättra prediktionsnoggrannheten.
-	Använda Random Forest: Denna algoritm är en ensemblemaskininlärningsmetod som kombinerar flera beslutsträd för att producera mer exakta förutsägelser.
-	Dataförberedelse: Kolumnerna ”PassengerId”, ”Name” och ”Ticket” har tagits bort, vilket förmodligen inte har någon betydande inverkan på överlevnadsförmågan.
Dessa tecken kan vara anledningen till att resultatet av Random Forest-modellen är högre än resultatet av Decision Tree-modellen.
