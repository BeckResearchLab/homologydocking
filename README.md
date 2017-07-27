# Docking of small molecules to quorum sensing up and down regulated proteins

### note the down regulated are presented as negative controls

Must use this taxon oid from JGI: 2563366535

See this manuscript for more information:
* http://jb.asm.org/content/199/5/e00773-16.full

Sharable Link to Homology Structure Statistics:
https://docs.google.com/a/baldwinschool.org/spreadsheets/d/1VRb7BypAisn903an2tUbuq6KGpAWk2VmczbScoT_XiE/edit?usp=sharing

Running LeDock from Command Line (the old way):
/Applications/LeDock.app/Contents/MacOS/LeDock
Now, we put `ledock_mac` in our path and run that.

Tools:
* `generate_jobs` makes a job file to use as input to GNU parallel

To run the dockings, requires GNU parallel:
* `parallel -a ledock.jobs --max-procs 4`
