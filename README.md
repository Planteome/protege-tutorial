[![Build Status](https://travis-ci.org/Planteome/protege-tutorial.svg?branch=master)](https://travis-ci.org/Planteome/protege-tutorial)
[![DOI](https://zenodo.org/badge/13996/Planteome/protege-tutorial.svg)](https://zenodo.org/badge/latestdoi/13996/Planteome/protege-tutorial)

Planteome Protege/OWL Course, Corvalis, November 2015

The main goal of the tutorial is have participants understand the
principles of developing OWL ontologies, how classes can be combined
together, how a reasoner can be used for auto-classification and
error-checking.


# Intro

 * [presentations/Protege-OWL-Intro.pptx](presentations/Protege-OWL-Intro.pptx)

# Tutorial

The tutorial text is here

 * [presentations/protege_planteome_tutorial.doc](presentations/protege_planteome_tutorial.doc)

We will work through the following examples. Each section
introduces new constructs and/or concepts.

For each section, the instructor will first demonstrate some
examples. The students will then follow the instructions in the
README.txt file for the section. After completion, the students can
exchange OWL files and review one another's work.

## Basics

 * [basic-subclass](basic-subclass)

    Task: build a basic hierarchy
    Constructs: SubClass, annotations
    Uses reasoner: None
    Ontology: cell component (subset)

 * [basic-restriction](basic-restriction)

    Task: add part_of restrictions to ontology
    Constructs: SubClass, ObjectProperty, "some" (existential restriction)
    Uses reasoner: None
    Ontology: cell component (subset)

 * [basic-dl-query](basic-dl-query)

    Task: perform queries using class expressions
    Constructs: and, some
    Uses reasoner: Hermit
    Ontology: cell component (subset)

 * [basic-classification](basic-classification)

    Task: use reasoner to build hierarchy
    Constructs: SubClass, "some", Equivalence, "and" (intersection)
    Uses reasoner: Hermit
    Ontology: cell component (subset)

## Optional

 * [disjoint-expressions](disjoint-expressions)

    Note: the instructor may use this one as an example
    Task: create spatial disjointness axioms without the use of helper "X part" classes
    Constructs: General Axioms
    Uses Reasoner: Hermit

 * [basic-disjoint](basic-disjoint)

    Task: find problems in ontology
    Constructs: DisjointWith
    Uses reasoner: Hermit
    Ontology: cell component (subset)

 * [taxon-union](taxon-union)

    Task: create taxonomic grouping classes
    Constructs: or, not
    Uses reasoner: Hermit
    Ontology: NCBITaxon (subset)

 * [occurs-in](occurs-in)

    Note: the instructor may use this one as an example
    Task: examine how to compose relations to get desired inferences
    Constructs: property chains
    Uses Reasoner: Hermit
    Ontology: BP and CC (subset)

 * [regulation-classification](regulation-classification)

    Task: examine how to compose relations to get desired inferences
    Constructs: property chains
    Uses Reasoner: Hermit
    Ontology: BP (subset)

 * [response-to-stimulus](response-to-stimulus)

    Task: use an external ontology for classification
    Constructs: owl:imports
    Uses Reasoner: Hermit
    Ontology: BP (Subset) and import of Stimulus ontology

 * [advanced-metabolism](advanced-metabolism)

    Note: We may skip this one until day 2
    Task: use an external ontology for classification, together with helper axioms
    Constructs: owl:imports, property chains
    Uses Reasoner: Hermit or Elk
    Ontology: BP (Subset) and import of Chebi plus extras


 * [obo-owl-classification](obo-owl-classification)

    Task: edit an ontology in OE and classify in Elk
    Uses Reasoner: Hermit
    Requires: OE 2.1.1beta4 or higher
     


