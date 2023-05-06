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


# Results

## Defining and classifying learning areas

Specific areas might have a different role in a specific training context. To structure the training materials, we defined three labels to assign to each learning area: basic (B), core (C\), and specialized (S). For example, when considering a training course, the B-labeled areas must cover information required to understand the other covered areas. The C-labeled areas are the ones that are essential to have a general overview of the main field of the course (e.g. bioinformatics). The S-labeled areas are optional and tailored to the audience. The S areas fully rely upon previous knowledge obtained from the B and C areas. Figure 1 shows the different areas we define.

![Classification of learning areas. The first row shows the basic (B) areas. The second row shows the core (C\) areas. The third and forth rows show six examples of the specialized (S) areas.](https://drive.google.com/uc?export=view&id=1i0stSDVNtK2gcpYdH4yOYgaAmk8920tJ)

## Defining and classifying learning topics

In order to provide a structured and comprehensive approach to scientific education, we have defined 20 learning topics. Each learning topic is grouped under a specific learning area, as visible in Table 2.


| **Learning Topic**               | **Learning Area**                 |
| -------------------------------- | --------------------------------- |
| Cell biology                     | Biology                       |
| Molecular biology and genetics   | Biology                       |
| Biochemistry and biophysics      | Biology                       |
| Shell scripting                  | Computational methods         |
| Programming                      | Computational methods         |
| Bioinformatics definition        | Interdisciplinary integration |
| NGS concepts                     | Interdisciplinary integration |
| Biomedical databases concepts    | Interdisciplinary integration |
| Structure determination concepts | Interdisciplinary integration |
| Sequence alignment               | Molecular sequence analysis   |
| Sequence data format             | Molecular sequence analysis   |
| Sequence database search         | Molecular sequence analysis   |
| Genomics/Epigenomics             | Omics                         |
| Transcriptomics                  | Omics                         |
| Proteomics/Interactomics         | Omics                         |
| Metabolomics                     | Omics                         |
| Protein structure                | Molecular structure analysis  |
| Structure data format            | Molecular structure analysis  |
| Structure prediction             | Molecular structure analysis  |
| Structure visualization, comparison and classification |Molecular structure analysis|

Table: Learning topics and their respective learning areas.

Each of these learning topics has been carefully selected to provide students with a deep understanding of the scientific disciplines they cover. By grouping these topics into specific learning areas, we aim to provide a structured approach to learning that allows students to build on their knowledge and develop a comprehensive understanding of the subject matter.

## Dependencies among learning topics

To design a training path for our training school we followed the guidelines of "The Learning Path step-by-step protocol". The protocol refers to a project started in the ELIXIR Biohackathon Europe 2021 and further developed in the ELIXIR Biohackathon Europe 2022 [@cardona2022]. The protocol is field-agnostic and accompanied by guidelines for curriculum developers and trainers.

For the training on a specific topic to be effective, it may or may not require some previous knowledge from the learner. Consequently, it is essential to teach some modules before others, and eventually to assess that the learning of some topic happened before moving on to the dependent topic. After defining 20 topics which we consider essential to our training school, we captured the dependencies among topics creating a coherent learning path, as shown in Figure 2.

![Dependencies between learning topics.](https://drive.google.com/uc?export=view&id=1tiA8mx4JjH0UN8AMGbmA0z9fEbKPf2FE)

## Defining learning outcomes

To identify how the session content can be informative to the students and correctly target their level of knowledge, it is good practice to define learning outcomes by framing them as a continuation of the sentence "By the end of the lesson, the learner will be able to..." and using the verbs in the Bloom's taxonomy (or their synonyms) [@bloom1956]. 
As an example, the topic "Protein structure" can have different learning outcomes according to each of the six Bloom's levels (we only show 4 levels since 5 and 6 are meant for highly specialized individuals):

**Protein structure analysis**

1. Name the most important structure determination methods
2. Describe levels of protein structure
3. Use structure visualization tools
4. Compare different structure prediction methods

## Defining learning activities

Once the Bloom's levels and the learning outcomes are decided, it is possible to define one or more activities to reach these outcomes, for each of the topics.

We list three examples of learning activities associated to topic, level and outcome:

**Example level 1**

- Topic: Sequence data format
- Level: 1	
- Outcome: Classify the different molecular sequences in fasta format (e.g. protein or nucleic acids)
- Activity: Lecture and examples of different molecular sequences

**Example level 2**

- Topic: Molecular biology and genetics
- Level: 2	
- Outcome: Explain the central dogma of molecular biology
- Activity: Lecture on replication, transcription and translation

**Example level 3**

- Topic: Protein structure analysis
- Level: 3
- Outcome: Use structure visualization tools
- Activity: Visualize a protein structure using Biopython

## Use cases

### Use case 1 - Identify the species from DNA sequences 

**Area:** Omics

**Level:** 3

**Exercise:** Use the BOLD system for DNA Barcoding to identify the species from the DNA sequences provided in FASTA format. 

The DNA sequences are from the C oxidase subunit 1 mitochondrial gene (COX1 or COI) which is highly efficient for species identification.

**Steps:**

1. Open BOLD systems at https://www.boldsystems.org/index.php/IDS_IdentificationRequest, select the option "Species Level Barcode Records" and paste the FASTA sequence as shown in Figure 3.

![The first step of the exercise is for species identification. An unknown FASTA sequence is pasted in the text box on the BOLD Systems website.](https://drive.google.com/uc?export=view&id=1s9Q207HMN6X8lSwHYwkBxrBFH3y9nsZx)

2. Visualize the results and take note of the species found, as shown in Figure 4. The phylogenetic tree can also be visualized and interpreted (optional).

![The second step of the exercise for species identification. Visualize and take note of the found species.](https://drive.google.com/uc?export=view&id=1iJDq1zsX6uvU8ggBaQxtgL4mznH0fEPe)

3. Iterate the process until each sequence is associated with the corresponding species. The final results are visible in Table 3. 

| ID         | Organism                                 |
|------------|------------------------------------------|
| Unknown 1  | Pan troglodytes (Chimpanzee)             |
| Unknown 2  | Pan paniscus (Pygmy chimpanzee) (Bonobo) |
| Unknown 3  | Homo sapiens (Human)                     |
| Unknown 4  | Equus caballus (Horse)                   |
| Unknown 5  | Oryctolagus cuniculus (Rabbit)           |
| Unknown 6  | Bos taurus (Bovine)                      |
| Unknown 7  | Ovis aries (Sheep)                       |
| Unknown 8  | Homo sapiens (Human)                     |
| Unknown 9  | Canis lupus (Gray wolf)                  |
| Unknown 10 | Capra hircus (Goat)                      |

Table: The final results from the omics exercise. The first column contains a list of identifiers (IDs) while the second column represents the species associated to each sequence.

4. (Optional) Try to associate a protein sequence to each DNA sequence and report its UniProt ID.

### Use case 2 - Prepare the structure of a receptor protein for successive inhibitor detection.

**Area**: Drug discovery

**Level:** 4

**Exercise:** Use the provided scripts and software to access and modify the structure of a receptor protein to prepare it for docking.

The receptor protein is PDB:2NYY available from Protein Data Bank (PDB).

**Steps:**

1. Move into a specific working directory: \
``` cd /home/ubuntu/Desktop/<your_name>/practical5 ``` \
Create necessary subdirectories:\
```mkdir receptor ligands scripts dockings```\
Activate virtual screening environment:\
```conda activate virtual_screening```
2. Move into the ’receptor’ directory.
Open the PDB structure 2NYY in PyMOL. Considering the information available on UniProt (P0DPI0), export light chain of botulinum neurotoxin type A into a PDB file called ’botA_LC.pdb’. Note that the final structure should contain a zinc (Zn) atom, but no calcium (Ca) atoms.
3. Open ’botA_LC.pdb’ file in a text editor and find x, y and z coordinates of the C$C\alpha$ atom of glutamate (GLU) 262. Write these coordinates down for future reference.
4. Prepare receptor structure:\
```prepare_receptor4.py -r botA_LC.pdb -A hydrogens```
5. Open ’botA_LC.pdbqt’ file in a text editor and manually set the charge of the zinc atom to 2.000

### Use case 3 - Plot trends of publications on Artificial Intelligence in bioinformatics. Highlight challenges and ethical implications. 

**Area:** Interdisciplinary integration

**Level:** 5

**Exercise:** Go to PubMed (https://pubmed.ncbi.nlm.nih.gov/) and look for papers about Artificial Intelligence in specific time frames. Use the provided scripts (or create your own) to plot the trends, compare them and write your conclusions.

**Steps:**

1. Open the advanced search in PubMed and look for papers containing the words: "Artificial Intelligence", "Natural Language Processing", "Machine Learning", and "Deep Learning" in a specific time frame (e.g. from 1980 to 1985):\
***Query example:***
    ```
    ((((Natural language processing[Title/Abstract]) OR 
    (Artificial intelligence[Title/Abstract])) OR 
    (Machine learning[Title/Abstract])) OR 
    (Deep Learning[Title/Abstract])) AND 
    (("1980"[Date - Publication] : "1985"[Date - Publication]))
    ```

2. Repeat the search and annotate the results for time frames of 5 years until March 31st 2023. Fill the lists with the results from the queries.\
***Lists example:***
    ```
    time=['1985','1990','1995','2000','2005','2010','2015','2020','2023']
    n_of_p1=[90,272,386,506,1093,2897,7069,49398,103962]
    # n_of_p1 -> number of publications - 1st query
    ```
3. Repeat the search for the same time frames. This time add the words 'Ethic', 'Ethics' or 'Challenges' in the advanced search. Fill the list.\
    ***Query example:***
    ```
    ((((Artificial Intelligence[Title/Abstract]) OR 
    (Machine Learning[Title/Abstract]) OR 
    (Deep Learning[Title/Abstract]) OR 
    (Natural Language Processing[Title/Abstract])) AND 
    ((Ethic[Title/Abstract]) OR 
    (Challenges[Title/Abstract]) OR 
    (Ethics[Title/Abstract]))) AND 
    (("2015"[Date - Publication] : "2023-03"[Date - Publication]))
    ```
    ***List example:***
    ```
    n_of_p2=[1,4,8,14,36,117,355,3546,9862] 
    # n_of_p2 -> number of publications - 2nd query
    ```
4. Plot and compare the trends.\
    ***Plot code example:***
    ```
    import matplotlib.pyplot as plt
    
    # Create the plot
    plt.plot(time, n_of_p1, color='b', label='Paper on AI')
    plt.plot(time, n_of_p2, color='#77dd77',label='Paper mentioning Ethics\
    and Challenges of AI')

    # Set x and y axis labels
    plt.xlabel('Time steps')
    plt.ylabel('Number of publications')

    # Add legend
    plt.legend()

    # Adjust x-ticks spacing
    plt.xticks(rotation=45, ha='right')

    # Show the plot
    plt.show()
    ```
    ***Output:***\
    ![Trend in the number of papers published in a specific time range mentioning one of the following words: "Artificial Intelligence", "Natural Language Processing", "Machine Learning" or "Deep Learning". The blue line shows the general trend in the number of papers mentioning these words, the green line shows those that are also associated with the words: "Ethics", "Ethic" or "Challenges".](https://drive.google.com/uc?export=view&id=1kgPYeAmMCiIayu3qJUuqkb4WvCBNPmom)\

5. Write your conclusion. Are the trends identical? Do you think Challenges and Ethics of AI are well-represented in scientific publications? Motivate your answer.
    
## Teaching platform
To create and share FAIR training materials, we envisaged the construction of an open-access teaching platform. The platform will store training materials and provide suggestions for designing a new training event. The materials will be labeled with information such as area, topic, bloom’s level, outcomes, material type, authorship and time to perform the activity. Topic dependencies will be fundamental in providing suggestions for designining a learning path. An overview of the database structure underlying the teaching platform is visible in Figure 6.

![Database structure for the teaching platform.](https://drive.google.com/uc?export=view&id=1ngbGpfCdEyMcHiCxxdxNSFSVMOgzQXGK)

## Additional topics and tailored content examples

Tailored content is essential for a successful outcome in every training event. In particular, a 5-day training school risks being too condensed and overwhelming if not properly planned. For these reasons, we believe it is important to add certain flexibility to our training events, monitoring the students' during and after the training school implementation.\
Our format aims to provide a space for general discussion and soft skill improvement in parallel to our highly structured training materials.
In the regular call for applications to a training event, we ask questions like "How would you rate your interest in knowing more about the following topics?" and "What additional topics would you be interested in knowing more about?".\
Additionally, we dedicate sessions to complementary discussions for scientific training schools such as: "Career in bioinformatics", "Ethics and challenges of AI", "Environmental protection", "Gender imbalance in science" and "Erasmus exchange opportunities".\
As an example, the session "Ethics and challenges of AI" would consist of  a discussion on the challenges connected to the use of AI in healthcare. These include: ensuring patient privacy and data security, addressing issues of bias and fairness in algorithmic decision-making, and establishing accountability for the actions of AI systems. Also, practical challenges can be clustered in the following groups: data integration problems, training set bias and black-box characteristics.


# Conclusions

Preparation of training materials for a training school in bioinformatics tailored to different audiences requires a general structure that should both be flexible and well-planned. In this work, we show how to prepare a structure which can be adapted to different target groups. In particular, we define learning areas, learning topics and the dependencies between them. These dependencies define a learning path which can be a valuable resource while organizing training schools. It can work as a backbone for defining learning outcomes, that satisfy both the student and the trainer, through specific learning activities.\
We developed a five-day training school format that caters to three target groups of young students: high school students, undergraduate students in biology-related fields, and undergraduate students in computational fields. Our focus on interdisciplinary integration is reflected in the fact that four of the learning topics fall under the "Interdisciplinary integration" learning area. This reflects the growing importance of interdisciplinary approaches in scientific research, and our desire to prepare students to tackle complex scientific problems using a multidisciplinary approach. Our ultimate goal is to inspire young students to pursue careers in bioinformatics and related fields and contribute to scientific advancements.\
One of the main advantages of our format is its ability to provide students with a broad overview of bioinformatics and scientific career opportunities. The tailored content ensures that each group receives information appropriate for their level of knowledge and experience. We also incorporate general discussion and soft skill development to create a more engaging and interactive learning environment. Another important feature of our approach is the use of assessment forms during and after training to monitor student progress and evaluate the effectiveness of the training school. By soliciting feedback from students, we can gather information that can be used to improve future iterations of the training school.\
We believe the materials produced in our training initiatives should be FAIR and open to everyone interested in using them. Moreover, it should be possible for other trainers to easily contribute their training materials. For these reasons, we defined a structure for an open-source teaching platform. In the future, we envisage the implementation of such a training platform and the addition of new materials specific to different target groups that will participate in our training events.


# Acknowledgments

This work was funded by ELIXIR, the research infrastructure for life-science data. We are also grateful to the Investment-development fund (IDF) of Montenegro for their support. We thank Anna Spackova, Alexia Cardona, Renato Alves, Denise Slenter, Bérénice Batut, Linelle Abueg, Suchitra Thapa and Gültekin Ünal for their valuable suggestions.


# References
