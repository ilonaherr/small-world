# small-world
Wer bereits mit Shopware Version 5.3.1 ein Theme einsetzt, und eventuell CSS/Less Änderungen an seinem Button "Land auswählen" vorgenommen hat, hat spätestens jetzt gemerkt, dass der Button wie der Ursprungsbutton jetzt ausschaut.
Das liegt vermutlich daran, dass sich die Klasse geändert hat.
 
**Früher hieß die Klasse**
   .field--select}
     .js--fancy-select{
     }   
  } **_und lag in der "footer.less"**

Die Klasse findet sich nun in der **fields.less** im Ordner Responsive _./frontend/_public/src/less/_components , mit dem Klassennamen: 

.select-field,
    .js--fancy-select {
    }
}

Hier habe ich mal eine Klassendefinition erstellt. Wichtig! dass die Datei in Eurem Themeordner im entsprechenden Verzeichnis angelegt und definiert wurde und in der all.less auch importiert wird. 
