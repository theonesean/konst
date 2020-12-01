# konst

konst is a command-line tool for polyglot developers to define constants and snippets across projects.

## Inspiration

The idea for this tool is from a conversation I had with a friend who is also a software developer:

**Jeff:**

	here's an ambitious project

	what about a tool or something

	a preprocessor kind of thing

	that lets you define constants across different languages

	so you can truly have just one place where that constant lives

**Sean:**

	could be a good command line tool

## Behavior

The constants would be defined in a `.konst` file in your home directory. You could annotate individual lines with the language or stack you’re using that constant for (say, `@php` or `@node`), or you could define blocks of constants for an individual language. 

When you’re creating a new projects, you can run konst init and it’ll do its best to infer the type of project you’re working on. You can also run konst init python to specify manually.

It will create a file in the root of the project (or a contextually valid location, like a `/constants` folder—this could also be configurable by language) with your constants that you can then include or import into your project wherever you want to
