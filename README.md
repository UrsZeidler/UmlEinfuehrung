# UmlEinfuehrung

Eine kleine Einführung in Uml.

UML ist eine Notationstechnik für die Objektorientierten (OO) Software Entwicklung.


## Historischer Abriss

UML als Unified Modeling Language war die Bestrebung die verschiedenen vorhandenen Graphischen Notationen zur Beschreibung eines Software Systems zu vereinheitlichen und auf ein formalisiertes Fundament zu stellen. 

![OO-historie](images/500px-OO-historie-2.png)

Ursprünglich handelt es sich um eine Initiative von Grady Booch, Ivar Jacobson und James Rumbaugh, oft werden sie als die drei Amigos bezeichnet. Bei rational Software angestellt entwickelten sie die UML 1.0 um ihre eigenen, verschiedenen Methoden und Notationen zu vereinheitlichen.

Diese Vereinheitlichung wurde 1997 an die OMG (Object Management Group) übergeben und als Standard angenommen.



## Model, Metamodel und Metametamodell (M0/M1/M2/M3)

Uml, als eine Notationssprache um Modelle (M1) zu definieren, ist selbst in einer Modellsprache definiert. Diese Modellsprache (M3) wird MOF (Meta object facility) genannt. Dieser Systematische Ansatz trägt sowohl zur Eindeutigkeit der Syntaktik bei auch wird er wichtig für die Modelgetriebene Entwicklung und den aus ihr resultierenden Techniken der Modell und Code Transformationen.

![mm](images/500px-MetamodelHierarchy_de.png)

M3 – MOF das “Meta object facility” ist stark ein begrenztes Model das von der OMG spezifiziert ist. Es enthält nur wenige Modelelement die jedoch geeignet sind Modelle zu spezifizieren.

![MOF](images/MOF_Metamodel_144dpi.jpg)

M2 – Mit dem M3, dem MOF, wird nun das Modell der UML beschrieben. Damit ist die Spezifikation der UML selbst auf eine solide und nachvollziehbare Basis gestellt.

M1 – In UML wird das zu entwerfende Modell beschreiben.

M0 – Ist die Software selber. Die in dem Modell (M1) beschriebenen Entitäten (Klassen und deren Beziehungen) sind als Instanzen in der laufenden Software vorhanden. Sie sind jedoch nur ein Modell der Wirklichkeit und nicht die Wirklichkeit selbst. Als Beispiel ist der Kunde in einem CRM nicht der Kunde selber sondern nur eine Abbildung des Kunden mit den für den Anwendungsfall relevanten Attributen. Jede Software ist demnach ein Modell.



## Gliederung der verschieden Diagrammtypen
Für die Modellierung verschiedenen Aspekte der Softwareentwicklung eignen sich nicht alle Diagrammformen, deshalb stellt die UML verschieden Diagramme bereit diese einzelnen Aspekte zu fassen. Grob unterteilen sie sich in Strukturelle und Verhaltes orientierte Diagramme. 

![diagramme](images/uml-25-diagrams.png)



### Struktur orientierte Diagramme

Aufgabe der Strukturorientierten Diagramme ist die Beschreibung des Aufbaus und der Teile aus denen das Software System besteht und deren Beziehung zueinander.


#### das Paketdiagramm

Uml unterstützt Namspaces, Namesräume sind ein Konzept die Elemente in einer Baumartigen Struktur hierarchisch zu gliedern. Die meisten Objektorientierten Programmiersprachen unterstützen Namspaces, z.B. in java in Form der Packages.

Das Packet Diagramm ist ein einfaches Diagramm mit nur einem elementaren Notationstypen, dem Packet. Zwischen Paketen können Beziehungen bestehen wie „include“ oder „Dependecies“.

![package](images/party-dao-package.png)

#### das Verteilungsdiagramm (Deployment Diagramm)

Das Deployment Diagramm beschreibt die relevante IT Landschaft mit den verschieden Komponenten und ihren vorgesehenen Interaktionen.  

![deployment](images/deployment.png)


#### das Klassendiagramm

Das Klassendiagrmm beschreibt den Aufbau und die Beziehungen von Klassen. Es ist eines der gebräuchlisten Diagramme in der OO da es in einem Direkten Zusammenhang mit der Implementierung der Software steht. Zentrale Elemente des Klassendiagramms sind die Klasse und das Interface. 

![class1](images/classDiagramm1.png)

Klassen sind Typen. Klassen können von anderen Klassen Erben, damit drückt sich ein X ist ein Y aus. Interfaces sind ebenfalls Typen. Interfaces können einander erweitern, ein anderes Wort für Erben. Und ein Interface kann von einer Klasse implementiert werden. Damit ist die Klasse auch den Type den das Interface darstellt.

