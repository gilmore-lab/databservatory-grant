Planning
================
Rick O. Gilmore
2017-11-21 14:20:01

Background
----------

This is a planning document for the Video Databservatory project.

Partners
--------

-   Vasant Honavar
-   Jim Rehg
-   Tal Yarkoni?

Related NIH or NSF grants
-------------------------

-   Tal Yarkoni's [`pliers`](https://github.com/tyarkoni/pliers) project is part of [NeuroScout](https://projectreporter.nih.gov/project_info_description.cfm?aid=9357698&icde=37015464) funded under 5R01MH109682-02.
    -   Rick spoke with Tal on 2017-11-13.
    -   The project is affiliated with OpenNeuro.
-   [NIH Big Data to Knowledge (BD2K)](https://commonfund.nih.gov/bd2k)

Use cases
---------

-   Platform for analyzing LENA recordings (Elika Bergelson from HomeBank) or CHAT format transcripts from PLAY videos
    -   Talk with Mike about integration with [`childes-db`](http://childes-db.stanford.edu/index.html)?
    -   Is *this* the chance to mirror the TalkBank/CHILDES videos on Databrary?
-   Video analysis of looking direction
    -   Integration with [Kim Scott's](http://www.mit.edu/~kimscott/index.html) platform [LookIt](https://lookit.mit.edu/).
    -   [Notes](https://docs.google.com/document/d/1Qkndhz6BPAcuKlL5RgmdaIvBvNzyG8oWWvSTMptku9w/edit) from a discussion with Databrary staff on 2017-10-26.
    -   [Kim Scott's notes](https://docs.google.com/document/d/11S7D1FfVO0MsTO1kh9OtcN2rKSEM2BOuCtZcRTyMmMU/edit#heading=h.9htopc2auau2) on existing tools for coding look direction from video.
-   Semi-automated video/image coding
    -   Raw files -&gt; machine applied codes -&gt; human analysts
    -   Raw files -&gt; human analysts -&gt; human applied codes -&gt; machine learning models
-   Visualize time series from PLAY project
    -   Tags become search terms/search indices for Databrary
-   Store videos on Databrary/Databservatory, link with annotations provided by MTurk workers.
-   Web-based video annotation (lower temporal/spatial resolution than Datavyu)
-   Research questions
    -   Can (Datavyu) tagged video segments be used to train a ML model. What would the target "behavior" be?
-   Develop or adapt existing video annotation standard
    -   `<date_timestamp_hhmmss.nnn>, <duration_ms>, <bounding_region_pix>, <code_type>, <code>`
    -   e.g, 20171121\_140425.033, .033, \[0,0,640,480\], face\_detected, TRUE
    -   Does Yarkoni's `pliers` propose format for annotation?

Commercial providers in the image/video annotation space
--------------------------------------------------------

-   [Playment](https://playment.io/), per [this](https://venturebeat.com/2017/11/21/playment-raises-1-6-million-to-improve-ai-training-through-crowdsourced-data-tagging/) story.
-   [CrowdFlower](https://www.crowdflower.com/), per [this](https://venturebeat.com/2017/07/19/crowdflower-expands-to-help-companies-implement-machine-learning/) story.
-   [Mighty AI](https://mty.ai/), per [this](https://venturebeat.com/2017/01/10/spare5-rebrands-as-mighty-ai-and-lands-14-million-from-intel-gv-accenture-others/) story.

Projects to benchmark against or integrate with
-----------------------------------------------

-   [childes-db](http://childes-db.stanford.edu/index.html)
-   [WordBank](http://wordbank.stanford.edu)
-   [OpenNeuro](http://openneuro.org)
-   [Neurosynth](http://neurosynth.org)
-   [Brain Imaging Data Structure (BIDS)](http://bids.neuroimaging.io/) as a possible "standard" data package for studies

Others to talk with
-------------------

-   [Kristin Branson](https://www.janelia.org/people/kristin-branson), head of [Branson Lab](https://www.janelia.org/lab/branson-lab) at Janelia Farm.
    -   Sample papers
        -   Egnor, S. E. R., & Branson, K. (2016). Computational analysis of behavior. *Annual Review of Neuroscience*, 39, 217–236. Retrieved from <http://dx.doi.org/10.1146/annurev-neuro-070815-013845>
        -   Kabra, M., Robie, A. A., Rivera-Alba, M., Branson, S., & Branson, K. (2013). JAABA: Interactive machine learning for automatic annotation of animal behavior. *Nature Methods*, *10*(1), 64–67. Retrieved from <http://dx.doi.org/10.1038/nmeth.2281>
-   Dima Amso
-   Chen Yu
-   Gedeon Deak
-   Greg Farber, NIMH
    -   Rick emailed 2017-11-20.
-   Deb Roy
-   Chris Gorgolewski or Russ Poldrack from [OpenNeuro](http://openneuro.org)
    -   Similarities between OpenNeuro's cloud analysis platform and what we want to build; possible synergies
