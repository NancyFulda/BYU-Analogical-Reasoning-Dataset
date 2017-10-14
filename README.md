<h1>BYU Analogical Reasoning Dataset (BARD)</h1>

A set of analogy tasks of the form A:B::C:D, intended as a benchmark for analogical reasoning and planning. Analogies are augmented with Penn Treebank part-of-speech tags and include both one-to-many and many-to-one relationships. The dataset contains 23,692 analogies in all.

<h2>Format</h2>
The BYU Analogical Reasoning Dataset is provided is four separate formats contained in subdirectories. Each subdirectory contains the same 23,692 analogical queries with the following distinctions.<br><br>
**python** - A set of python dictionaries containing each analogy subcorpus
**python-reversed** - Python dictionaries with word positions swapped (i.e. milk:refrigerator::broom:closet ==> refrigerator:milk:: closet:broom)<br>
**text** - A set of plain text files containing one analogical query per line.<br>
**text-reversed** - Plain text files with word positions swapped (i.e. milk:refrigerator::broom:closet ==> refrigerator:milk:: closet:broom)<br>


<h3>Analogy Subcorpora</h3> 
*accessing_containers (420)*
affordance - 2448
belong - 992
causation - 210
containers - 420
locations for objects - 2070
rooms for containers - 1406
rooms for objects - 1406
tools - 930
trash or treasure - 552
travel - 992

11,846 analogies total


90 analogies - measures ability to determine how best to access the contents of a container
jar_NN:open_NN :: box_NN:open_NN
bottle_NN:pour_VB :: faucet_NN:turn_NN

USAGE - python 2.7
import pickle
f=open('accessing-containers.p')
analogies = pickle.load(f)

USAGE - python 3.x
import pickle
f=open('accessing-containers.p')
analogies = pickle.load(f,encoding='latin1')


Lots of many-to-one relationships - it is not possible to get a perfect score if you're only counting the top response word.

ANALOGY SHAPES
we believe analogy shapes have something to do with the ease/difficulty of the analogies as well as with the types of algorithms that may be needed to solve them. [list the shapes associated with the corpora] 
