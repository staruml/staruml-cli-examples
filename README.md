# StarUML CLI Examples

> Note that StarUML CLI is supported from the version 5.x

```sh
$ git clone https://github.com/staruml/staruml-cli-examples.git
```

To see help:

```sh
$ staruml --help
```

## EJS examples

__Simple Class List__

- `ejs/class-list.ejs` 

```sh
$ staruml ejs models/library.mdj -t ejs/class-list.ejs -o class-list.html
```

__Simple Java Class__

```sh
$ staruml ejs models/library.mdj -t ejs/java-class.ejs -s @UMLClass -o "out/<%=element.name%>.java"
```