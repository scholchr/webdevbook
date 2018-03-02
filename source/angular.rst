:github_url: https://github.com/scholchr/webdevbook/blob/master/source/angular.rst

=======
Angular
=======

Häufige Tasks
=============

Angular Framework aktualisieren ``ng update``


ServiceWorker
=============

#. Unterverzeichnis

 - **Problem**: ServiceWorker wird nicht aufgerufen, wenn sich die Angular-App in einem Unterverzeichnis (bspw. ``https://dev.hksinformatik.de/webwib/``). Das Problem ist möglicherweise schon durch `GitHub Issue 19524 <https://github.com/angular/angular/issues/19524>`_ gelöst

 - **Lösungsansatz**: In ``src\app.module.ts`` dem ServiceWorker explizit das Unterverzeichnis angeben: ``ServiceWorkerModule.register('/webwib/ngsw-worker.js', ...``.

 - .. warning:: Bei einer falschen Pfadangabe erscheint die Fehlermeldung: Uncaught (in promise) DOMException: Failed to register a ServiceWorker: The script has an unsupported MIME type ('text/html').
