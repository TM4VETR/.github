# Text Mining 4 VET Research

This is a preliminary collection of Text Mining steps useful for VET research.

Every part uses stout and stdin to forward data to the next step, use command line arguments to pass additional parameters. Only Readers, as first step of a pipeline, and Writer, as last step of the pipeline, differ. 

Attention: Some arguments are currently missing, for example defining typesystem. 

Example pipeline:

```
#!/bin/bash

python3 GenericTextReader/reader.py --file testinput |  python3 SpacyNER/spacyner.py | python3 NECSVWriter/necsvwriter.py -o out.csv
```
See https://github.com/TM4VETR/ExamplePipelines.
