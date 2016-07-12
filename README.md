# UmlEinfuehrung

Eine kleine Einführung in Uml.

UML ist eine Notationstechnik für die Objektorientierten (OO) Software Entwicklung.


## Historischer Abriss

UML als Unified Modeling Language war die Bestrebung die verschiedenen vorhandenen Graphischen Notationen zur Beschreibung eines Software Systems zu vereinheitlichen und auf ein formalisiertes Fundament zu stellen. 

![OO-historie](images/500px-OO-historie-2.png)

Ursprünglich handelt es sich um eine Initiative von Grady Booch, Ivar Jacobson und James Rumbaugh, oft werden sie als die drei Amigos bezeichnet. Bei rational Software angestellt entwickelten sie die UML 1.0 um ihre eigenen, verschiedenen Methoden und Notationen zu vereinheitlichen.

Diese Vereinheitlichung wurde 1997 an die OMG (Object Management Group) übergeben und als Standard angenommen.



## Model, Metamodel und Metametamodell (M0/M1/M2/M3)

Uml als eine Notationssprache um Modelle (M1) zu definieren ist selbst in einer Modellsprache definiert. Diese Modellsprache (M3) wird MOF (Meta object facility) genannt. Dieser Systematische Ansatz trägt sowohl zur Eindeutigkeit der Syntaktik bei auch wird er wichtig für die Modelgetriebene Entwicklung und den aus ihr resultierenden Techniken der Modell und Code Transformationen.

![mm](images/500px-MetamodelHierarchy_de.png)

M3 – MOF das “Meta object facility” ist stark ein begrenztes Model das von der OMG spezifiziert ist. Es enthält nur wenige Modelelement die jedoch geeignet sind Modelle zu spezifizieren.

![MOF](images/MOF_Metamodel_144dpi.jpg)

M2 – Mit dem M3, dem MOF, wird nun das Modell der UML beschrieben.

M1 – In UML wird das zu entwerfende Modell beschreiben.

M0 – Ist die Software selber.



## Gliederung der verschieden Diagrammtypen


### Struktur orientierte Diagramme

Aufgabe der Strukturorientierten Diagramme ist die Beschreibung des Aufbaus und der Teile aus denen das Software System besteht.

#### das Klassendiagramm

#### das Kompositionsstrukturdiagramm (auch: Montagediagramm)

#### das Komponentendiagramm

#### das Verteilungsdiagramm

#### das Objektdiagramm

#### das Paketdiagramm

#### das Profildiagramm


### Verhaltes orientierte Diagramme

Aufgabe der Verhaltensorientieren Diagramme ist die Beschreibung der Verhaltensaspekte des Software Systems.

#### das Aktivitätsdiagramm

#### das Anwendungsfalldiagramm (auch: Use-Case o. Nutzfalldiagramm genannt)

#### das Interaktionsübersichtsdiagramm

#### das Kommunikationsdiagramm

#### das Sequenzdiagramm

#### das Zeitverlaufsdiagramm

#### das Zustandsdiagramm.



## MDE/MDA (Model getriebene Entwicklung)


## Software die UML unterstützt

Papyrus (Eclipse Plugin) https://eclipse.org/papyrus/
Eclipse ist eine Plattform nicht nur zur einfachen Java Entwicklung, unter dem Dach der Eclipse Foundation gibt es eine Menge Projekte die sich mit der Modellierung beschäftigen. (https://eclipse.org/modeling/) Hier ist besonders das Acceleo Projekt (http://www.eclipse.org/acceleo/), ein auf dem MTL (Model to Text Language) basierender Codegenerator und ATL (http://www.eclipse.org/atl/) eine model Transformations Sprache hervor zu heben.


----

images from wikipedia


