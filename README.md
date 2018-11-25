# Programmeerproject

Note before reading: for now the description of the project might be to vague. This is because I had limited time to work on this document due to sickness. However I hope it will give insight in my current idea and will inspire feedback on how to make it more precise. 


##### Thomas Hoedeman - 10318070

##### Goal:
Make the relationship between different mental disorders and symptoms insightful.

## Problem statement
When searching for information on mental disorders, these disorders are represented as distinct categories with clear demarcation.
However, practice shows that mental disorders are strongly related and share symptoms and/or problem areas. Furthermore disorder rarely present them in a uniform way and often people can be diagnosed with multiple disorders (high comorbidity). The public view of mental disorders lacks understanding of the relatedness and causality between underlying symptomatology that crosses categorical borders.

###### Network representation of relatedness between symptoms of DSM disorders:

![alt text](/Figures/Small_world.png)
_**Source**: Borsboom, D., Cramer, A. O., Schmittmann, V. D., Epskamp, S., & Waldorp, L. J. (2011). The small world of psychopathology. PloS one, 6(11), e27407._

## Solution

#### *Make the relationship between different mental disorders and symptoms insightful.*


My solution for this problem is an interactive website that displays an overview of different mental disorders and data about how they are related on symptom level.

#### Description

When opening the index page a pop-up intro text
will describe the goal of the website/infographic,  including basic statistics (bar chart) about mental health in the Netherlands. This pop-up can be closed to view the index page.  

![alt text](/Figures/popup_bar.png)

#### Network of comorbidity

The index page will display a network of mental disorders. The links display meaningful connections between the disorders. The size of the area that the disorder takes should correspond to the prevalence. Each line represents the comorbidity rate between these disorders. The line length and/or thickness should correspond to the rate. The network gives the option to link in other information as well , for example about the influence of social environment or physical health.

![alt text](/Figures/Network_disorders.png)

#### Specific disorder information

When clicking on a disorder, a  popup will  (preferably in a Prezi-like zoom, however this might be hard to implement).
In the popup for this specific disorder, a small description of the symptoms and basic statistics should be displayed. These statistics should include prevalence across different groups such as age and sex.

Furthermore and most importantly, information on how this disorder is related to other disorders in comorbidity and symptom overlap

Description:
A short description of the disorder and a list of the symptoms will be displayed
![alt text](/Figures/depression.png)

General statistics:
A bar graph will be used to inform about prevalence across age and gender. You will be able to select which information you want to view.
![alt text](/Figures/depression_bar.png)

Comorbidity:
An interactive view of comorbidity of this disorder with other disorders with the current disorder at the center
![alt text](/Figures/comorbidity_depression.png)

Symptom overlap:
![alt text](/Figures/depression_anxiety_overlap.png)

#### Additional features

Additional features that would exceed the minimum viable product would focus on brain related information.

Potentially the starting network can be linked to brain areas that are involved in the disorders. If you look at the picture below the data could be represented in a network formed like the brain and the disorders could be placed on the areas that are highly involved in the symptomatology

![alt text](/Figures/brainnetwork.jpg)

Example of how disorders can be linked to the brain:

![alt text](/Figures/braind_disorders.png)

Furthermore for each disorder specific information about

For this website I think the hardest part is the fact that I aim to integrate information from mutiple sources. This makes it potentially to much work to gather all information for many different disorders. Therefore it is important to select not too many disorder, but still be complete.

## Prerequisites

#### Datasources
* [prevalence](csb.nl) of mental disorders in the Netherlands, JSON format
* [comorbidity rates](http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/articles_541pdf.pdf), data has to be implemented in csv or json.
* symptom overlap infographics are not number based, has to be taken from literature

#### External components
* D3
