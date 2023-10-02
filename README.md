-Come prima cosa dobbiamo scaricare il file da google classroom e rinominarlo nella maniera corretta
-In seguito dobbiamo aprire la cartella su visual studio code
-Subito dopo inizia il vero programma\
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-Per prima cosa dobbiamo scorrere ogni elemento dentro all'array usando un foreach:\

foreach (var num in vettore){}
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-All'interno di questo vettore richiamiamo il metotodo IsnumeroTelefonoItaliano e controlliamo che "num" sia valido:\

 if (IsnumeroTelefonoItaliano(num))
        {
            return num;
        }   
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-Subito dopo possiamo creare un metodo che verifchi le varie caratteristiche che deve avere il numero di telefono\

-Con questo metodo verifichiamo lunghezza della stringa e i prefissi, se ritorna "true" vuol dire che è valida:\

if (num.Length == 13 && (num.StartsWith("+39"))
    {
        return true;
    }
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-Di seguito gli altri 2 metodi per verificare se sono giuste, ma con caratteristiche diverse:\

        if (num.Length == 14 && num.StartsWith("0039"))
    {
        return true;
    }
-Questo è l'ultimo:\

    if (num.Length == 10 && num.StartsWith("3"))
    {
        return true;
    }
-Se la stringa non soddisfa le condizioni, il programma ritorna "false" e quindi il numero non risulta valido.

-Il codice finisce così, verrà modificato in caso di aggiornamenti
