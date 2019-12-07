# esercizio-Inc1000 parte 1
Ho creato 2 oggetti con la stessa classe a cui ho esteso a Thread,questi 2 oggetti hanno il compito di incrementare un contatore di 1000 .
Quando si va a fare l' output si può ri-chiamare il metodo dell' oggetto soltanto richiamando la classe,questo perchè il contatore è una variabile statica, quindi tutti gli oggetti di quella classe la condividono.
In output viene restituito il valore 0,questo perchè i Thread vengono fermati priva che facciano il loro incremento.

# esercizio-Inc1000 parte 2
Viene aggiunto il metodo "NomeOggetto.join();" per far si che i Thread incrementino il cont. Questo comporta un rischio, ovvero, due o più thread possono incrementare e riiscriverre contemporaneamente la variabile cont, perciò si andrebbe a perdere qualche numero.

# esercizio-Inc1000 parte 3
Viene aggiunto il tipo synchronyzed per far si che non venga incrementato contemporaneamente da due o più Thread.
