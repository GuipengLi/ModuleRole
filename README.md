ModuleRole
==========

A Tool for Modulization, Role Determination and Visualization in Protein-Protein Interaction Networks



Abstract
--------

Rapidly increasing amounts of (physical and genetic) protein-protein interaction (PPI) data are produced by various high-throughput techniques, and interpretation of these data remains a major challenge. In order to gain insight into the organization and structure of the resultant large complex networks formed by interacting molecules, using simulated annealing, a method based on the node connectivity, we developed ModuleRole, a user-friendly web server tool which finds modules in PPI network and defines the roles for every node, and produces files for visualization in Cytoscape and Pajek. For given proteins, it analyzes the PPI network from BioGRID database, finds and visualizes the modules these proteins form, and then defines the role every node plays in this network, based on two topological parameters Participation Coefficient and Z-score. This is the first program which provides interactive and very friendly interface for biologists to find and visualize modules and roles of proteins in PPI network. As an interactive and highly customizable application, ModuleRole requires no expert knowledge in graph theory on the user side and can be used in both Linux and Windows system, thus a very useful tool for biologist to analyze and visualize PPI networks from databases such as BioGRID.


Availability
------------

ModuleRole is implemented in Java and C, and is available at [bioinfo.org](http://www.bioinfo.org/modulerole/index.php). Supplementary information (user guide, demo data) is also available at this website. See more details in this [paper](http://www.plosone.org/article/info%3Adoi%2F10.1371%2Fjournal.pone.0094608)

Usage
-----
Download ModuleRoleV1.3.1_64bit.jar and the data in test/. Open the cmd or terminal, then run:

    $ java -jar ModuleRoleV1.3.1_64bit.jar test/BIOGRID-ORGANISM-Mus_musculus-3.2.103.tab.txt test/test-genelist.txt test/output > log.txt

**test-genelist.txt** is a list of genes pre-defined by user.
**BIOGRID-ORGANISM-Mus_musculus-3.2.103.tab.txt** is PPI data download from [BioGRID](http://thebiogrid.org/downloads/archives/Release%20Archive/BIOGRID-3.2.103/BIOGRID-ORGANISM-3.2.103.tab.zip).

The result will be saved in the directory output/. The \*.net and \*.xgmml files can be load into **Pajek** and **CytoScape** respectively. See the example in test/output/phyNet/simulatedAnnealing.


Citation
--------

Li, G., Li, M., Zhang, Y., Wang, D., Li, R., Guimera, R., . . . Zhang, M. Q. (2014). ModuleRole: A Tool for Modulization, Role Determination and Visualization in Protein-Protein Interaction Networks. PLoS One, 9(5), e94608. doi: 10.1371/journal.pone.0094608  [paper](http://www.plosone.org/article/info%3Adoi%2F10.1371%2Fjournal.pone.0094608)


Contact
-------

Email:  guipeng.lee@gmail.com
