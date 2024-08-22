# Automatic Derivation of Semantic Representations for Thai Serial Verb Constructions: A Grammar-Based Approach

This is the computational Thai grammar accompanying [this paper](https://aclanthology.org/2024.acl-srw.37/) which was presented at the ACL 2024 Student Research Workshop in Bangkok, Thailand.

## Abstract:

Deep semantic representations are useful for many NLU tasks (Droganova and Zeman, 2019; Schuster and Manning, 2016). Manual annotation to build these representations is time-consuming, and so automatic approaches are preferred (Droganova and Zeman, 2019; Bender et al. 2015). This paper demonstrates how rich semantic representations can be automatically derived for Thai Serial Verb Constructions (SVCs), where the semantic relationship between component verbs is not immediately clear from the surface forms. I present the first fully-implemented, unified analysis for Thai SVCs, deriving appropriate semantic representations (MRS; Copestake et al. 2005) from syntactic features, implemented within a DELPH-IN computational grammar (Slayden 2009). This analysis increases verified coverage of SVCs by 73% and decreases ambiguity by 46%.

## Grammar Files:

The lexical and phrase structure rules described in the paper and used to parse and analyze SVCs can be found in the thai.tdl file, and are instantiated in lrules.tdl and rules.tdl. thai.tdl also contains the additional head features and lexical types. Additional constraints (those that are common to all grammars) can be found in matrix.tdl, while the lexicon is found in lexicon.tdl. The tsdb folder contains the files and results for each testsuite (including regression tests, development data, and held-out data). 

## Installation and Usage:

The grammar can be compiled using the LKB grammar engineering environment, which can then be used to parse sentences and generate semantic representations. Full testsuites can be analyzed using [incr tsdb()]. More information about the LKB can be found [here](https://github.com/delph-in/docs/wiki/LkbTop) and installation instructions can be found [here](https://github.com/delph-in/docs/wiki/LkbInstallation).

The grammar was implemented within the LinGO Grammar Matrix framework, situated within the DELPH-IN consortium. More information about the Grammar Matrix can be found [here](https://matrix.ling.washington.edu/index.html) and [here](https://github.com/delph-in/docs/wiki/MatrixTop), while an overview of DELPH-IN can be found [here](https://github.com/delph-in/docs/wiki).
