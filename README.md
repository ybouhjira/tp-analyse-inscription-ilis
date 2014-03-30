# Les structures 

```c
typedef struct etudiant{
  char nom[20];
  char prenom[20];
  char cin[20];
  char cne[20];
  int notes[8];
  enum Diplome {DUT, DEUG, DEUST, LICENCE, MAITRISE, MASTER, CPGE};
  char Etablissement[30];
  int nbreAns;
  int anDiplome;
}

typdef struct OptionsDiplome {
  int nombreAnMax;
  int nombreMentionsMin;
  int noteMin;
  float pourcentage;
}
```

# Les fichiers

Dossier->Diplome.
Fichier->Etablissement.
Elements-Fichier->Etudant.

```
nom  prenom  cne  cin  Diplome  nbre_annees  Etablissement Classement/Notes.
nom1 prnom1  cne ...
nom2 prenom2 ...

```
  
# Conditions

```
DUT/DEUG/DEUST  ->  nbre_annees = 2;
LICENSE/MASTER   ->   nbre_annees = 3;
MAITRISE  ->   nbre_annees = 4;


DUT/DEUG/DEUST  ->   1 mention ASSEZ-BIEN;
LICENSE/MAITRISE/MASTER  ->   2 mentions;


PREPAS  ->   Classement;
AUTRE  -> Moyenne;
```


                                
  

