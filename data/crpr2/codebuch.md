# Datensatz VfB Stuttgart Netzwerk #
Codebuch Stand 2021-02-22   
erstellt von Sarah Huß (sh311@hdm-stuttgart.de)

## Inhalt
- Edges.csv (Edgelist)
- Nodes.csv (Nodelist)
- Codebuch.rm (Codierung der Datensätze)

## Ursprung und Datenerhebung
Ich habe den Datensatz im Rahmen des Testats für den Kurs Netzwerkanalyse erhoben. Die Daten sind im Internet recherchiert worden.

Das Netzwerk ist ein *ungerichtetes two-mode Akteurs- und Organisationsnetzwerk*. Es wurden zwei getrennte Fragen erhoben:

**Projektarbeitsnetzwerk work**  
1a) Bei welchem Oragn (Vorstand oder Aufsichtsrat) der Akteur tätig ist.  
1b) Bei welchee außenstehenden Organisation der Akteur tätig ist.  
  


# NODE-Attribute

**id**  
ID des Aktuers oder der Organisation, welche identisch mit der der Edgelist sein muss.
Bei Akteuren sind das die Anfangsbuchstaben der Vor- und Nachnamen in Großbuchstaben.
Bei Organisationen sind es die Anfangsbuchstaben der einzelnen Wörter, aus der sich der Name der Organisation zusammensetzt.

**name**  
Gibt den vollen Vor- und Nachnamen des Akteurs am (Person oder Organisation).

**type**
Gibt an, ob es sich bei um einen Akteur (natürliche Person) handelt = 0, oder um eine Organisation = 1.

**age**  
Das Alter des Akteurs, angegeben in natürlichen Zahlen.  

***function***
Gibt an, in welchem Gremium des VfB Stuttgarts der Akteur tätig ist.
V = Vorstand
AR = Aufsichtsrat

***representation***
Gibt an, in welchen Themenbereichen die Akteure innerhalb des VfBs tätig sind.
SP = Sport
US = Unternehmensstrategie 
K = Kommunikation
F = Finanzen
VW = Verwaltung 

***position***
die position die der Akteur einnimmt 
V= Vorstand
IV= Interimvorstand
MG= Mitglied
STV= Stellvertreter

***organisation****
die Organisationen, denen der Akteur angehört als id aufgelistet


# EDGE-Attribute  

***id***
ID des Aktuers oder der Organisation, welche identisch mit der der Nodelist sein muss.
Bei Akteuren sind das die Anfangsbuchstaben der Vor- und Nachnamen in Großbuchstaben.
Bei Organisationen sind es die Anfangsbuchstaben der einzelnen Wörter, aus der sich der Name der Organisation zusammensetzt.
  
**from**  
von wem die beziehung ausgeht 

**to**    
an wen die Beziehung geht

-> da es ein ungerichtetes Netzwerk ist, ist es nicht wichtig wer bei *from* und wer bei *to* aufgeführt ist.
     
##
