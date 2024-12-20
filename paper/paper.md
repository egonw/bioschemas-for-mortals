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
authors_short: Phil Reed, Helena Schnitzer, Nick Juty
---


# Introduction

Bioschemas is a community effort `[@citesAsAuthority:Gray2023]` to improve the FAIRness `[@citesAsAuthority:Wilkinson2016]` of web-based resources. Established by ELIXIR over seven years ago, it is relatively well adopted by technical communities exemplified in workflows, software, and tools `[@citesForInformation:Castro2023;  @citesForInformation:Rosinach2023; @citesForInformation:Arend2024; @citesForInformation:Soiland-Reyes2024]` but less so for communities such as training or even data services.

The Bioschemas website hosts tooling, training and guidance materials. Largely, guidance is at a technical level — written by techies for techies — making it inappropriate or inaccessible for a large cohort of potential Bioschemas users. Practical ‘how to use Bioschemas’ help and examples have been neglected. Furthermore, examples focus on simple use cases and not real set-ups that users actually encounter in their work. This makes access to directly usable markup impossible, leaving users confused about where to go next. This lack of helpful support poses an unacceptably high technical barrier for the broader user community and means Bioschemas is not being fully exploited. Common complaints frequently cited include there being a technical ‘barrier’, lack of ‘lightweight’ guidance, the need to ‘demystify’ and the lack of assistance to users who have the desire to implement Bioschemas, but not the ‘how’ this can be accomplished.

