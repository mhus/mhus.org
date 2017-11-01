mhus-lib 3.3.2:

* Simple asynchrone en/decryption (non standard encryption for simple secrets like passwords in property files)
* Basic classes for security block style text files
* Reorganise Karaf JMS Services. Simplify and cleanup DataChannel implementation

mhus-osgi-tools 1.3.2:

* Add tools for encryption, if necessary create a bouncycastle port

encryption:

* Add basic encryption and signing services and handling

mhus-lib 3.4:

* Merge functionality with external libraries like <https://github.com/google/guava> or apache commons libraries.
* Move most of the Karaf commands into mhus-osgi-tools

mhus-osgi-tools 1.4:

* Rename the artefacts to separate osgi, karaf/felix and equinox bundles

mhus-sop 1.0:

* Implement operations local and over JMS
* Implement RESTlesser interface
* Implement the AAA system
* Basic database access and DB AAA
