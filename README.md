# presidentielle-2017
Datasets &amp; statistics about the 2017 French presidential election

# JSON format
```
{
  // Résultats par candidat
  "result":[
    [
      "Emmanuel MACRON",        // Candidat ayant le plus de voix dans la localisation considérée
      24.01,                    // Pourcentage des voix
      8657326                   // Nombre de voix
    ],
    [
      "Marine LE PEN",          // Candidat en 2ème position
      21.3,
      7679493
    ],
    ...
  ],
  
  // Sous-divisions locales (dans la plupart des cas, France > Région > Département > Commune, mais attention aux DOM-TOM)
  "subregions":{                
    "region-auvergne-et-rhone-alpes":{
      "result":[...]
      "subregions":{...}
      "votants":{...}
    },
    "region-bourgogne-franche-comte":{...}
  },
  
  // Statistiques sur les votants
  "votants":{
    "blancs":659302,             // Nombre de votes blancs
    "blancs_prc":1.39,           // Pourcentage de votes blancs (par rapport au nombre d'inscrits)
    "exprimes":36058813,         // Suffrage exprimés
    "exprimes_prc":75.78,        // Pourcentage de suffrages exprimés (par rapport au nombre d'inscrits)
    "inscrits":47581118,         // Nombre d'inscrits
    "nuls":285431,               // Nombre de bulletins nuls
    "nuls_prc":0.6,              // Pourcentage de bulletins nuls (par rapport au nombre d'inscrits)
    "participation":37003546,    // Nombre de participants
    "participation_prc":77.77    // Taux de participation
  }
}
```
Tous les nombres décimaux sont des arrondis au centième.

Source : Ministère de l'Intérieur
