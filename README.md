This is a preliminary work on finishing the ongoing project of modularising ZMK. This repository is intended to include the set of boards, shields, modules, and any other extensions to ZMK. None of these elements are actually stored within this repository. This repository strictly contains links to repositories and metadata.

This repository would ideally also contain tools to help manage the collection, and to make the collection more useful in general. In particular, there is the hope that this repository will (with enough automated tools) contain every single keyboard that could be supported by ZMK - This includes a number of (wired-only) keyboards which are not yet supported, but excludes keyboards which run on 8-bit MCUs as Zephyr does not support those.

This repository should be distinct from the core ZMK repository to separate the pull requests of the collection from the pull requests of ZMK itself. 

The repository links point to a particular commit. If an element is being updated, such as to add support for a display, then once the update has finished the owner of the element is expected to submit a pull request updating the commit to a newer one. Most metadata about boards is expected to change only extremely rarely. Metadata collected is to allow the creation of tools such as a fork of jhelvy's split keyboard comparison tool.

The main issue facing this repository is the potential presence of malicious actors. Such actors could attempt to include malicious code, text, or images within a module. This is the main thing that reviewers will be checking for, aside from making sure that the checklist is satisfied. An automated tool to handle many cases should be developed at some point, but some cases -- in particular images -- are unlikely to be automated anytime soon.