The goal of this project is to reimagine, reframe and supplement the existing Bioschemas guidance available. Working with non-technical users from the data and training platforms, we identified patterns of use, commonly undertaken tasks (including use of different content management systems (CMS) and on user personas and roles. This information will be used to identify what is needed by less technical users, ultimately providing specific code examples that can be copy/pasted, documented examples for different web setups, customised guidance for different personas, and to address usability and content accessibility. The materials provided through this longer term goal will be validated by non-technical users, starting with relevant ELIXIR stakeholders.

# Task 1: Analytics

Google Analytics information was captured from July to November 2024 (and is ongoing). Data was captured and analysed over this period in an effort to ascertain user behaviour, including sessions, location of originating request, transitions, pages accessed, view time (engagement), landing page (page session started), and source (direct, organic search and referral). 

## Main outcomes

Roughly 33% of visits from users arriving from ‘direct’ routes (bookmark or web link) resulted in ‘engaged’ sessions, while almost 50% engagement was seen when using ‘referral’ links.

Large numbers of visits were to ‘Training’ related pages, which we believe are a result of current work in those areas, for example, the ELIXIR Training Platform is currently developing [guidance on how to mark up training materials](https://elixir-europe-training.github.io/ELIXIR-TrP-Bioschemas/) so they can be discovered by the [ELIXIR TeSS](https://tess.elixir-europe.org/about) (Training eSupport System) portal.

We note that some ‘help’ URLs were highly accessed, including ‘/tutorials/howto/…’ on ‘bioschemas’, ‘add markup’, and ‘add github’. We excluded such links which were explainable as ‘noise’ in the context of this work. We conclude that help pages are among those most visited, after excluding explainable phenomena. 


## Next steps

We will continue to collect analytics information going forward, to identify whether changes made in the webpages/organisation of materials and their availability impact the findability and usability of the guidance. This may manifest as  increased engagement times on those pages, for example. (Appendix A.1).

There appears to be a clear need, supported by other tasks in this work, especially user stories, suggesting that more general guidance is needed. 

Further analysis of the analytics could be undertaken to understand the needs or guidance viewed on a national level, for instance, whether there are regional differences in the needs in Germany versus those in the UK.

Several tutorials and pages about community engagement are not discoverable because they do not appear in the menu. More is required to expose all available support in a systematic way. 

While we attempt to evaluate the conversions (where there is a concrete action that is the result of having viewed some page), at best we can only approximate what this would manifest as, in the context of guidance/tutorials. There may, with sufficient information, be a way to see, for example, whether some guidance specifying the use of GitHub corresponded to some GitHub commits. We could also look further to delineate between new users and returning users. 


# Task 2: User Stories
To classify the tasks and objectives of our users’ needs with respect to Bioschemas, we decided to collect ‘User Stories’, in the form: \
As a `<persona>` I want to `<task>` so that `<objective>`.

We proposed a set of personas in advance and supplemented these as we moved through the exercise with different participants.
The set of personas we created in advance: Data steward, Developer, Researcher, Manager, Trainer. These were supplemented with ‘Systems Administrator’ and ‘Explorer’.

## Main outcomes
These stories were collected through Miro, and the original set, organised by Persona, are shown in Appendix 2.1. To further analyse this information, we clustered further (Appendix 2.2). This provides a way to organise the tasks into whether they are inward facing (or external facing (for instance a developer may be internally organising Bioschemas for their source, or externally looking to harvest available markup outside of their control). We also identified possible knowledge paths, which could be likened to ‘[Learning Paths](https://elixir-europe.org/internal-projects/commissioned-services/learning-paths-2018)’. We note that there are also objectives that are shared between personas, and tasks common across them.

![Pie chart showing types of persona surveyed](task-2.png)

To support the collection of user stories, we also hosted an online zoom drop in (Task 3). This provided us valuable information on user experiences in using Bioschemas, as well as indicating specific guidance that was missing. Examples of this include general guidance on metadata, guidance on what Bioschemas is useful for, and the difference between ‘Types’ and ‘Profiles’. We did find this information on the website, but it is not easy to locate. (see also Task 7 - UX/UI). A high level ‘infographic’ was also suggested by multiple participants as being highly desirable. We spun this off as Task 8.

## Next Steps

Using the clustering, we will be able to correctly annotate new and existing guidance as being appropriate to particular personas, taking into consideration those common tasks.  The ‘arrow’ in the ‘explorer’ persona (Appendix 2.2) could be expressed as a learning path, where an ‘explorer’ visits first to get general knowledge of metadata/schemas, moves further with knowledge of ‘bioschemas’, and then becomes proficient enough to ‘champion’ Bioschemas usage.


# Task 3: Drop in session to facilitate Task 2
![Screenshot from the drop in session, 17:00 CET, 6th Nov 2024](task-3.png)

A drop-in session was scheduled in the middle of the week, inviting Bioschemas users from outside the hackathon pool of participants to provide a focused set of contributions. We looked at the user stories, landscape and website accessibility. The discoveries were formally captured within the work of Task 2.


# Task 4: Assets

While the Bioschemas website does provide help and guidance, it is somewhat scattered, poorly ‘labelled’, and hard to find. To exacerbate this issue, the site itself does not have a search function (see also UX/UI, Task 7). This task was undertaken to document what guidance and help is available on the site, where it is located, and whether it is accessible through the menus (in particular, the top navigation bar and its drop down menus). Such activity is necessary to determine which guidance is already written, but hard to find, versus which documentation itself is missing. To execute this task, we started with the GitHub pages and matched ‘raw’ content (in GitHub) to its location on the Bioschemas (live web) site.

## Main outcomes

The [register](https://docs.google.com/spreadsheets/d/1pjHv7oKqt-RDcIWIL3r0MNISLj2JHRSL/edit?gid=1406033492#gid=1406033492) of assets includes documentation (by type), whether up to date, for materials both internal and available through some key external resources such TeSS and Zenodo. Some of the information here also ties into the web interface and usability of Bioschemas (Task 7).

1. Use cases are only available from the specification (profiles) & a page of use cases (under live deploys) which is not on the menu, and does not list all use cases.   
2. There is a 2nd repo for specifications but the link is labelled examples; not accessible (images in a table). The examples is different from the pop up (3)  
3. Profiles have pop up examples, but others are from repo (2)  
4. Can reach use cases from profile by the links tab \- could be clearer  
5. Could use more examples  
6. Table with black/blue on the tables is an accessibility issue (See Task 7 for more about accessibility issues)


As a concrete outcome in this task, we identified that no guidance for the only supported Bioschemas markup generator was available. This has now been [drafted](https://docs.google.com/document/d/1-NxWpJynnKoq4muF-3gE464zLxgzBJPAA4jBo7GY6B8/edit?tab=t.0), and will appear on the website once finalised. 

![Outcome 4.1 and 4.4: Navigating to use cases is only possible via Profiles and Types pages. There is an index of all use cases which is not in the menu.](task-4a.png)

![Outcome 4.2 and 4.3: There are different sets of examples depending which route you take through the Profiles and Types pages, some of which are stored raw in a different GitHub repository (Specifications). This second repository has an inconsistent file structure and gaps for the latest versions of some Profiles and Types (such as ComputationalTool).](task-4b.png)

## Next Steps

This information can be used in other tasks. Firstly, further work is required to organise the available materials logically, facilitating its accessibility through the web interface/search functions. This in of itself may help identify missing guidance. Secondly, this can be cross-referenced with what guidance and which type of guidance the different personas require. For example, a tutorial about markup for implementing bioschemas in github, versus a code example for a particular profile to implement in a web page. Thirdly, we can also check whether the guidance is up to date.


# Task 5: Guide to using markup generator

This task was undertaken as a subtask of Task 4, and has been completed.


# Task 6: Governance for contributions

There exists [governance documentation](https://github.com/BioSchemas/governance/tree/master) for community contributions to profiles and types. It does not cover contributions to guidelines and documentation, which may be written by a wider set of personas, including those with less technical experience. Task 6 seeks to fill this gap, proposing additional governance for guidelines and documentation contributions. This task was deprioritised and will be revisited when possible. This would describe how users can contribute to missing guidance, help in its review, and would include for example the provision of templates to facilitate submissions.

Two ways of contribution are possible. Contributors can either submit their work via Google Docs or directly through GitHub, with the latter being our preferred option for convenience.

It is crucial to determine who will handle the review process, ensuring the materials align with our guidelines, serve the intended purpose, and are thoroughly tested.   
Any recommendations will need to be formally presented to the Bioschemas steering group for approval.

We need to clarify our objectives and provide contributors with general guidance on suitable content for submission. We might consider developing one or more templates to support this, which can then be presented to the committee. Templates may vary based on the type of contribution—examples include summaries, step-by-step guides, and overviews.

Current priorities: 

1. Our primary focus is on creating a step-by-step guide for implementing Bioschemas with content management systems (CMS). At this stage, we have one approach documented on GitHub using Jekyll.  
2. Introducing Bioschemas: For non-technical contributors, we should provide a general introduction to Bioschemas, including an overview of metadata and some descriptive guidance that doesn’t require coding.


# Task 7: UX/UI

The main point of entry to help for Bioschemas is surfaced as the Bioschemas web site. This was examined with respect to usability and interface aspects, with the aim to provide feedback to the Bioschemas Steering committee to identify improvements that could be made in both short and long term. 

## Main outcomes

We have created a list of improvements that could be made to the website to facilitate users’ needs in finding appropriate guidance for their particular persona. While the implementation of a ‘persona’ based search, or a decision tree based drill down tool to select appropriate guidance (as with Data Stewardship Wizard) may be worthy long term goals, shorter term implementations, such as a search button, should be easy to implement. The list of suggestions is shown below (Table 1).

After discussion on the technical effort required in implementing all requests listed in Table 1, consideration must be given to whether a re-implementation may be less resource-intensive. Implementation of requested features should be mindful of differing expertise levels with the existing infrastructure (1 week for an informed expert, versus 1 month for someone unfamiliar with the subject).


Bioschemas website UX/UI improvements proposed

| Category | Summary | Implementation Difficulty | Comment |
| :---- | :---- | :---- | :---- |
| New feature | Show the current page in the menu | Low | Could lift from [ETT](https://github.com/ELIXIR-Belgium/elixir-toolkit-theme) |
| New feature | Search the site | Medium | Could lift from ETT |
| New feature | Faceted search | Hard |  |
| New feature | Fly-out submenu navigation, and review navigation content | Medium | Bootstrap examples |
| New feature | Make a form for ‘propose new type’ instead of an email address | Low | Could lift from RDMkit |
| New feature | Breadcrumbs | Medium | Easier to manually add to metadata on each page |
| Improvement | Make titles closer match between page titles, heading and menu links | Low |  |
| Improvement | Full review of content, URLs, names, language | Hard |  |
| Improvement | Direct people to the profiles vs types description, make it obvious | Very low | Add heading within that page, link to it |
| Improvement | Simplify the group creation process | Hard | For discussion with Steering group |
| Improvement | Harmonise where the menus are; don't bury links to help inside paragraphs \- if its the only way to reach it | Hard |  |
| Improvement | Make desktop view wider to accommodate left side menu | Hard | Need mobile view to have equivalent |
| New content | Infographic why to use Bioschemas for mortals | Medium | See Task 8, could go on home or about page somewhere |
| New content | Visualisation of what is a profile and what is a type | Medium | Could be a decision tree or other graphic |
| New content | Contribution guide for content writers | Medium | Part of Task 6 |
| New content | Contribution guide for web developers  | Medium | README file, how to properly use Bootstrap, CSS/JS |
| New content | Give more description on the Properties page | Medium |  |
| Accessibility | Use accessibility tools to thoroughly check site  | Hard | Eg [WAVE](https://wave.webaim.org/)  |
| Accessibility | Improve colours of properties links in the Profiles table, eg remove ‘visited’ colour change | Easy | Uses colour alone to convey info, but it’s an inherited problem from Schema.org |
| Accessibility | Add ARIA markup, especially on the Profiles table, so links can be distinguished by screen readers | Medium | Identify other places where this is needed |



# Task 8: Infographic

Multiple participants across our activities stated their desire to have a high level infographic to serve as an entry point for Bioschemas.

## Main outcomes

The infographic could convey: 

* What is Bioschemas?  
* Why bother with markup?  
* What is the semantic web?  
* What's the difference between types and profiles?  
* How do I find out more?

In a short brainstorm session we have drafted one panel (or a 3 or 4 panel infographic) (Appendix 8.1). This showcases the concepts ‘cloud’ (the internet/www), the ‘you’, being central in the infographic, and the ‘relationship’ between them, which we represent as a ‘cloud’ of logos, which will be taken from the logos of the resources listed in the live deploys pages of bioschemas, with the objective to cast the user into a familiar environment, since they should hopefully recognise some of those logos.

## Next steps

More work is needed to converge upon the remaining ‘panels’ for the infographic. This can be undertaken in a community exercise, possibly on the bioschemas community call. Also during this event we had an icebreaker activity, where participants drew a colleague with their eyes shut (Appendix B).  



# Acknowledgements

- Led by: Nick Juty, Helena Schnitzer, Phil Reed
- Participants (on site): Emily Knight, Lucy Pelton, Deborah van Wyk
- Online: Leyla Jael Castro, Munazah Andrabi, Ulrike Wittig, Finn Bacall, Ginger Tseung
- Interactions with other groups: \#[24](https://github.com/elixir-europe/biohackathon-projects-2024/blob/main/24.md), \#[21](https://github.com/elixir-europe/biohackathon-projects-2024/blob/main/21.md) 
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
