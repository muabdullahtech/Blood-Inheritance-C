## Blood Type Inheritance Simulator

This program simulates genetic inheritance of blood type (A, B, or O) across multiple generations. It models individuals with two parents and two alleles (genes) that determine their blood type.

### Functionality

* Creates a family tree with a specified number of generations (`GENERATIONS` constant in code).
* Randomly assigns blood type alleles to the founding generation (parents of the child).
* Inherits alleles from parents for subsequent generations based on Mendelian inheritance principles (simplified for this simulation).
* Prints the family tree structure, indicating generation and blood type for each individual.

### Usage

1. Compile the program using a C compiler (e.g., `gcc blood_inheritance.c -o blood_inheritance`).
2. Run the executable (`./blood_inheritance`).
3. The program will generate and print a three-generation family tree with simulated blood types.

### Example Output

```
Child (Generation 0): blood type AA
Parent (Generation 1): blood type AB
Grandparent (Generation 2): blood type A
Grandparent (Generation 2): blood type B
```

**Note:** This is just one possible outcome. The program generates a random family tree with each execution.

### Code Structure

The code is organized into several functions:

* `create_family`: Creates a new individual with specified generations and assigns parents and alleles recursively.
* `print_family`: Prints the family tree structure with indentation and blood types.
* `free_family`: Frees memory allocated for individuals in the family tree.
* `random_allele`: Randomly generates a blood type allele (A, B, or O).

### Limitations

This program is a simplified simulation and does not account for all complexities of blood type inheritance, such as Rh factor or co-dominance. 
