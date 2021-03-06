# Introduction

This [project](https://anujk14.github.io/XML-To-Blockly/) is funded by the 2016 edition of the [Google Summer of Code program](https://summerofcode.withgoogle.com/).
[Anuj Khandelwal](https://github.com/anujk14/) has been selected to work on a [Graphical workflow editor for eHive using Blockly](https://summerofcode.withgoogle.com/projects/#5041231054766080) in the [Ensembl Genomes Browser](https://summerofcode.withgoogle.com/organizations/6373155673210880/) organization under [Matthieu Muffato](www.ebi.ac.uk/~muffato/)'s mentorship.

[eHive](https://github.com/Ensembl/ensembl-hive) is a system used to run computation pipelines in distributed environments. eHive workflows are currently being migrated to a Relax NG specification. Currently the eHive workflows are manually coded and this requires expertise in computer science. It also takes up a lot of time. Due to such shortcomings handling workflows becomes very cumbersome.

This project aims to remove these drawbacks of the existing system by creating a graphical editor for eHive workflows using Google's [Blockly](https://developers.google.com/blockly/) library which would enable us to visualize the XML code in terms of Blockly blocks and provide output for them in XML format using Blockly's existing "Export to XML" option. The backbone of this graphical editor would be some rules written to handle the Relax NG XML schema specification and to create Blockly blocks automatically in accordance with the same.

For example, the XML to Blockly converter would apply pre-defined rules to the Relax NG specification entered by the user, and generate code to represent the specification using Blockly blocks.

The proposed editor would have capabilities of handling not just workflows for eHive, but any specifications written using the Relax NG schema.

# How to use

1. Open https://ens-lg4.github.io/XML-To-Blockly/ in your web browser.
5. Click on the 'Choose file' and open a Relax NG file. This will create a list of blocks in the toolbox.
6. Play with the blocks to create a diagram that follows the specification.

# Current state

We are still working on the conversion of Relax NG rules to Blockly blocks and constraints.
Once this is done, we'll add the ability to import / export XML files (that follow the specification).

Navigate to https://ens-lg4.github.io/XML-To-Blockly/ to use the graphical XML editor.
