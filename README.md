# Work In Progress ! Do not rely on this doc !

#Poppy docs 

**All the documentation you need to use the Poppy robots**

This documentation contains:

* General Poppy project description
* Assembly guides for Poppy Humanoid, Poppy Torso and Poppy Ergo Jr
* Documentations of Poppy's libraries:
    * Pypot
    * Poppy creatures
    * poppy_humanoid
    * poppy_torso
    * poppy_ergo_jr


## Links of version in development
* [html](http://poppy-project.github.io/poppy-docs/)  
* [pdf](http://poppy-project.github.io/poppy-docs/Poppyprojectdocumentation.pdf)

## Install Sphinx and generate the doc

Install sphinx:

`pip install sphinx sphinxjp.themes.basicstrap`

Install commonmark to be able to use markdowns in Sphinx:

`pip install commonmark recommonmark`

If you want to generate Latex or pdf documents:

`sudo apt-get install -qq texlive texlive-latex-extra dvipng`


Then, to create HTML doc:

`make html`

Your files are in `_build\html`

To create a pdf doc:

`make latexpdf`

Your files are in `_build\latex`

To recreate the API doc of a module, use sphinx-apidocs. For example when doc is in poppy-humanoid/poppy-humanoid/software/poppy_humanoid, output path is poppy-humanoid/doc and you want to overwrite previous doc (-f option):

`sphinx-apidoc -f  -o poppy-humanoid/doc poppy-humanoid/poppy-humanoid/software/poppy_humanoid`

Translation:

Follow the instructions of [http://sphinx-doc.org/latest/intl.html](http://sphinx-doc.org/latest/intl.html) . Warning! I had to use version 11 of transifex-client to uploads my docs (pip install transifex-client==0.11.1.beta)

Transifex project is poppy-docs : https://www.transifex.com/poppy-project/poppy-docs/






