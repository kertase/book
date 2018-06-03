# Die Rust Programmiersprache

[Vorwort](foreword.md)
[Einführung](ch00-00-introduction.md)

## Einstieg

- [Einstieg](ch01-00-getting-started.md)
    - [Installation](ch01-01-installation.md)
    - [Hallo, Welt!](ch01-02-hello-world.md)
    - [Hallo, Cargo!](ch01-03-hello-cargo.md)

- [Programmiere ein Ratespiel](ch02-00-guessing-game-tutorial.md)

- [Geläufige Programmierkonzepte](ch03-00-common-programming-concepts.md)
    - [Variablen und Wandelbarkeit](ch03-01-variables-and-mutability.md)
    - [Datentypen](ch03-02-data-types.md)
    - [Wie Funktionen funktionieren](ch03-03-how-functions-work.md)
    - [Kommentare](ch03-04-comments.md)
    - [Flußsteuerung](ch03-05-control-flow.md)

- [Besitz verstehen](ch04-00-understanding-ownership.md)
    - [Was ist Besitz?](ch04-01-what-is-ownership.md)
    - [Referenzen und borgen](ch04-02-references-and-borrowing.md)
    - [Ausschnitte](ch04-03-slices.md)

- [Struct⋅en benutzen um zusammenhängende Daten zu strukturieren ](ch05-00-structs.md)
    - [Definieren und initialisieren von Struct⋅en](ch05-01-defining-structs.md)
    - [Ein Beispielprogramm das Struct⋅en benutzt](ch05-02-example-structs.md)
    - [Methodensyntax](ch05-03-method-syntax.md)

- [Enum⋅en und Musterzuordnung](ch06-00-enums.md)
    - [Einen Enum definieren](ch06-01-defining-an-enum.md)
    - [Der `match` Flußsteuerungsoperator](ch06-02-match.md)
    - [Prägnante Flußkontrolle mit  `if let`](ch06-03-if-let.md)

## Grundlegende Rust Kompetenzen

- [Module](ch07-00-modules.md)
    - [`mod` und das Dateiensystem](ch07-01-mod-and-the-filesystem.md)
    - [Sichtbarkeit mit `pub` steuern](ch07-02-controlling-visibility-with-pub.md)
    - [Auf Namen in anderen Modulen verweisen](ch07-03-importing-names-with-use.md)

- [Geläufige Sammlungen](ch08-00-common-collections.md)
    - [Vektoren](ch08-01-vectors.md)
    - [Zeichenketten](ch08-02-strings.md)
    - [Streuwerttabelle](ch08-03-hash-maps.md)

- [Fehlerbehebung](ch09-00-error-handling.md)
    - [Unbehebbare Fehler mit `panic!`](ch09-01-unrecoverable-errors-with-panic.md)
    - [Behebbare Fehler mit `Result`](ch09-02-recoverable-errors-with-result.md)
    - [`panic!`⋅en oder nicht `panic!`⋅en](ch09-03-to-panic-or-not-to-panic.md)

- [Generische Typen, Eigenschaften und Lebensdauer](ch10-00-generics.md)
    - [Generische Datentypen](ch10-01-syntax.md)
    - [Eigenschaften: gemeinsames Verhalten definieren](ch10-02-traits.md)
    - [Überprüfen von Referenzen mit Lebensdauer](ch10-03-lifetime-syntax.md)

- [Proben](ch11-00-testing.md)
    - [Proben schreiben](ch11-01-writing-tests.md)
    - [Proben laufen lassen](ch11-02-running-tests.md)
    - [Probengestaltung](ch11-03-test-organization.md)

- [Ein I/O Projekt: Ein Zeilenbefehlsprogramm erstellen](ch12-00-an-io-project.md)
    - [Zeilenbefehlsargumente übernehmen](ch12-01-accepting-command-line-arguments.md)
    - [Eine Datei einlesen](ch12-02-reading-a-file.md)
    - [Restrukturierung um Modularität und Fehlerbehebung zu verbessern](ch12-03-improving-error-handling-and-modularity.md)
    - [Entwicklung der Funktionalität der Bibliothek mit probengetriebener Entwicklung](ch12-04-testing-the-librarys-functionality.md)
    - [Mit Umgebungsvariablen arbeiten](ch12-05-working-with-environment-variables.md)
    - [Writing Error Messages to Standard Error Instead of Standard Output](ch12-06-writing-to-stderr-instead-of-stdout.md)

## Thinking in Rust

