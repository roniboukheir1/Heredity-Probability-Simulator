# Heredity-Probability-Simulator

This Python program simulates the heredity patterns of a trait passed down through a family over generations. It calculates the probabilities of family members having a specific gene and the associated trait based on their parents' genetic information.

Description

The simulator models the inheritance of a gene that can cause a particular trait. It takes into account the unconditional probabilities for having zero, one, or two copies of the gene and the probabilities of expressing a trait given the number of gene copies. The program also accounts for gene mutation, which can alter the inheritance pattern.

Features

- Load gene and trait data from a CSV file.
- Calculate joint probability distributions for gene and trait presence in a family.
- Update and normalize probabilities for each family member.
- Utilize a Monte Carlo simulation to estimate probabilities.

Usage

To run the heredity simulation, you need to provide a CSV file containing the family data. The CSV should have columns for `name`, `mother`, `father`, and `trait`. The `trait` column should contain `0` or `1` if the trait presence is known, or be blank if unknown.

bash

python heredity.py data.csv

Dependencies

Python 3.x
CSV module (included in standard Python library)
itertools module (included in standard Python library)
sys module (included in standard Python library)

Data Format

Name, mother, father, trait
Alice,,,
Bob, Alice, Charles, True
Charles,,,

Contributing

If you’d like to contribute to this project, please fork the repository and use a feature branch. Pull requests are warmly welcomed.

Licensing

Remember to replace "heredity.py" and "data.csv" with the actual filenames if they are different. The `README.md` file should be placed in the root directory of your repository. When you push this to GitHub, the platform will automatically display the contents of the `README.md` file as the homepage of the repository.
