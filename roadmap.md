[index](index.md)

### mhus-parent 3.6.3 (mhus-lib 3.6.3 / mhus-osgi-tools 1.6.2)

* Reorganization of the project content
* Split osgi-tools-services into api and implementation (left 'services') parts. Move jms related from services into the jms sub project (package names are changed)
* Move vaadin out of mhus-lib into a separate project mhus-vaadin. Move the bridge projects from mhus-osgi-tools also into the new project
* Reactivate removed mongo classes and create a new project mhus-mongo. I fork morphia into a sub project to prepare it to work with xdb annotations and UUID instead of ObjectId

Notes for mhus-vaadin:

* Version 1.* is vaadin 8 compatible
* Version 2.* will be vaadin 13 compatible

### mhus-lib 3.3.2:

* Simple asynchrone en/decryption (non standard encryption for simple secrets like passwords in property files)
* Basic classes for security block style text files
* Reorganise Karaf JMS Services. Simplify and cleanup DataChannel implementation

### mhus-osgi-tools 1.3.2:

* Add tools for encryption, if necessary create a bouncycastle port

encryption:

* Add basic encryption and signing services and handling

### mhus-lib 3.4:

* Merge functionality with external libraries like <https://github.com/google/guava> or apache commons libraries.
* Move most of the Karaf commands into mhus-osgi-tools

### mhus-osgi-tools 1.4:

* Rename the artefacts to separate osgi, karaf/felix and equinox bundles
* Switch to karaf 4.1.*

### mhus-sop 1.0:

* Implement operations local and over JMS
* Implement RESTlesser interface
* Implement the AAA system
* Basic database access and DB AAA
