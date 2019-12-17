# E2E-NLG-Challenge
 A seq2seq model transfering MR into NL
 
This is a sequece2sequence model transfering meaning representations(MR) of a restaurant into a description in natural language(NL). Pytorch is used to build up the seq2seq neural model.

### Overview

The aim of the project is to:

1. train a model on the E2E restaurant data set on a GPU
2. implement beam search for evaluation
3. implement a BLEU evaluator and report BLEU scores

In this dataset, the inputs are restaurant meaning representations, which are a series of key-value pairs that encode information about a restaurant. The outputs are fluent sentences that describe the restaurant. Here is an example:

*Input: Meaning Representation*

```
name[The Eagle],
eatType[coffee shop],
food[French],
priceRange[moderate],
customerRating[3/5],
area[riverside],
kidsFriendly[yes],
near[Burger King]
```

*Output: Fluent Sentence*

```
The three star coffee shop, The Eagle, gives families a mid-priced dining experience featuring a variety of wines and cheeses. Find The Eagle near Burger King.
```
