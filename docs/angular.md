```eval_rst
:github_url: https://github.com/scholchr/webdevbook/tree/master/source/angular.md
```

# Angular

## Häufige Tasks

Angular Framework aktualisieren `ng update`

Veraltete Pakete anzeigen `npm outdated -l`

## Angular Component Collections

* [Clarity UI](https://vmware.github.io/clarity/documentation/)
* [PrimeNG](https://www.primefaces.org/primeng/)

* [Material](https://material.io)
    * [Floating Action Button](https://material.io/components/web/catalog/buttons/floating-action-buttons/)
    * [Floating Action Button Guideline](https://material.io/guidelines/components/buttons-floating-action-button.html)

## ngOnInit vs. Constructor

## Router

### Alle Routen ausgeben

`console.log('configured routes: ', this.router.config);`

## ServiceWorker

### Unterverzeichnis
* **Problem**: ServiceWorker wird nicht aufgerufen, wenn sich die Angular-App in einem Unterverzeichnis 
(bspw. `https://dev.hksinformatik.de/webwib/`). Das Problem ist möglicherweise schon durch [Issue 19524](https://github.com/angular/angular/issues/19524>) gelöst

* **Lösungsansatz**: In `src\app.module.ts` dem ServiceWorker explizit das Unterverzeichnis angeben: 
`ServiceWorkerModule.register('/webwib/ngsw-worker.js', ...`.

* Bei einer falschen Pfadangabe erscheint die Fehlermeldung: *Uncaught (in promise) DOMException: Failed to register a 
ServiceWorker: The script has an unsupported MIME type ('text/html').*

## Testing

### Grundaufbau
```
describe("A suite", function() {
  it("contains spec with an expectation", function() {
    expect(true).toBe(true);
  });
});
```
* `describe` gruppiert zusammengehörige Test (Specs) in einer Testsuite und beschreibt diese anhand eines Stringparameters.
* `it` ist ein einzelner Test und beinhaltet eine oder mehrere Erwartungen (expectations) mittels `expect`
* Setup und Teardown
  * `beforeEach` wird vor jedem Test aufgerufen
  * `afterEach` wird nach jedem Test aufgerufen
  * `beforeAll` wird einmalig vor dem Aufrufen aller Test ausgeführt
  * `afterAll` wird einmalig nach dem Aufrufen aller Test ausgeführt

### Deaktivieren von Tests
* `xdescribe` deaktiviert die jeweilige Testsuite mitsamt ihrer Tests
* `xit` deaktiviert einzelne Tests
* `fdescribe` fokussiert die jeweilige Testsuite und führt nur diese aus
* `fit` fokussiert einen einzelnen Test und führt nur diesen aus


## Probleme

### Node-Sass kann die Python Ausführungsdatei nicht finden
* **Problem**: *node-sass can't find python executable*
* **Lösung**: `npm install -g --production windows-build-tools`

### Fehlermeldung beim Anlegen neuer Komponenten per ``ng``
* **Problem**: Beim Ausführen von `ng generate component new-component` erscheint: *More than one module matches. Use skip-import option to skip importing the component into the closest module.*
* **Lösung**: `ng g c new-component --module app` sofern das Hauptmodul `app.module.ts` ist.

## Sourcemaps
`ng serve --sourcemaps`