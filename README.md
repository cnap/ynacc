# The Yahoo News Annotated Comments Corpus (YNACC)


The dataset contains comment threads posted in response to online news articles. In total, YNACC contains 522k comments from 140k threads posted in response to Yahoo News articles. 9.2k comments and 2.4k threads in this dataset have been coded at the comment-level and the thread-level. The annotations include 6 dimensions of individual comments and 3 dimensions of threads on the whole, listed below. The coding was done by two groups of annotators: professional, trained editors and untrained crowdsourced workers. In addition to the coded Yahoo News articles, YNACC also contains annotations for 1k threads from the Internet Argument Corpus (Walker et al., 2012; Abbot et al., 2017).

For more information about this work, please see our paper,

[**Finding Good Conversations Online: The Yahoo News Annotated Corpus**](law-2017-ynacc.pdf)  
Courtney Napoles, Joel Tetreault, Enrica Rosato, Brian Provenzale, and Aasish Pappu  
11th Linguistic Annotation Workshop (LAW-XI), 2017

This paper should be cited in any research using this corpus.

```
@InProceedings{napoles2017ynacc,
    author    = {Courtney Napoles and Joel Tetreault and Enrica Rosata and Brian Provenzale and Aasish Pappu},
    title     = {Finding Good Conversations Online: The Yahoo News Annotated Comments Corpus},
    booktitle = {Proceedings of The 11th Linguistic Annotation Workshop},
    month     = {April},
    year      = {2017},
    address   = {Valencia, Spain},
    publisher = {Association for Computational Linguistics},
	pages     = {13--23},
}

```

## Obtaining the corpus

To download the data, please visit the following URL:
http://webscope.sandbox.yahoo.com/catalog.php?datatype=l&did=83

## Annotation scheme

Threads have the followng annotations:

*  constructiveclass - Constructive, Not constructive
*  sd_agreement  - Agreement throughout, Continual disagreement, Agreement to disagreement, Disagreement to agreement
*  sd_type - Argumentative (back and forth), Flamewar (insulting), NA, Not persuasive, Off-topic/digression, Personal stories, Positive/respectful, Snarky/humorous

The comment-level annotations are

* sentiment - Mixed, Neutral, Negative, Positive
* tone - Controversial, Sarcastic, Informative
* commentagreement - Agree, Disagree, Adjunction Opinion
* topic - Offtopic with article, offtopic with conversation
* intendedaudience - Broadcast, Reply
* persuasiveness - Persuasive, Not persuasive

This repository includes the [annotation instructions](rater-guidelines.pdf) and the [html template](hit-template.html) used for Mechanical Turk.

Additionally, all of the comments contain the following metadata:

*  sdid - subdialogue ID
*  commentindex - position of the comment as it appears in the subdialogue
*  headline - headline of the article
*  url - URL of the original article
*  guid  - encrypted user id
*  commentid - comment id
*  timestamp - timestamp of the comment
*  thumbs-up - comment level thumbsup
*  thumbs-down - comment level thumbsdown
*  text  - text of the comment
*  parentid - ID associated with the first comment of the subdialogue

## References
Rob Abbott, Brian Ecker, Pranav Anand, and Marilyn Walker. _Internet Argument Corpus 2.0: An SQL schema for dialogic social media and the corpora to go with it_. LREC 2016.

Marilyn Walker, Jean Fox Tree, Pranav Anand, Rob Abbott, and Joseph King. _A corpus for research on deliberation and debate_. LREC 2012.

---

Contact: Courney Napoles <napoles@cs.jhu.edu>  
Updated: 3 April 2017
