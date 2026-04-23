# Editors comments

Your Correspondence, "Population-scale Ancestral Recombination Graphs with
tskit 1.0", has now been seen by 3 reviewers. As you will see from their
comments below, although the reviewers find your work of considerable potential
interest, they have raised a number of concerns. We continue to be interested
in potentially publishing your manuscript in Nature Methods, but would like to
evaluate your response to these concerns before we reach a final decision on
publication.

We therefore invite you to revise your manuscript to address these concerns. In
particular, we would expect that a revised version of the manuscript provides:

* Clarification of the significance of the tskit 1.0 release.

* Contextualisation of the work with that of others and your own prior work to
  clarify the advance made in the tskit software.

* Discussion comparing tskit to related work with respect to functionality,
  efficiency, or scalability.

* Discussion of future directions.

We are committed to providing a fair and constructive peer-review process. Do
not hesitate to contact us if there are specific requests from the reviewers
that you believe are technically impossible or unlikely to yield a meaningful
outcome.

When revising your paper:

* include a point-by-point response to the reviewers and to any editorial
  suggestions

* please underline/highlight any additions to the text or areas with other
  significant changes to facilitate review of the revised manuscript

* address the points listed described below to conform to our open science
  requirements

* ensure it complies with our general format requirements as set out in our
  guide to authors at www.nature.com/naturemethods

* resubmit all the necessary files by using the link below to access your home
  page



# Reviewers' Comments:

## Reviewer #1 (Remarks to the Author):

This brief correspondence describes the tskit library (version 1.0), which has
emerged as the leading software for analysis and manipulation of ancestral
recombination graphs (ARGs). tskit consists of several components, including
the core tree sequence data model, supporting libraries in C, and APIs in C,
Python, Rust, and R. A particular strength of the software is that it is
designed to be highly efficient and scalable, enabling analyses of as many as
several million ARGs. As described in this manuscript, tskit extends to
applications ranging from coalescent/ARG simulation to statistical and
population genetic inference, to visualization and ARG inference. It now serves
as enabling software for more than 60 software tools (Table S1), many of which
themselves are quite widely used.

This manuscript is quite short and essentially just announces and describes
version 1.0 of the software. As such, there is not much to review. But I think
publishing an announcement of this kind is appropriate, both to broadcast the
availability of a stable version 1.0 of the software and to provide a handle
for citations in the literature. The online documentation for the software is
excellent so there is no need to repeat technical details in a journal
publication.

My own laboratory makes regular use of tskit and we have found it to be very
well engineered and documented. Indeed, tskit has emerged as a kind of model
for scientific software evolutionary and population genomics community. As part
of this review, we downloaded the latest version and used it to carry out a
variety of simple calculations on simulated ARGs and we found that everything
worked as documented. We strongly support the publication of this announcement.

Signed: Adam Siepel


## Reviewer #2 (Remarks to the Author):

This correspondence serves both as a brief overview of the highly influential
tskit package alongside the announcement of tskit version 1.0. The tskit
package, which implements the tree sequence data model, has had a very
significant impact on population genetics over the past decade:
- Based on its highly efficient and biologically motivated storage of genetic
  variation data, it has facilitated for instance fast algorithms for computing
conventional population genetic summary statistics
- Led to very fast and flexible simulation of population genetic data using
  msprime and slim, which have become the gold-standard tools in the field
- Has been adopted broadly in widely used methods that infer ancestral
  recombination graphs
- And is utilised in many leading downstream population genetic inference
  methods that use ARGs and achieve unprecedented accuracy in resolving
evolutionary histories

I don’t have any major comments as the correspondence does not report any
specific new results and is relatively short. I think it covers the major
achievements of the tskit package, for which the tskit developer team deserves
substantial recognition. Perhaps one comment is that the correspondence could
more clearly state the significance of the 1.0 release (i.e., why this
milestone is reached now). Also, it would be a valuable opportunity to outline
any future directions, and some perspective on how the tskit community may
evolve.


## Reviewer #3 (Remarks to the Author):

This manuscript presents a software toolkit, tskit 1.0, for facilitating
software development involving ancestral recombination graphs (ARGs). As the
paper notes, ARGs have greatly grown in importance in evolutionary and
population genetics as data and compute resources have accumulated that allow
one to identify and work with non-trivial ARGs. The area is thus important and
the paper makes a strong case for the impact of this particular platform in
bringing ARGs to large-scale genomic data. As Table S1 demonstrates, tskit has
already been widely used in the field for developing a variety of applications
in population genetics, some quite well cited. I think the paper would have
value in highlighting this to a broader community of methods developers. This
is a library that supports application development development rather than a
specific application, so I cannot comment on experience with using it and
cannot easily test it myself in review. I have looked through the repository,
though, and it appears to be a substantial piece of work, well organized and
with supportive documentation and tutorials. The nature of the contribution
also makes significance harder to judge than for a more typical
application-focused paper, since the actual community of developers who would
benefit from reading the paper is a lot smaller than the community of users who
would not obviously benefit from reading it but benefit indirectly from those
developers reading it. Nonetheless, I am persuaded that the underlying work is
important. There is not much I would suggest changing although I have just a
few concerns and critiques:

1. The paper would benefit from describing more clearly what is new in the
present paper relative to the original 2016 paper on an earlier version of
tskit and a recent 2024 paper describing the methodology. Is there anything
fundamentally new beyond these other publications? What does publishing this
particular manuscript accomplish that the 2024 paper did not? I do not think
that needs to be explained in the manuscript itself but might be better
explained in a cover letter or response to reviewers.

2. While I understand this is a communication and an intentionally brief paper
that cites prior work from the authors about the methods, it would be helpful
to have at least a summary of what makes this package particularly effective
for large-scale ARGs. Are there new innovations in algorithms or data
structures, for example? Or is it just better software engineering?

3. Related to the prior point, it would be helpful to see more detail on
comparison to related work, even if just in the supplement, to back up the
claims of superiority of tskit to alternatives in the literature with respect
to functionality, efficiency, or scalability.

