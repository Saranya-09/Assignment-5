# Assignment-5
# QUESTION-1
# Protein Interaction Network Analysis
# Author: Saranya Guvvala
# Date: [04-27-2024]
# Programming Language & Version: Python 3.8
# Dependencies: pandas, networkx, matplotlib, numpy

# Input
Human-PPI.txt: A file with protein interaction data. It has two columns for each interacting protein pair, separated by spaces.

# Script Description
This script analyzes how proteins interact with each other. It calculates and reports:

# Degrees: How many connections each protein has.
# Clustering Coefficients: How closely proteins tend to group together.
# Average Clustering Coefficient: The average of the clustering coefficients for all proteins.
# Degree Distribution: A graph showing how common each degree of connection is among all proteins.
It also checks if the network follows a power law, a common pattern in protein interaction networks.

# Output
Degree Distribution Plot: A graph that shows the distribution of connections each protein has, displayed on a log-log scale. This graph helps to visualize the network's structure.

# QUESTION-2
# Protein Path Length Analysis
# Author: Saranya Guvvala 
# Date: [04-27-2024] 
# Programming Language & Version: Python 3.8 Dependencies: pandas, networkx, scipy
# Input Files: 
Human-PPI.txt: Contains protein-protein interaction data, with each line representing an interaction between two proteins separated by whitespace.
protein-list1.txt and protein-list2.txt: Each file contains a list of proteins. Each protein should be listed on a new line.
# Script Description
This script analyzes the interactions between proteins in a network. It takes three input files:

Human-PPI.txt: This file contains information about pairs of proteins that interact with each other.
protein-list1.txt: This file contains a list of proteins.
protein-list2.txt: This file contains another list of proteins.

The script performs the following steps:

Loading Data: Reads the protein interaction data from the Human-PPI.txt file and the protein lists from protein-list1.txt and protein-list2.txt.
Building the Network: Constructs a network (like a map) of how the proteins are connected to each other based on their interactions.
Calculating Path Lengths: For the proteins listed in protein-list1.txt and protein-list2.txt, it calculates the shortest "path" (the minimum number of steps) required to connect each pair of proteins in the network.
Statistical Comparison: Performs the Mann-Whitney U test to compare the distributions of these shortest path lengths between the two protein lists.

# Output
Prints the Mann-Whitney U test statistic and p-value to the console, indicating whether there is a significant difference in the connectivity patterns (or path lengths) between the two sets of proteins.

