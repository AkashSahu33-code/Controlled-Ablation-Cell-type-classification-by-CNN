This project is all about classification of Controlled and Ablation cell types .

Let us know a bit about about that

Controlled vs. Ablation Cell Types

In biomedical and biophysical research, especially in experimental cell studies, distinguishing between controlled and ablation cell types is crucial for understanding cellular function and system-level responses.

Controlled Cell Types: These are unaltered or untreated cells used as a baseline reference. They represent normal physiological conditions and help establish expected behavior in the absence of intervention.

Ablation Cell Types: These are cells that have been intentionally removed, silenced, or destroyed (via genetic, chemical, or laser-based methods) to study the impact of their absence. 
                      This allows researchers to identify the specific roles of individual cell types in a biological system.

Why It Matters:
Classifying cells into controlled and ablation types enables:

* Functional analysis of specific cells or genes
* Insight into disease mechanisms (e.g., neurodegeneration, immune response)
* Validation of therapeutic targets
* Improved understanding of cellular interactions and system robustness
This distinction is especially valuable in biophysics and biomedical fields, where quantifying and modeling biological processes depends on precisely controlled experimental conditions.


Lets know bit about our CNN implementation-

I had very less and Imbalanced image set as biological data is very tough to mine hence we needed to work on limited resources.
I tackled both problems by using Class weight technique for Balancing class imbalanced data & Image Augmentation for less amount of Image data.

I choosed the images Randamoly using python for Test & Training Set . We had 144 images belongs to Controlled Cell and 90 images of Ablation type of cells which we splited in 80:20 Ratio for Training set and Test set respectively.
The image set was very Heterogenous and Non-Linear and completely difficult to classify by Naked eye.


* Used CNN for classification & ran it till 33 epochs.
* Image Augmentation includes following Techniques & pParameters
  rescale = 1./255,
  shear_range = 0.2,
  zoom_range = 0.2,
  horizontal_flip = True
* Used relu and sigmoid as activation function.
* filters=32
* kernel_size=3
* Neuron unit = 128
  
  
