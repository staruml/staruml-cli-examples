# StarUML CLI Examples

> Note that StarUML CLI is supported from the version 5.x

To see help:

```sh
$ staruml --help
```

## EJS examples

To run examples, first clone this repository:

```sh
$ git clone https://github.com/staruml/staruml-cli-examples.git
$ cd staruml-cli-examples
```

__Simple HTML Page__

Generate a simple HTML page showing all UMLClasses.

```sh
$ staruml ejs models/library.mdj \
  -t ejs/class-list.ejs \
  -o class-list.html
```

__Simple Java Class__

Generate Java class files for all UMLClasses.

```sh
$ staruml ejs models/library.mdj \
  -t ejs/java-class.ejs \
  -s @UMLClass \
  -o "out/<%=filenamify(element.name)%>.java"
```
