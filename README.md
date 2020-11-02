# Maven Module Properties Demo
This demo shows how to make properties from one module available in others

## Motivation
If you want to delay processing from one module and do it in another, some of the context properties are needed.
An example of this is delaying a `deploy`, until a stub / proxy has been added to an artifact.

## Example Use Case
This example skips the `install` goal in module 1, and uses the `install-file` goal to do it in module 2.
To do this the properties are saved for later use.
