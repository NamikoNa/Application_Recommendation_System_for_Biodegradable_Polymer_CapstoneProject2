# CapstoneProject2_Application_Recommendation_System_for_Biodegradable_Polymer
## Project Title: 
Application Recommendation System for Biodegradable Polymer

## < Problem and Goal >  
Developing new applications of a polymer is one of the most important and challenging steps to sell a polymer as a product. It requires a wide range of knowledge about polymer itself (physical property, formability, etc.) and products that might already exist or might not yet. The goal of this project is to make an application recommendation system that gives some hints about potential applications for a given polymer by a user. A biodegradable polymer has been chosen as a polymer kind for this project. I was a polymer scientist for more than 10 years. I created what I had wanted at the time. 

## < Abstract >  
Patent information was used for this project, and the data were acquired from [WIPO](https://patentscope.wipo.int/search/en/search.jsf). To understand the data and make a decent model, the exploratory data analysis was implemented about the countries, polymer kinds, application kinds, and language variety of the abstracts. According to a pre-trained language identification model by [fastText](https://fasttext.cc/), the data included 19 kinds of languages in the abstracts, and 90% of the abstracts were written in English or Japanese. This wide language variety made this project more complicated, interesting, and worth pursuing to obtain multi-skills. I decided to use English and Japanese abstracts to calculate the sentence similarities so that they could be used to prioritize the recommendation.  
  
Two application recommendation systems were created. One system accepts one patent and another accepts two IPC codes as input by a user, and they provide 10 potential applications. The recommendation systems use two features to extract potential applications, a network and sentence similarity. The network has information about patents and IPC codes, and is used to extract the neighbor patents of an input patent (or two IPC codes.) Sentence similarities of patent abstracts were calculated by cosine similarity. The similarities are used to prioritize the neighbor patents so that the system can pick up the most similar patents and therefore the most prospective applications.  
  
  
## < Table of Contents >  
### 1. Codes  
[CapstoneProject2_codes.ipynb](https://github.com/NamikoNa/Application_Recommendation_System_for_Biodegradable_Polymer_CapstoneProject2/blob/master/CapstoneProject2_codes.ipynb)  
  
### 2. Reports  
Project proposal: [CapstoneProject2_ProjectProposal.pdf]()  
Milestone report 1: [CapstoneProject2_MilestoneReport1.pdf]()  
Milestone report 2: [CapstoneProject2_MilestoneReport2.pdf]() 
**☆ Final report:** [CapstoneProject2_FinalReport.pdf]()  
  
### 3. Presentation  
  **☆ [CapstonProject2_PresentationSlide]()**  
  
### 4. Figures
System 1 workflow: [system_1.png](https://github.com/NamikoNa/Application_Recommendation_System_for_Biodegradable_Polymer_CapstoneProject2/blob/master/system_1.png)
System 2 workflow: [system_2.png](https://github.com/NamikoNa/Application_Recommendation_System_for_Biodegradable_Polymer_CapstoneProject2/blob/master/system_2.png)
  
This project was conducted as a part of the Data Science Career Track Course at Springboard. My deepest appreciation goes to them, especially to my mentor, who gave me constructive comments and warm encouragement.  

