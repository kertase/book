# Einführung

> Anmerkung: Die zweite Edition ist auf English als Buch gedruckt und digital verfügbar  [The Rust Programming
> Language][nsprust] [No Starch
> Press][nsp].

[nsprust]: https://nostarch.com/rust
[nsp]: https://nostarch.com/

Willkommen zu *Die Rust Programmiersprache*, ein einführendes Buch über Rust.
Die Rust Programmiersprache hilft dir schneller, zuverlässige Computerprogramme zu schreiben.
Hohe Ergonomie-ebenen und niedrige Kontrollebenen sind oft widersprüchlich bei Programmsprachentwürfen; Rust stellt sich diesem Konflikt. Durch ausgleichen von leistungsstarken technischen Kapazitäten und eine gute Entwicklererlebnis, gibt Rust dir die Möglichkeit auf niedriger Kontrollebene Details (so wie Speichernutzung) ohne die ganzen Mühen die herkömmlich mit einer solchen Kontrollebene verbunden werden

## Rust ist für

Rust ist ideal für viele Leute für eine Vielfalt an Gründen. Laß uns ein paar der wichtigsten Gruppen betrachten.

### Entwicklerschaften

Rust stellt produktive Werkzeuge, für Kollaborationen von großen Entwicklerschaften mit variierenden Verständnis von Systemprogrammierung, zur Verfügung. Quelltext auf niedriger Ebene ist für subtile Programmierfehler anfällig, welche in den meisten anderen Sprachen nur durch umfangreiches Testen und vorsichtigen Quelltext Überprüfungen durch erfahrene Programmierer gefunden werden können. In Rust spielt der Kompilator die Rolle eines Torwächters in dem er Quelltext, mit schlüpfrigen Fehlern, unter anderem Nebenhäufigkeitsfehler ablehnt. Durch Zusammenarbeit mit dem Kompilator, kann die  Entwicklerschaft ihre Zeit auf die Logik des Programms konzentrieren statt nach Programmfehlern zu jagen.

Rust bringt auch Zeitgenössische Entwicklerwerkzeuge in die Welt der Systemprogrammierung:

* Cargo, der inbegriffene Abhängigkeitsverwalter und Erstzellwerkzeug macht das Hinzufügen,
  übersetzen, und verwalten von Abhängigkeiten schmerzlos und einheitlich quer durch das Rust
  Ökosystem.
* Rustfmt garantiert einen einheitlichen entwicklerübergreifenden Quelltextstil.
* Der Rust Sprachserver treibt die Integration in Integrierte Entwicklungsumgebung (IDE) 
  für Quelltextvervollständigung und inzeilige Fehlermeldungen an.

Durch nutzen dieser und anderer Werkzeuge im Rust Ökosystem, können Entwickler während des Schreiben von systemebenem Quelltext produktiv sein.

### Studenten

Rust ist für Studenten und andere die interessiert sind Systemkonzepte kennenzulernen. Durch das nutzen von Rust haben viele Themen wie Betriebssystem entwicklung kennengelernt. Die Gemeinschaft ist sehr Wiederkommend und gern bereit Fragen von Studenten zu beantworten. Durch Bemühungen wie dieses Buch, will die Rust Gemeinschaft Systemkonzepte zugänglicher zu mehr Leuten machen, insbesondere für die die noch im Programmiren unerfahren sind.

### Gesellschaften

Hunderte von kleinen Gesellschaften. groß oder klein, benutzen Rust in der Produktion für eine Vielfalt von Aufgaben. Diese Aufgaben beinhalten, Beifehlzeilenwerkzeuge, Netzdienste, DevOps Bereitstellung,  eingebettete Systeme, Audio und Video Analysen und Umschlüsselung, kryptographische Währungen, Bioinformatik, Suchmaschinen, Allesnetz,  Machinenlernen, und sogar bedeutend teile des Firefox Webbrowsers.

### Quelloffene Entwickler

Rust ist für die Leute die die Rust Programmiersprache, Gemeinschaft, Entwicklerwerkzeuge und Bibliotheken mit aufbauen wollen. Wir würden es lieben wen du der Rust Sprache beitragen würdest.

### Leute die Geschwindigkeit und Stabilität schätzen

Rust ist für Leute die sich nach Geschwindigkeit und Stabilität lechzen. Mit Geschwindigkeit meinen wir die Geschwindigkeit der Programme die man mit Rust erstellen und die Geschwindigkeit, mit der man diese Schreiben kann. Des Rusts Kompilators Überprüfungen sichert Stabilität durch das Hinzufügen von Funktionalitäten und durch Restrukturierung. Dies ist im Gegensatz, zu spröden veralteten Quelltext in Sprachen ohne diese Überprüfungen in denen der Entwickler oft angst Änderungen vorzunehmen, zu sehen. Durch Anstreben von kostenlose Abstraktionen einer hohen Funktionalitätsebene die sich zu einer niedrigen Quelltextebene übersetzt, die ebenso schnell wie manuelle geschriebener Quelltext ist, bemüht Rust sicheren Quelltext auch schnell zu machen.

