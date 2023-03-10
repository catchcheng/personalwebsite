---
title: "Neural Machine Translation Using an Attention Model"
date: 2020-11-09 09:27:12
categories: DeepLearning Keras
badges:
  - type: success
    tag: NLP
  - type: danger
    tag: LSTM
image: assets/img/machinetranslation.png
---

Machine translation models can be used to map from one sequence to another. They are useful not just for translating human languages (like French->English) but also for tasks like date format translation. An attention mechanism allows a network to focus on the most relevant parts of the input when producing a specific part of the output.

<!--more-->

Here is the attention model in the following figure.

![../../assets/img/emomachinetranslationjifier.png](../../assets/img/machinetranslation.png)

After fitting the model, we can now see the results on the examples.
source: 3 May 1979
output: 1999-05-03
source: 5 April 09
output: 2009-04-04
source: 21th of August 2016
output: 2016-06-20
source: Tue 10 Jul 2007
output: 2007-07-10
source: Saturday May 9 2018
output: 2018-05-09
source: March 3 2001
output: 2011-03-03
source: March 3rd 2001
output: 2011-03-03
source: 1 March 2001
output: 2011-03-01
