# cbs-variables-thesaurus: https://skosmos.odissei.nl/cbs
 
Jupyter notebook to generate linked data descriptions of the variables and columns in the CBS microdata data designs. This script is run on the XML files describing the data designs, which are not yet public because of potential privacy issues.

The most recent, formal released version of the output is available at https://skosmos.odissei.nl/cbs

The output is modelled as a SKOS Concept Scheme. In CBS terminology, the actual column-level descriptions are referred to as "context variables" and the more abstract, underlying conceptual variables as just "variables".  The latter are modelled as SKOS "Top Concepts", and serve as broader concepts for the context variables that are at the bottom level. Note that no further structure has been added. As a consequence, there are over 10.000 top concepts at the highest level of the thesaurus.

Older versions of the thesaurus use the https://portal.odissei-data.nl/data/cbs/variableThesaurus/ namespace.

At the time of writing, we are switching to using https://w3id.org/odissei/cv/cbs/variableThesaurus/.