Die Rust Sprache erhofft sich auch viele andere Nutzer zu unterstützen; die hier genannt Nutzer sind lediglich einige der größten Interessenvertreter. Alles in Allem betratet, ist Rusts größte Zielsetzung die Kompromisse die Entwickler Jahrzehnte lang hinnehmen mußten, durch Bereitstellen von Sicherheit *und* Produktivität, Geschwindigkeit *und* Ergonomie, zu beseitigen.

## Für wem ist dieses Buch

Dieses Buch nimmt an das du schon mal in einer anderen Sprach Quelltext geschrieben hast, aber macht keine Annahme darüber in welcher. Wir versuch das Material so weitgehend wie möglich zugänglich für eine weite Vielfalt an Entwicklungshintergründen zu gestalten. Wir verbringt nicht viel Zeit mit den Fragen was Programmieren *ist* oder wie darüber nachdenkt. Falls du vollkommen neu im Programmieren bist, wärst du besser aufgehoben ein Buch zu lesen das eine Einführung in die enthält.

## Wie nutzt man dieses Buch

Im Allgemeinen, nimmt dieses Buch an das es in Reihenfolge von vorn nach hinten gelesen wird. Spätere Kapitel bauen auf Konzepte aus früheren Kapiteln, und frühere Kapitel könnten nicht zu sehr ins Detail in manchen Themen gehen; Typischerweise werden diese in einem späteren Kapitel nochmal betrachtet.

Du wirst zwei Typen von Kapiteln in diesem Buch begegnen: Konzept Kapitel und Projektkapitel. In Konzeptkapiteln, wirst du über einen Aspekt von Rust lernen. In Projektkapiteln,  werden wir kleine Programme zusammen erstellen, durch Anwendung des zuvor gelernten. Kapitel 2, 12 und 20 sind Projektkapitel; der sind Konzeptkapitel.

Chapter 1 explains how to install Rust, how to write a Hello, world! program,
and how to use Cargo, Rust’s package manager and build tool. Chapter 2 is a
hands-on introduction to the Rust language. Here we cover concepts at a high
level, and later chapters will provide additional detail. If you want to get
your hands dirty right away, Chapter 2 is the place for that. At first, you
might even want to skip Chapter 3, which covers Rust features similar to those
of other programming languages, and head straight to Chapter 4 to learn about
Rust’s ownership system. However, if you’re a particularly meticulous learner
who prefers to learn every detail before moving on to the next, you might want
to skip Chapter 2 and go straight to Chapter 3, returning to Chapter 2 when
you’d like to work on a project applying the details you’ve learned.

Chapter 5 discusses structs and methods, and Chapter 6 covers enums, `match`
expressions, and the `if let` control flow construct. You’ll use structs and
enums to make custom types in Rust.

In Chapter 7, you’ll learn about Rust’s module system and about privacy rules
for organizing your code and its public Application Programming Interface
(API). Chapter 8 discusses some common collection data structures that the
standard library provides, such as vectors, strings, and hash maps. Chapter 9
explores Rust’s error-handling philosophy and techniques.

Chapter 10 digs into generics, traits, and lifetimes, which give you the power
to define code that applies to multiple types. Chapter 11 is all about testing,
which even with Rust’s safety guarantees is necessary to ensure your program’s
logic is correct. In Chapter 12, we’ll build our own implementation of a subset
of functionality from the `grep` command line tool that searches for text
within files. For this, we’ll use many of the concepts we discussed in the
previous chapters.

Chapter 13 explores closures and iterators: features of Rust that come from
functional programming languages. In Chapter 14, we’ll examine Cargo in more
depth and talk about best practices for sharing your libraries with others.
Chapter 15 discusses smart pointers that the standard library provides and the
traits that enable their functionality.

In Chapter 16, we’ll walk through different models of concurrent programming
and talk about how Rust helps you to program in multiple threads fearlessly.
Chapter 17 looks at how Rust idioms compare to object-oriented programming
principles you might be familiar with.

Chapter 18 is a reference on patterns and pattern matching, which are powerful
ways of expressing ideas throughout Rust programs. Chapter 19 contains a
smorgasbord of advanced topics of interest, including unsafe Rust and more
about lifetimes, traits, types, functions, and closures.

In Chapter 20, we’ll complete a project in which we’ll implement a low-level
multithreaded web server!

Finally, some appendixes contain useful information about the language in a
more reference-like format. Appendix A covers Rust’s keywords, Appendix B
covers Rust’s operators and symbols, Appendix C covers derivable traits
provided by the standard library, and Appendix D covers macros.

There is no wrong way to read this book: if you want to skip ahead, go for it!
You might have to jump back to earlier chapters if you experience any
confusion. But do whatever works for you.

An important part of the process of learning Rust is learning how to read the
error messages the compiler displays: these will guide you toward working code.
As such, we’ll provide many examples of code that doesn’t compile along with
the error message the compiler will show you in each situation. Know that if
you enter and run a random example, it may not compile! Make sure you read the
surrounding text to see whether the example you’re trying to run is meant to
error. In most situations, we’ll lead you to the correct version of any code
that doesn’t compile.

## Quelltext

Die Quelldateien aus denen dieses Buch generiert wurde können auf
[GitHub][book] gefunden werden. 

[book]: https://github.com/rust-lang/book/tree/master/second-edition/src
