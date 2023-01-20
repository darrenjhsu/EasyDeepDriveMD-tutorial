
## Exploring cyclosporin A conformations in a sub-optimal way

... which is why this is a tutorial and not scientific work.


### First, get the EasyDeepDriveMD and dependency

Get the repository:

```bash
git clone git@github.com:darrenjhsu/EasyDeepDriveMD.git
```

Now you should have the folder structure like this:

```
Experiment/
  |- Force_fields/
  |    |- all your force field files
  |- Structures/
  |    |- protein.psf
  |    |- protein.pdb
  |- Templates/
  |    |- protein_init.pdb
  |    |- sampling.conf
  |- EasyDeepDriveMD/ 
```

Follow the Requirement section in the README for EasyDeepDriveMD, and make sure that MDAnalysis works.
We will be using the `main` branch and for this particular system.


### Try out the script

It is really simple, just

```bash
cd EasyDeepDriveMD
bsub Ssubmit.sh
```

This will submit a tiny sampling job, using 1 node (6 GPUs) for 2 hours, running as many rounds as possible.
While it is executing, please read the README in `EasyDeepDriveMD/`.
It gives more information about how you can change different parts of this pipeline.


