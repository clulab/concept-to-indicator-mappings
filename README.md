# Mappings between high-level concepts and indicators

To bridge the gap between the high-level concepts extracted by machine readers
and the lower-level variables required for expert models, it is proposed to
build an 'intermediate ontology' of indicators.

This repository contains mappings between high-level concepts and indicators,
expressed in the human-readable YAML format. Each concept can have multiple
indicators, and indicators can be shared across concepts.

We eagerly solicit the input of domain experts to collaboratively construct and
curate this set of mappings.

# Format

The format of the mappings file is as shown below:

```yaml
- concept:
  - indicators:
    - indicator_1
    - indicator_2
    - indicator_3
```

For example, conflict could be represented as:

```yaml
- food_security:
  - indicators:
    - Global_food_security_index
```

**Note**: Please use underscores in lieu of spaces.

# Extensions

It is possible that we may need to extend this format to be useful for modelers,
perhaps with links to data sources, etc.  We enthusiastically welcome
suggestions!

# Contributing

You can contribute in two ways:

- You can fork this project, make changes in your local copy, and submit a pull
    request.
- You can email Mihai at `msurdeanu AT email DOT arizona
  DOT edu` to request to be added to the repository as a contributor.
