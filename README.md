# Handling sdf files

## Backgroud
  1. There is a standard for 'sdf' files, but each file writer has different issues with strings that mean specific spaces.
  2. In 'sdf' files, properties(keys) may exist in duplicates. In this case, when the package called 'RDKit' reads the 'sdf' file, the fuplicate properties are replaced with the value of the last duplicate property.

## Unresolved issues
  1. For the solution, if there are duplicate properties, all values are stacked, but the number of duplicates is differnt for each property, so the number of stacked values is different for each property.
