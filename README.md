# schema-org-entity-relational-diagrams

Some truly terrible (but real and existing) ER diagrams for the schema.org model

Use these at your own risk as the accuracy of the information is not guaranteed. Rely on the official schema.org documentation as the primary source of information.


## Known issues

- `3DModel` is missing.
- Predicates which have a range of more than one class aren't serialised properly - they get listed as a `stringlist` and the related classes don't show up on the diagram. See https://github.com/linkml/linkml/issues/2527.

## Generating the models

```bash
make
```

### Parallelisation

```bash
make -j 4 # (Or other appropriate parallelisation factor for your machine)
```

## License

License inherited from <https://github.com/schemaorg/schemaorg/>.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0
