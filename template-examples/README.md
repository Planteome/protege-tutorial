You will need python for this example.

Here we use [dead simple owl design patterns](https://github.com/dosumis/dead_simple_owl_design_patterns) to auto-generate a simple trait ontology.

The input here is a simple tabular file, [test1.csv](test1.csv) - this lists a set of traits together with 'slot fillers' for two variables, `entity` and `quality`

The transformation between the csv and the OWL file is provided by [simple_measurable.yaml](simple_measurable.yaml)

You can generate the ontology from the CSV like this:

    python3 apply-pattern.py -p simple_measurable.yaml -i test1.csv > mytest.owl

Now open this in Protege, switch on Elk, and look at the inferred hierarchy
