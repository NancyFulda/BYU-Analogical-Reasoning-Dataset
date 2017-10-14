<h1>BYU Analogical Reasoning Dataset (BARD)</h1>

A set of analogy tasks of the form A:B::C:D, intended as a benchmark for analogical reasoning and planning. Analogies are augmented with Penn Treebank part-of-speech tags and include both one-to-many and many-to-one relationships. The dataset contains 23,692 analogies in all.

<h2>Format</h2>
The BYU Analogical Reasoning Dataset is provided is four separate formats contained in subdirectories. Each subdirectory contains the same 23,692 analogical queries with the following distinctions.<br><br>
<strong>python</strong> - A set of python dictionaries containing each analogy subcorpus<br>
<strong>python-reversed</strong> - Python dictionaries with word positions swapped (i.e. milk:refrigerator::broom:closet ==> refrigerator:milk:: closet:broom)<br>
<strong>text</strong> - A set of plain text files containing one analogical query per line.<br>
<strong>text-reversed</strong> - Plain text files with word positions swapped (i.e. milk:refrigerator::broom:closet ==> refrigerator:milk:: closet:broom)<br>


<h2>Analogy Subcorpora</h2> 
accessing_containers (420)<br>
affordance (2448)<br>
belong (992)<br>
causation (210)<br>
containers (420)<br>
locations for objects (2070)<br>
rooms for containers (1406)<br>
rooms for objects (1406)<br>
tools (930)<br>
trash or treasure (552)<br>
travel (992)<br><br>

11,846 analogies total


<!--CLEANING HOUSE - IGNORE THIS TEXT FOR NOW
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
we believe analogy shapes have something to do with the ease/difficulty of the analogies as well as with the types of algorithms that may be needed to solve them. [list the shapes associated with the corpora] -->