![class2](images/classDiagrammAss.png)
 
Beziehungen von Klassen zueinander werden als Assoziationen bezeichnet. Assoziationen können gerichtet sein, d.h. man kann von einer Instanz A zu einer Instanz Z „navigieren“, sie können etwas über den Lebens Zyklus der Kind Objekte aussagen(Komposition bedeutet das die Kinder mit dem Elternobjekt sterben, Shared das ihr Lebenszyklus unabhängig vom Elternobjekt ist).
#### das Objektdiagramm

Im Objekt Diagramm werden erstellte Exemplare der Klassen dargestellt. Die im Objekt Diagramm werden Instanzen von Klassen mit ihren Attribut werten dargestellt. 

![instance](images/instanceDiagramm.png)

 
#### das Kompositionsstrukturdiagramm (auch: Montagediagramm)

#### das Komponentendiagramm

Das Komponeten Diagramm beschreibt das Software System in einer groben Granularität, es beschreibt die Struktur der Interaktionen der verschiedenen Komponeten miteinander. Unter einer Komponete versteht man die Zusammenfassung einer Funktionalität. 

![profil](images/component-diagram-overview.png)

#### das Profildiagramm

Ein Profil ist die Möglichkeit UML, um Fachspezifische Eigenschaften, zu erweitern. So können Eigenschaften die nicht in UML vorgesehen sind in dem Modell spezifiziert werden. 

Es ist ein recht einfaches Diagramm, das im Prinzip aus zwei Diagramm Elementen, den Stereotyp und der Metaklasse.

Der Stereotype erweitert eine Metaklasse um Eigenschaften.
Eine Metaklasse ist ein Modellelement aus dem UML Metamodel auf die ein Stereotype angewendet werden kann.

![profil](images/contracts.profile.png)



### Verhaltes orientierte Diagramme

Aufgabe der Verhaltensorientieren Diagramme ist die Beschreibung der Verhaltensaspekte des Software Systems.

#### das Aktivitätsdiagramm

Das Aktivitätsdiagramm stellt den Ablauf von Aktivitäten in einem Softwaresystem dar. Das Einsatzgebiet kann vom Logik Fluss einer Methode bis zu einem groben Überblick über die allgemeinen Aktivitäten.

![activity](images/activity.png)

#### das Anwendungsfalldiagramm (auch: Use-Case o. Nutzfalldiagramm genannt)

Das use-case Diagramm ist eine gebräuchlich Form die Anwendungsfälle der Software zu abstrakt zu beschreiben. Es besteht aus Anwendungsfälle die von sog. Actoren ausgeführt werden. Diese Use-cases können untereinander Beziehungen haben, sie können voneinander abhängig sein, ein Use-Case kann einen anderen Use-Case auch erweitern.

![use-case](images/use-case.png)

#### das Zustandsdiagramm

Das Zustandsdiagramm beschrieb eine Zustandsautomaten. Die Übergänge von einem zu einem anderen Zustand können beschreiben werden.

![state](images/state-maschine.png)


#### das Kommunikationsdiagramm

Im Kommunikationsdiagramm werden die Nachrichten die die Komponenten einander schicken. Nachrichten sind Pfeile die mit einer Sequenznummer versehen werden können.

![state](images/communication-diagram-overview.png)


#### das Sequenzdiagramm

Das Sequenz Diagramm beschreibt den Zeitlichen Ablauf einer Menge von beteiligten Objekten. 

![state](images/sequnce.png)



#### das Interaktionsübersichtsdiagramm

Das Interaktionsübersichts Diagramm ist eine Kombination des Sequenz und des Aktivitätsdiagramm.

![state](images/communication-diagram-overview.png)


#### das Zeitverlaufsdiagramm




## MDE/MDA (Model getriebene Entwicklung)

Die Modellgetriebene Entwicklung unterstützt die Modelierung der Software dahingehen als es möglich ist die Modelle als Vorlagen für Textgeneratoren zu benutzen die dann z.B. Quelltext Generieren.


## Software die UML unterstützt

Papyrus (Eclipse Plugin) https://eclipse.org/papyrus/
Eclipse ist eine Plattform nicht nur zur einfachen Java Entwicklung, unter dem Dach der Eclipse Foundation gibt es eine Menge Projekte die sich mit der Modellierung beschäftigen. (https://eclipse.org/modeling/) Hier ist besonders das Acceleo Projekt (http://www.eclipse.org/acceleo/), ein auf dem MTL (Model to Text Language) basierender Codegenerator und ATL (http://www.eclipse.org/atl/) eine Model Transformations Sprache hervor zu heben.


## Weiterführende Quellen

http://www.uml-diagrams.org

http://www.torsten-horn.de/techdocs/uml.htm




----

images from wikipedia



