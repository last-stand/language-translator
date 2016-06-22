= Language Translator

Language translator translates *English* language sentences into *Hindi*. It uses javascript parser link:Jison[http://zaa.ch/jison/] for parsing English sentences and then convert it to Hindi sentenses.

== Settings to run project:

Run the *npm install*.

=== 1. grammar.jison :

In this file we give context-free grammar. After executing this file with Jison, it outputs a JavaScript file(in this case grammar.js) capable of parsing the language described by that grammar. We can use the generated script to parse inputs and accept, reject or perform actions. To generate script from grammar.jison file run the give command to the terminal:
----
jison grammar.jison
----

=== 2. lang_translater :

This is the main file where we use our generated JavaScript file by grammar.jison. It takes as file with valid English sentences(here it is *sampleText*)in it and performs translation on it. To run this use the given command to the terminal:
----
node lang_translter.js sampleText
----
