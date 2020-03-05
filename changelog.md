# Changelog
Alle nennenswerten Änderungen an diesem Projekt werden in dieser Datei dokumentiert.

Das Format basiert auf [Keep a Changelog](http://keepachangelog.com/de/1.0.0/)
und dieses Projekt hält sich an [Semantic Versioning](http://semver.org/lange/de/spec/v2.0.0.html).

## Unreleased


## [0.1.10] - 2020-03-05
### Added
- Git: `.gitgnore` Probleme und Lösungen hinzugefügt
- Javascript: 'function call' vs. 'arrow functions' und 'destr assignment' hinzugefügt

### Changed
- MkDocs Abhängigkeit von Version 1.0.4 auf 1.1 erhöht


## [0.1.9] - 2019-11-28
### Added
- `python.md` hinzugefügt

### Changed
- Umstieg von Sphinx auf MkDocs
- `angular.md`: Link zum Github Issue 19524 korrigiert


## [0.1.8] - 2019-08-13
### Changed
- `conf.py`:
  - Struktur und Inhalt an `sphinx-quickstart` Vorlage angepasst
  - Rechtschreibfehler korrigiert
- `index.md`:
  - Changelog Link verweist nun auf Github (per `eval_rst`)
  - Changelog Include auf von 20 auf 30 Zeilen erhöht
  - der Tabellenbeispiel-Kommentar ist nun 'Copy & Paste'-freundlicher

### Removed
- `conf.py`:
  - `source_suffix` entfernt
  - `sphinx.ext.todo`-Extension entfernt
  - `sphinx.ext.viewcode`-Extension entfernt
  - `'enable_eval_rst': True` im app hook entfernt, da es gleich dem Standardverhalten ist

## [0.1.7] - 2019-08-13
### Added
  - `conf.py`: `recommonmark` als Extension hinzugefügt

### Changed
- `conf.py`:
  - Anordnung der Import vereinfacht
  - `html_static_path` auskommentiert
  - `needs_sphinx` auf `2.1.2` gesetzt
  - `copyright` aktualisiert

### Removed
- `conf.py`:
  - `github_doc_root` entfernt
  - im 'app setup hook' unter `recommonmark_config` den `url_resolver` entfernt, da er fehlerhafte Links generiert hat
  - mehrere ungenutzte HTML Optionen entfernt


## [0.1.6] - 2019-08-13
### Added
- `conf.py`: für `pigar` nötige Module in hinzugefügt
- `python.md`: `pigar hinzugefügt`

### Changed
- `requirements.txt`: `pigar` als  Tool verwendet
- `python.md`: Struktur verändert

## [0.1.5] - 2019-05-08
### Added
- Angular Routenübersicht

### Changed
- Sphinx auf Version 2.0.1 aktualisiert
- conf.py angepasst (add_source_parser und add_source_suffix)

## [0.1.4] - 2019-01-22
### Added
- Angular Testing Grundlagen hinzugefügt

### Changed
- Sphinx auf Version 1.8.3 aktualisiert

## [0.1.3] - 2018-12-03
### Added
- sphinx-markdown-tables Erweiterung hinzugefügt
- Angular: 'ngOnInit vs. Contructor' Platzhalter hinzugefügt

### Changed
- recommonMark: 'CommonMark' (.md) anstatt 'reStructured Text' (.rst)
- Versionierungsformat von '0.0.x' nach '0.1.x' geändert, gemäß:
  [Semantic Versioning FAQ](https://semver.org/#how-should-i-deal-with-revisions-in-the-0yz-initial-development-phase)
- Reihenfolge der Indexdatei: Inhalt vor Changelog
- Changelogauszug vergrössert

## [0.1.2] - 2018-09-21
### Added
- Grails
  - URL Mappings

## [0.1.1] - 2018-09-21
### Added
- JavaScript
  - Promise
  - Oberservable
- Angular Basics
  - Component Collections
  - Service Worker im Unterverzeichnis
- CSS
  - Properties vergleichen