#### command

##### Usage

Mandatory when applicable

**Usage conditions**

Must be filled in for components with componentDistributionForm="dockerImage".

##### Type

free text

##### Definition/Explanations

A command line used to invoke a component

**Recommended usage**

* For components registered as Docker images, fill in with the command used to invoke the component; please note that it must \(a\) only contain your executor i.e. the part required to run your command by excluding the parameters and their respective values, and \(b\) be available to run from everywhere in the docker image \(i.e. add your executor in the /usr/bin/ or use absolute paths\).