- [Funktionale Sprachen Funktionalitäten: Iteratoren und Funktionsabschlüsse ](ch13-00-functional-features.md)
    - [Funktionsabschlüsse: anonyme Funktionen die ihre Umgebung erfassen können](ch13-01-closures.md)
    - [Eine Serie von Elementen mit Iteratoren verarbeiten](ch13-02-iterators.md)
    - [Unser I/O Projekt verbessern](ch13-03-improving-our-io-project.md)
    - [Leistung Vergleichen: Schlaufen geg. Iteratoren](ch13-04-performance.md)

- [Mehr über Cargo und Crates.io](ch14-00-more-about-cargo.md)
    - [Erstellungen mit Veröffentlichungsprofilen anpassen](ch14-01-release-profiles.md)
    - [Eine Crate auf Crates.io veröffentlichen](ch14-02-publishing-to-crates-io.md)
    - [Cargo Arbeitsraum](ch14-03-cargo-workspaces.md)
    - [Binärdateien von Cargo mit `cargo install` installieren](ch14-04-installing-binaries.md)
    - [Cargo mit selbsterstellten Befehlen erweitern](ch14-05-extending-cargo.md)

- [Intelligente Zeiger](ch15-00-smart-pointers.md)
    - [`Box<T>`  Zeigt auf Daten auf dem Heap und hat ein bekannte Größe](ch15-01-box.md)
    - [Der `Deref` Trait ermöglicht Zugriff auf die Daten über ein Referenz](ch15-02-deref.md)
    - [Der `Drop` Trait läßt bei der Säuberung Kode laufen](ch15-03-drop.md)
    - [`Rc<T>`,  der Referenz zählende intelligente Zeiger ](ch15-04-rc.md)
    - [`RefCell<T>` und das Muster der inneren Wandelbarkeit](ch15-05-interior-mutability.md)
    - [Erstellen von Referenzzyklen und leckender Speicher ist Sicher](ch15-06-reference-cycles.md)

- [Furchtlose Nebenläufigkeit](ch16-00-concurrency.md)
    - [Aktivitätsträger](ch16-01-threads.md)
    - [Nachrichtenweitergabe](ch16-02-message-passing.md)
    - [Gemeinsamer Zustand](ch16-03-shared-state.md)
    - [Erweiterbare Nebenläufigkeit: `Sync` und `Send`](ch16-04-extensible-concurrency-sync-and-send.md)

- [Objekt Orientierte Programmiereigenschaften von Rust](ch17-00-oop.md)
    - [Charakteristiken von Objektorientierten Sprachen](ch17-01-what-is-oo.md)
    - [Trait Objekte benutzen die Werte von verschiedenen Typen erlauben](ch17-02-trait-objects.md)
    - [Implementation eines objektorientierten Entwurfsmusters](ch17-03-oo-design-patterns.md)

## Erweiterte Themen

- [Muster gleichen der Struktur von Werten](ch18-00-patterns.md)
    - [Alle Stellen an den Muster genutzt werden können](ch18-01-all-the-places-for-patterns.md)
    - [Widerlegbarkeit: Ob ein Musterabgleich scheitern könnte](ch18-02-refutability.md)
    - [Die ganze Mustersyntax](ch18-03-pattern-syntax.md)

- [Fortgeschrittene Funktionalitäten](ch19-00-advanced-features.md)
    - [Unsicheres Rust](ch19-01-unsafe-rust.md)
    - [ Fortgeschrittene Lebendauer](ch19-02-advanced-lifetimes.md)
    - [Erweiterte Traits](ch19-03-advanced-traits.md)
    - [Fortgeschrittene Typen](ch19-04-advanced-types.md)
    - [ Fortgeschrittene Funktionen und Funktionsabschlüsse](ch19-05-advanced-functions-and-closures.md)

- [Abschließendes Projekt: einen mehrprozeßgestützten Webserver erstellen](ch20-00-final-project-a-web-server.md)
    - [Einen enizelprozeßgestützten Webserver](ch20-01-single-threaded.md)
    - [Unseren einzel- in einen mehrprozeßgestützten Server wandeln](ch20-02-multithreaded.md)
    - [Elegantes Herunterfahren und säubern](ch20-03-graceful-shutdown-and-cleanup.md)

- [Anhang](appendix-00.md)
    - [A - Schlüsselwörter](appendix-01-keywords.md)
    - [B - Operatoren und Symbole](appendix-02-operators.md)
    - [C - Ableitbare Eigenschaften](appendix-03-derivable-traits.md)
    - [D - Macros](appendix-04-macros.md)
    - [E - Übersetzungen](appendix-05-translation.md)
    - [F - Neueste Funktionalitäten](appendix-06-newest-features.md)
    - [G - Wie Rust hergestellt wird und „Nightly Rust“](appendix-07-nightly-rust.md)
