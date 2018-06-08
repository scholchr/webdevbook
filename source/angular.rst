:github_url: https://github.com/scholchr/webdevbook/blob/master/source/angular.rst

=======
Angular
=======

Häufige Tasks
=============

Angular Framework aktualisieren ``ng update``

Veraltete Pakete anzeigen ``npm outdated -l``


Angular Component Collections
=============================

* `Clarity UI <https://vmware.github.io/clarity/documentation/>`_

* `PrimeNG <https://www.primefaces.org/primeng/>`_

* `Material <https://material.io>`_

    * `Floating Action Button <https://material.io/components/web/catalog/buttons/floating-action-buttons/>`_

    * `Floating Action Button Guideline <https://material.io/guidelines/components/buttons-floating-action-button.html>`_


ServiceWorker
=============

#. Unterverzeichnis

    * **Problem**: ServiceWorker wird nicht aufgerufen, wenn sich die Angular-App in einem Unterverzeichnis (bspw. ``https://dev.hksinformatik.de/webwib/``). Das Problem ist möglicherweise schon durch `GitHub Issue 19524 <https://github.com/angular/angular/issues/19524>`_ gelöst

    * **Lösungsansatz**: In ``src\app.module.ts`` dem ServiceWorker explizit das Unterverzeichnis angeben: ``ServiceWorkerModule.register('/webwib/ngsw-worker.js', ...``.

    * Bei einer falschen Pfadangabe erscheint die Fehlermeldung: ``Uncaught (in promise) DOMException: Failed to register a ServiceWorker: The script has an unsupported MIME type ('text/html').``


Probleme
========

#. Node-Sass kann die Python Ausführungsdatei nicht finden

    * **Problem**: *node-sass can't find python executable*

    * **Lösung**: ``npm install -g --production windows-build-tools``


#. Fehlermeldung beim Anlegen neuer Komponenten per ``ng``

    * **Problem**: Beim Ausführen von ``ng generate component new-component`` erscheint: *More than one module matches. Use skip-import option to skip importing the component into the closest module.*

    * **Lösung**: ``ng g c new-component --module app`` sofern das Hauptmodul ``app.module.ts`` ist.



Sourcemaps
==========

``ng serve --sourcemaps``