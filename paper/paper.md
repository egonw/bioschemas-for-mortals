---
title: 'BioHackEU24 report: Bioschemas for Mortals'
title_short: 'BioHackEU24 #10: Bioschemas for Mortals'
tags:
  - markup
  - schemas
authors:
  - name: Phil Reed
    orcid: 0000-0002-4479-715X
    affiliation: 1
  - name: Helena Schnitzer
    orcid: 0000-0002-6382-9452
    affiliation: 2
  - name: Nick Juty
    orcid: 0000-0002-2036-8350
    affiliation: 1
affiliations:
  - name: The University of Manchester, UK
    index: 1
  - name: Forschungszentrum Jülich, DE
    index: 2
date: 8 November 2023
cito-bibliography: paper.bib
event: BH24EU
biohackathon_name: "BioHackathon Europe 2024"
biohackathon_url:   "https://biohackathon-europe.org/"
biohackathon_location: "Barcelona, Spain, 2024"
group: Project 10
# URL to project git repo --- should contain the actual paper.md:
git_url: https://github.com/PhilReedData/bioschemas-for-mortals
# This is the short authors description that is used at the
# bottom of the generated paper (typically the first two authors):
authors_short: Nick Juty, Helena Schnitzer, Phil Reed
---


# Introduction

Bioschemas is a community effort `[Gray2023]` to improve the FAIRness of web-based resources. Established by ELIXIR over seven years ago, it has good adoption by the technical communities in workflows, software, and tools but less adoption than it should be. Particularly in less technical communities such as training or even data services.

The Bioschemas website hosts tooling, training and guidance materials. Practical 'how to use Bioschemas' help and examples have been neglected. Guidance is technical - written by techies for techies - inappropriate or inaccessible for a large cohort of potential Bioschemas users. Examples focus on simple use cases and not real set-ups that users actually encounter in their work. This makes access to directly usable markup impossible, leaving users confused about where to go next. This lack of helpful support poses an unacceptably high technical barrier for the broader user community and means we are not fully exploiting Bioschemas. Common complaints frequently cite a technical ‘barrier’, the lack of ‘lightweight’ guidance, the need to ‘demystify’ and the lack of assistance to users who have the desire to implement Bioschemas, but not the ‘how’.

The goal of this project is to reimagine, reframe and supplement the existing Bioschemas guidance available. Working with non-technical users from the data and training platforms, Patterns of use, tasks(different CMS; properties) and user personas. This will be used to provide users with specific code examples that can be copy/pasted, documented examples for different web setups, customised guidance for different personas and be validated by non-technical users in the data and training platforms.

# Task 1: Analytics

Google Analytics information was captured from July - Nov 2024 (ongoing). Data was captured and analysed over this period in an effort to ascertain user behaviour, including sessions, location of originating request, transitions, pages accessed, view time (engagement), landing page (page session started), and source (direct, organic search and referral). 

## Main outcomes

Roughly 33% of visits from users arriving from ‘direct’ routes (bookmark or web link) resulted in ‘engaged’ sessions, while almost 50% engagement was seen when using ‘referral’ links.

Large numbers of visits were to ‘Training’ related pages, which we believe are a result of current work in those areas, for example, Training Platform improving its process with respect to being scrapeable by TeSS.

Excluding such links which were explainable as ‘noise’, we note that some ‘help’ URLs were highly accessed, including ‘/tutorials/howto/...’ on ‘bioschemas’, ‘add markup’, ‘add github’. We conclude that help pages are among those most visited, after excluding explainable phenomena. 


## Next Steps

We will continue to collect analytics information going forward, to identify whether changes made in the webpages/organisation of materials and their availability are visible through the analytics. This is supported by engagement times on those pages. (Appendix A.1).

There appears to be a clear need, supported by other tasks in this work, especially user stories, suggesting that more general guidance is needed. 

Further analysis of the analytics could be undertaken to understand the needs or guidance viewed on a national level, for instance, whether there are regional differences in the needs in Germany vs those in the UK.

Where is tutorials/community - it's not in the menu? Same for many other ‘tutorials’ viewed

