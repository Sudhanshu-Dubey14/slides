% Documentation using Doxygen 
% Sudhanshu Dubey
% 27th July 2019

## Why Documentation?

1. To help you, *the creator*
1. To help him/her, *the contributor*
1. To help they, *the users*

## How Documentation?

1. [A separate manual](https://www.freecadweb.org/wiki/index.php?title=Main_Page)
1. **Using comments**
1. Git commits?

## Doxygen

> [Doxygen](http://doxygen.nl/index.html) is the de facto standard tool for generating documentation from annotated C++ sources.

- Download doxygen from [here](http://doxygen.nl/download.html#gitrepos)
- And then [install](http://doxygen.nl/manual/install.html) it.

## Why Doxygen?

1. Supports *lots* of languages
1. Easy to use, configure and customise (Because of **FOSS**)
1. From comment to manual
	- Easy to update
	- Synchronised documentation

## Where Doxygen?

- Small Projects
- Medium Projects
- Large Projects
- All "Projects"

## How Doxygen?

- Create sample configuration file using ``doxygen -g``
- Modify parameters like:
	- ``PROJECT_NAME``
	- ``PROJECT_BRIEF``
	- ``OUTPUT_DIRECTORY``
	- ``INPUT``
	- etc
- [Document your code](http://doxygen.nl/manual/docblocks.html)

## So let's do it!!

**Special Recommendation**: You can us a Markdown file as you main page by setting ``USE_MDFILE_AS_MAINPAGE`` to the md file.
