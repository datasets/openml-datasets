The resources for this dataset can be found at https://www.openml.org/d/300

Author: Ron Cole and Mark Fanty (cole@cse.ogi.edu, fanty@cse.ogi.edu)  
Donor: Tom Dietterich (tgd@cs.orst.edu)  
Source: [UCI](https://archive.ics.uci.edu/ml/datasets/ISOLET)   
Please cite: UCI  

### Description

ISOLET (Isolated Letter Speech Recognition) dataset was generated as follows: 150 subjects spoke the name of each letter of the alphabet twice. Hence, there are 52 training examples from each speaker. The speakers are grouped into sets of 30 speakers each, 4 groups can serve as training set, the last group as the test set. A total of 3 examples are missing, the authors dropped them due to difficulties in recording. 

This is a good domain for a noisy, perceptual task. It is also a very good domain for testing the scaling abilities of algorithms. For example, C4.5 on this domain is slower than backpropagation!

### Source

* Creators: 
Ron Cole and Mark Fanty 
Department of Computer Science and Engineering, 
Oregon Graduate Institute, Beaverton, OR 97006. 
cole '@' cse.ogi.edu, fanty '@' cse.ogi.edu 

* Donor: 
Tom Dietterich 
Department of Computer Science 
Oregon State University, Corvallis, OR 97331 
tgd '@' cs.orst.edu

### Attributes Information
  
All attributes are continuous, real-valued attributes scaled into the range -1.0 to 1.0. The features are described in the paper by Cole and Fanty cited below. 
The features include spectral coefficients; contour features, sonorant features, pre-sonorant features, and post-sonorant features. The exact order of appearance of the features is not known.

### Relevant papers

Fanty, M., Cole, R. (1991).  Spoken letter recognition.  
In Lippman, R. P., Moody, J., and Touretzky, D. S. (Eds). Advances in Neural Information Processing Systems 3.  San Mateo, CA: Morgan Kaufmann.

Dietterich, T. G., Bakiri, G. (1991)  Error-correcting output codes: A general method for improving multiclass inductive learning programs.  
Proceedings of the Ninth National Conference on Artificial Intelligence (AAAI-91), Anaheim, CA: AAAI Press.

Dietterich, T. G., Bakiri, G. (1994) Solving Multiclass Learning Problems via Error-Correcting Output Codes.

