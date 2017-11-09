# small-world
Wer bereits mit Shopware Version 5.3.1 ein Theme einsetzt, und eventuell CSS/Less Änderungen an seinem Button "Land auswählen" vorgenommen hat, hat spätestens jetzt gemerkt, dass der Button wie der Ursprungsbutton jetzt ausschaut.
Das liegt vermutlich daran, dass sich die Klasse geändert hat.
 
**Früher hieß die Klasse**</br>
   .field--select}
     .js--fancy-select{
     }   
  }

Die Klasse findet sich in der **fields.less** im Ordner Responsive _./frontend/_public/src/less/_components.
 
**Aktuell heißt die Klasse**</br>
.select-field,
    .js--fancy-select {
    }
}

Hier habe ich mal eine Klassendefinition erstellt und in die footer.less eingebunden. 
P.S: Einstellung gilt nur für Desktopansicht. Für Smartphones, muss extra noch geschrieben werden. </br> </br>
**Es geht ja auch nur darum welche Klasse angesprochen werden soll.**
</br> Und noch was, den textbaustein "Land auswählen" hab ich mittels inlestyle direkt im Textbaustein weiss gemacht. 

Wäre schön wenn wir die richtigen Anpassungen beim nächsten Livestream machen könnten.
