# Software Catalogue

This path contains a catalogue of all the software components developed or to be developed for the DComEX project.

This includes the simulation software, and software used for pre processing, ML, etc.

Pre processing and post-processing are important, because they form a workflow with the simulation applications. As such they will want to run efficiently on the same system (maybe on a CPU-only partition) as part of an automated pipeline.

If your software is something like "a Tensorflow model", treat Tensorflow as a "library" and your model as software, so that we can capture it here.

To add a new software component make a copy of the `template.md` and fill it in. See the main `readme.md` for more detailed instructions.
