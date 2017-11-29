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

Habe dazu in meinem Theme einfach in src/less/_components auch eine fields.less angelegt.
Danach die Klassen die ich überschreiben möchte eingebunden.
Anschließend in meiner all.less noch die less importiert und fertig.

Wäre schön wenn wir die richtigen Anpassungen beim nächsten Livestream machen könnten.