While we attempt to evaluate the conversions (where there is a concrete action that is the result of having viewed some page), at best we can only approximate what this would manifest as, in the context of guidance/tutorials. There may, with sufficient information, be a way to see, for example, whether some guidance specifying the use of GitHub corresponded to some GitHub commits. We could also look further to delineate between new users and returning users. 

# Task 2: User Stories
...

![Pie chart showing types of persona surveyed](task-2.png)

...

# Task 3: Drop in session to facilitate Task 2
...
![Screenshot from the drop in session, 17:00 CET, 6th Nov 2024](task-3.png)
...

# Formatting

This document use Markdown and you can look at [this tutorial](https://www.markdowntutorial.com/).

## Subsection level 2

Please keep sections to a maximum of only two levels.

## Tables and figures

Tables can be added in the following way, though alternatives are possible:

Table: Note that table caption is automatically numbered and should be
given before the table itself.

| Header 1 | Header 2 |
| -------- | -------- |
| item 1 | item 2 |
| item 3 | item 4 |

A figure is added with:

![Caption for BioHackrXiv logo figure](./biohackrxiv.png)

# Other main section on your manuscript level 1

Lists can be added with:

1. Item 1
2. Item 2

# Citation Typing Ontology annotation

You can use [CiTO](http://purl.org/spar/cito/2018-02-12) annotations, as explained in [this BioHackathon Europe 2021 write up](https://raw.githubusercontent.com/biohackrxiv/bhxiv-metadata/main/doc/elixir_biohackathon2021/paper.md) and [this CiTO Pilot](https://www.biomedcentral.com/collections/cito).
Using this template, you can cite an article and indicate _why_ you cite that article, for instance DisGeNET-RDF [@citesAsAuthority:Queralt2016].

The syntax in Markdown is as follows: a single intention annotation looks like
`[@usesMethodIn:Arend2023]`; two or more intentions are separated
with colons, like `[@extends:discusses:Castro2023]`. When you cite two
different articles, you use this syntax: `[@citesAsDataSource:Rosinach2023; @citesAsDataSource:Soiland-Reyes2024]`.

Possible CiTO typing annotation include:

* citesAsDataSource: when you point the reader to a source of data which may explain a claim
* usesDataFrom: when you reuse somehow (and elaborate on) the data in the cited entity
* usesMethodIn
* citesAsAuthority
* citesAsEvidence
* citesAsPotentialSolution
* citesAsRecommendedReading
* citesAsRelated
* citesAsSourceDocument
* citesForInformation
* confirms
* documents
* providesDataFor
* obtainsSupportFrom
* discusses
* extends
* agreesWith
* disagreesWith
* updates
* citation: generic citation


# Results


# Discussion

...

# Acknowledgements

- Led by: Nick Juty, Helena Schnitzer, Phil Reed
- Participants (on site): Emily Knight, Lucy Pelton, Deborah van Wyk
- Online: Leyla Jael Castro, Munazah Andrabi, Ulrike Wittig, Finn Bacall, Ginger Tseung
- Interactions with other groups: #24, #21 
- Project Repository: https://github.com/elixir-europe/biohackathon-projects-2024/blob/main/10.md



# Appendices

## Appendix A1
![Views and engagement rates of pages, measured with Google Analytics.](appendix-a1.png)

## Appendix A2.1
![The user stories for Bioschemas, organised by persona.](appendix-a2.1.png)

## Appendix A2.2
![Visual clustering of user story concepts, within each persona, and related tasks.](appendix-a2.2.png)

## Appendix A7
![Example image showing difference between Types and Profiles.](appendix-a7.png)

## Appendix A8.1
![Layout suggestion for the infographic, showing the cloud of websites using Schema.org.](appendix-a8.1.png)


## Appendix A8.2
![Initial illustration of the infographic ‘Why use Bioschemas?’.](appendix-a8.2.png)

## Appendix B
![Gallery of icebreaker drawings of each other with our eyes closed (leads).](appendix-b1.png)
![Gallery of icebreaker drawings of each other with our eyes closed (participants).](appendix-b2.png)


# References
