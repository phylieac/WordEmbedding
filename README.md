# WordEmbedding

This is a Xcode Project, which you can complie in your MacOS. Or use the makefile in Windows/Linux/MacOS.

From Wiki:
Word embedding is the collective name for a set of language modeling and feature learning techniques in natural language processing (NLP) where words or phrases from the vocabulary are mapped to vectors of real numbers. Conceptually it involves a mathematical embedding from a space with one dimension per word to a continuous vector space with much lower dimension.

# Introduction

We proposes a method that captures the specified words (here we use the name entity) semantic relationship based on WORD VECTOR estimation toolkit v 0.1c. The specified words can embedd into the much lower dimension.

# Build and Run

* Xcode

  build and run the WordEmbedding
  
  ./wordembedding -train data.txt -entity entity.txt -output vectors.txt -cbow 0 -size 200 -window 8 -negative 25 -hs 0 -sample 1e-4 -threads 20 -binary 0 -iter 15
  
* Makefile
  
  cd ../WordEmbedding folder
  
  make
  
  ./wordembedding -train data.txt -entity entity.txt -output vectors.txt -cbow 0 -size 200 -window 8 -negative 25 -hs 0 -sample 1e-4 -threads 20 -binary 0 -iter 15
  
  Waring: -entity is the specified words file.
  Other parameters for training to look up Word2vec.
  
  
