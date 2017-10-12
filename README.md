*****THIS README IS STILL BEING CREATED. EXPECT GENERAL CHAOS*****

# BYU-Analogical-Reasoning-Dataset
A set of python dictionaries containing word-based analogy tasks, originally used in CoRL 2017

The BYU Analogical Reasoning Dataset is a series of benchmark analogy test sets of the form A:B :: B:C.
The analogy words are augmented with Penn Treebank part-of-speech tags. They include both one-to-many and many-to-one relationships.

Included analogy sets:

accessing_containers - 420
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
