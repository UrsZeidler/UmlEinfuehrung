# UmlEinfuehrung

Eine kleine Einf�hrung in Uml.

UML ist eine Notationstechnik f�r die Objektorientierten (OO) Software Entwicklung.


## Historischer Abriss

UML als Unified Modeling Language war die Bestrebung die verschiedenen vorhandenen Graphischen Notationen zur Beschreibung eines Software Systems zu vereinheitlichen und auf ein formalisiertes Fundament zu stellen. 

![OO-historie](images/500px-OO-historie-2.png)

Urspr�nglich handelt es sich um eine Initiative von Grady Booch, Ivar Jacobson und James Rumbaugh, oft werden sie als die drei Amigos bezeichnet. Bei rational Software angestellt entwickelten sie die UML 1.0 um ihre eigenen, verschiedenen Methoden und Notationen zu vereinheitlichen.

Diese Vereinheitlichung wurde 1997 an die OMG (Object Management Group) �bergeben und als Standard angenommen.



## Model, Metamodel und Metametamodell (M0/M1/M2/M3)

Uml, als eine Notationssprache um Modelle (M1) zu definieren, ist selbst in einer Modellsprache definiert. Diese Modellsprache (M3) wird MOF (Meta object facility) genannt. Dieser Systematische Ansatz tr�gt sowohl zur Eindeutigkeit der Syntaktik bei auch wird er wichtig f�r die Modelgetriebene Entwicklung und den aus ihr resultierenden Techniken der Modell und Code Transformationen.

![mm](images/500px-MetamodelHierarchy_de.png)

M3 � MOF das �Meta object facility� ist stark ein begrenztes Model das von der OMG spezifiziert ist. Es enth�lt nur wenige Modelelement die jedoch geeignet sind Modelle zu spezifizieren.

![MOF](images/MOF_Metamodel_144dpi.jpg)

M2 � Mit dem M3, dem MOF, wird nun das Modell der UML beschrieben. Damit ist die Spezifikation der UML selbst auf eine solide und nachvollziehbare Basis gestellt.

M1 � In UML wird das zu entwerfende Modell beschreiben.

M0 � Ist die Software selber. Die in dem Modell (M1) beschriebenen Entit�ten (Klassen und deren Beziehungen) sind als Instanzen in der laufenden Software vorhanden. Sie sind jedoch nur ein Modell der Wirklichkeit und nicht die Wirklichkeit selbst. Als Beispiel ist der Kunde in einem CRM nicht der Kunde selber sondern nur eine Abbildung des Kunden mit den f�r den Anwendungsfall relevanten Attributen. Jede Software ist demnach ein Modell.



## Gliederung der verschieden Diagrammtypen
F�r die Modellierung verschiedenen Aspekte der Softwareentwicklung eignen sich nicht alle Diagrammformen, deshalb stellt die UML verschieden Diagramme bereit diese einzelnen Aspekte zu fassen. Grob unterteilen sie sich in Strukturelle und Verhaltes orientierte Diagramme. 


### Struktur orientierte Diagramme

Aufgabe der Strukturorientierten Diagramme ist die Beschreibung des Aufbaus und der Teile aus denen das Software System besteht und deren Beziehung zueinander.

#### das Klassendiagramm

#### das Kompositionsstrukturdiagramm (auch: Montagediagramm)

#### das Komponentendiagramm

#### das Verteilungsdiagramm

#### das Objektdiagramm

#### das Paketdiagramm

#### das Profildiagramm

Ein Profil ist die M�glichkeit UML, um Fachspezifische Eigenschaften, zu erweitern. So k�nnen Eigenschaften die nicht in UML vorgesehen sind in dem Modell spezifiziert werden. 

Es ist ein recht einfaches Diagramm, das im Prinzip aus zwei Diagramm Elementen, den Stereotyp und der Metaklasse.

Der Stereotype erweitert eine Metaklasse um Eigenschaften.
Eine Metaklasse ist ein Modellelement aus dem UML Metamodel auf die ein Stereotype angewendet werden kann.

![profil](images/contracts.profile.png)



### Verhaltes orientierte Diagramme

Aufgabe der Verhaltensorientieren Diagramme ist die Beschreibung der Verhaltensaspekte des Software Systems.

#### das Aktivit�tsdiagramm

#### das Anwendungsfalldiagramm (auch: Use-Case o. Nutzfalldiagramm genannt)

#### das Interaktions�bersichtsdiagramm

#### das Kommunikationsdiagramm

#### das Sequenzdiagramm

#### das Zeitverlaufsdiagramm

#### das Zustandsdiagramm.



## MDE/MDA (Model getriebene Entwicklung)


## Software die UML unterst�tzt

Papyrus (Eclipse Plugin) https://eclipse.org/papyrus/
Eclipse ist eine Plattform nicht nur zur einfachen Java Entwicklung, unter dem Dach der Eclipse Foundation gibt es eine Menge Projekte die sich mit der Modellierung besch�ftigen. (https://eclipse.org/modeling/) Hier ist besonders das Acceleo Projekt (http://www.eclipse.org/acceleo/), ein auf dem MTL (Model to Text Language) basierender Codegenerator und ATL (http://www.eclipse.org/atl/) eine Model Transformations Sprache hervor zu heben.


----

images from wikipedia


