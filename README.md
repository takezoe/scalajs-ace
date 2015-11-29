scalajs-ace
===============

Static types for the [Ace](http://ace.c9.io/) editor for [Scala.js](http://www.scala-js.org/) programs.

Usage
-----

Add the following to your sbt build definition:

```scala
resolvers += "amateras-repo" at "http://amateras.sourceforge.jp/mvn/"

libraryDependencies += "com.scalawarrior" %%% "scalajs-ace" % "0.0.2"
```
then enjoy Ace in Scala.js!

```scala
import com.scalawarrior.scalajs.ace._

val editor = ace.edit("editor")
editor.setTheme("ace/theme/monokai")
editor.getSession().setMode("ace/mode/scala")

val text = editor.getValue()
```
