---
title: 'BioHackathon Europe 2022 Paper for Project 3: Bioinforming'
title_short: 'BioHackEU22 #3: Bioinforming'
tags:
  - training
authors:
  - name: Marco Anteghini
    orcid: 0000-0003-2794-3853
    affiliation: 1, 2
  - name: Katarina Elez
    orcid: 0000-0002-6160-8701
    affiliation: 3
  - name: Selle Bandstra
    orcid: 0000-0002-0684-6811
    affiliation: 3
  - name: Rijuta Lamba
    orcid: 0000-0001-8323-4694
    affiliation: 4
  - name: Lisanna Paladin
    orcid: 0000-0003-0011-9397
    affiliation: 5
affiliations:
  - name: Wageningen University and Research, Wageningen, The Netherlands
    index: 1
  - name: Zuse Institut Berlin, Berlin, Germany
    index: 2
  - name: Freie Universität Berlin, Berlin, Germany
    index: 3
  - name: University of Oulu, Oulu, Finland
    index: 4
  - name: European Molecular Biology Laboratory, Heidelberg, Germany
    index: 5
date: 01 May 2023
cito-bibliography: paper.bib
event: BH22EU
biohackathon_name: "BioHackathon Europe 2022"
biohackathon_url: "https://2022.biohackathon-europe.org/"
biohackathon_location: "Paris, France, 2022"
group: Project 3
# URL to project git repo --- should contain the actual paper.md:
git_url: https://github.com/bioinform-org/biohackeu22-bioinforming-paper
# This is the short authors description that is used at the
# bottom of the generated paper (typically the first two authors):
authors_short: Marco Anteghini & Katarina Elez \emph{et al.}
---


# Abstract

Optimal formats to inform and engage young students in novel biology-related fields are short courses. Training schools, e.g. lasting for five days, can provide enough content to introduce students to an extensive overview of bioinformatics and scientific career opportunities. In this work, we define a five-day training school format tailored to three target groups of young students: high school students, undergraduate students in biology-related fields and undergraduate students in computational fields. We structure the content and sessions around learning areas consisting of learning topics, detailing the dependencies between them. For each learning topic, we define learning outcomes and learning activities. Moreover, we conceptualize a teaching platform to manage FAIRyfied (Findable, Accessible, Interoperable, Reusable) training materials that anyone will be able to use to design a new training school in bioinformatics.


# Introduction

## Background
Science promotes innovation and the growth of technology, which in turn stimulates the economic development of countries. Especially in underdeveloped countries, innovation and scientific drive could contribute to becoming competitive in the global economy [@lema2021]. Therefore, educating the next generation of scientists is essential for achieving progress. In particular, innovative fast-growing fields such as bioinformatics should receive more attention [@tastanbishop2014].

Science promotion and engagement of students at a young age can have a decisive influence on their decision to pursue a scientific career [@osborne2008]. To raise interest in science among the youth, a significant impact can be made at a pre-university level i.e. in the later years of high school education [@monroygarcia2020]. Free educational content is essential for stimulating young students and increasing their interest in bioinformatics, facilitating their future choice of higher education studies regardless of their social background [@moenkediek2022].

Non-governmental, non-profit organization Bioinformatika (Bioinform) aims to achieve this goal by offering various free-of-charge training events. One of the main event formats that Bioinform organizes is a one-week training school designed to introduce the participants to the most relevant topics in bioinformatics and stimulate their curiosity for science learning. This NGO originated from the “BioINForming - Pilot” project, supported by the European Commission through the 2nd call of the Western Balkans Alumni Association (WBAA) in 2021. During this pilot project, the founders of Bioinform organized a five-day training school in bioinformatics for high school students in Montenegro in January 2022. Moreover, a survey was conducted among young students (105) in Montenegro to get insights into their background knowledge and interest in bioinformatics.

In this paper, we present our improved method for designing a five-day training school in bioinformatics tailored to three different target groups: high school students, undergraduate students in biology-related fields and undergraduate students in computational fields. We also show specific use cases. During ELIXIR BioHackathon Europe 2022, we worked with other ELIXIR members and specialists to better define our training school content concerning learning areas and learning topics with their inter-dependencies. It allowed us to associate realistic learning outcomes and the related learning activities to perform. Moreover, we defined a database structure to implement a teaching platform that enables interested trainers to create tailored training schools in bioinformatics.

## Learning principles

### Definitions

- **Learning area**. A learning area is defined as the “Grouping of traditionally discrete but related subjects with the explicit aim of integrating students’ learning” [@unesco2013].
- **Learning topic**. In this work, we define learning topics as teaching units that include a presentation of the theory (corresponding to a learning outcome) and one or seveal learning activities (e.g. an exercise corresponding to a learning outcome). Our topics usually cover two or fewer hours of teaching.
- **Learning path**. Selection and interconnection of learning topics tied together for learners to progress through, while mastering a particular subject or program [@nabizadeh2020].
- **Learning outcome**. "Totality of information, knowledge, understanding, attitudes, values, skills, competencies or behaviors an individual is expected to master upon successful completion of an educational programme" [@unesco2012].
- **Learning activity**. The specific activity that will support learners to achieve the learning outcomes. Learning activities are coupled with specific learning outcomes at each level of the Bloom's taxonomy [@bloom1956]. They can refer both to theoretical lectures and to practical exercises. The Bloom's taxonomy is summarised subsequently.

### Bloom's taxonomy

Bloom’s taxonomy is a set of six levels reflecting the cognitive domain [@bloom1956]. These six levels represent complexity and specificity that classify the educational learning outcomes. Table 1 shows more details on each of Bloom’s levels.

| **Level** | **Level description** |
| :--- | :--- |
| 1 | Remember (recall or reiterate information)|
| 2 | Understand (demonstrate understanding of facts)|
| 3 | Apply (apply knowledge to real/new situations)|
| 4 | Analyse (resolve ideas into simple parts, identify patterns)|
| 5 | Synthesize (pull ideas into a coherent whole, create new ideas)|
| 6 | Evaluate (make and defend judgments, assess theories and outcomes)|

Table: Description of Bloom's levels.


# Acknowledgments

This work was funded by ELIXIR, the research infrastructure for life-science data. We are also grateful to the Investment-development fund (IDF) of Montenegro for their support. We thank Anna Spackova, Alexia Cardona, Renato Alves, Denise Slenter, Bérénice Batut, Linelle Abueg, Suchitra Thapa and Gültekin Ünal for their valuable suggestions.


# References
