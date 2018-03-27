## How to install/deploy

[![Build Status](https://vertx.ci.cloudbees.com/buildStatus/icon?job=vert.x3-ext-parent)](https://vertx.ci.cloudbees.com/view/vert.x-3/job/vert.x3-ext-parent/)

~~~
% mvn install -DskipPkg
~~~

This is important otherwise it will fail (because it can't package what does not exists).

## Base parent pom for Vert.x extension projects

This parent pom extends the `io.vertx:vertx-parent` pom and provides common default configuration and execution for
data object generation and documentation.

### Api documentation

Documentation is generated from `src/main/asciidoc` in the `target/asciidoc/java` directory in _Asciidoc_ format at compilation
time and can be previewed using the Chrome _Asciidoctor.js_ plugin.

Full api documentation can be generated using `mvn site` phase, the _Asciidoc_ files are transformed to HTML and
the Api documentation (JavaDoc) is also generated in the _target/docs_ directory.
