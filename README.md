# cbs-variables-thesaurus: https://skosmos.odissei.nl/cbs
 
Jupyter notebook to generate linked data descriptions of the variables and columns in CBS microdata data designs. This script is run on the XML files describing the data designs, which are not public because of potential privacy issues.

The most recent, formal released version of the output is available at https://skosmos.odissei.nl/cbs. Note that this thesaurus is used within ODISSEI and SSHOC-NL related projects and has not been endorsed by CBS in any way.

The output is modelled as a SKOS Concept Scheme. In CBS terminology, the actual column-level descriptions are referred to as "context variables" and the more abstract, underlying conceptual variables as just "variables".  The latter serve as broader concepts for the context variables that are at the bottom level. Note that no further structure has been added. As a consequence, there are over 10.000 concepts at the highest level of the thesaurus, so we choose not to model these explicitly as skos:topConcept because many SKOS implementations do not handle such large numbers of top concepts really well.

Older versions of the thesaurus use the https://portal.odissei-data.nl/data/cbs/variableThesaurus/ namespace.

At the time of writing, we have switched to using https://w3id.org/odissei/cv/cbs/variableThesaurus/.