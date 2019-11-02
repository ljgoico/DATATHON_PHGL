<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# COOKIES
*[Hernando Cardenas]*
*[Laura Jimenez]*
*[Gustavo Denes]*
*[Paula Gual]*

*[datapt-bcn, Barcelona & 2019]*

## Content
- [Project Description](#project-description)
- [Organization](#organization)
- [Hypotheses / Questions](#hypotheses-/-questions)
- [Dataset](#dataset)
- [Cleaning](#cleaning)
- [Analysis](#analysis)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [Workflow](#workflow)
- [Links](#links)

<a name="project-description"></a>

## Project Description
Este proyecto se trata de solucionar el overstock en una fabrica de galletas, lo empezamos a tratar como un problema de multiclasificacion de galletas para luego enfrentarlo como un problema de clasificacion binaria para decidir si producir o no esa galleta. 

<a name="hypotheses-/-questions"></a>

## Organization
* Se repartio el dataset entre el grupo para tratar 4 variables por integrante y luego de esto se fueron probando distintos modelos
* Gestion de tareas con Trello


<a name="links"></a>


## Hypotheses / Questions
* Las galletas con mas calorias son las de mayor calidad.
* 


<a name="dataset"></a>

## Dataset
· Categóricas: Butter type | Mixins
· Ordinales: Aesthetic Appeal | Quality [TARGET]
· Nominales: Sugar to flour ratio | Sugar index | Bake temp | Chill time | Calories | Density | pH | Grams baking soda | Bake time | Weight | Diameter | Crunch Factor
   

<a name="cleaning"></a>

## Cleaning
Los nulos se han rellenado con la media en una nueva columna para no interferir en el modelo de ML.
La columna Diameter se ha eliminado al no aportar valor.
Se han eliminado filas que contenían un valor negativo -99.


<a name="analysis"></a>

## Transformation
· 2 tipos One-hot Encoder con los ‘Mixins’:
    · Por cada grupo de ingredientes.
    · Por cada ingrediente.
· One-hot Encoder con ‘Butter type’.
· Agregación de nuevas columnas con las medias para que posteriomente no afecte al modelo de Machine Learning.



<a name="transformation"></a>

## Analysis
* Exploratory Data Analysis
*

<a name="model-training-and-evaluation"></a>

## Model Training and Evaluation
*Random forest
*Extra Tree Clasification
*Light Gbm
*Svm

Tomamos el Random Forest Classificator, train 0.85, train 0.82 
Tambien se ha intentado aplicar deep learning


<a name="conclusion"></a>

## Conclusion
*Random Forest es el algoritmo que parece ajustarse mejor al problema.
*Se miden las feature importances. Las m{as importantes son: bake temp, calories, density y ybake time.

<a name="future-work"></a>

## Future Work
*Mejorar el Deep learning
*Seguir con el hypertunning del modelo.

<a name="workflow"></a>

## Workflow
* Import data
* Preprocesamiento
* EDA
* Featuring Engieneering
* Model Creation
* Documentation

<a name="organization"></a>



## Links

[Repository](https://github.com/ljgoico/DATATHON_PHGL)  
[Slides](https://docs.google.com/presentation/d/18JBxvt7ROJkJVM4BYfFeF6R7oLd8UZpygja8Za_tOR0/edit?ts=5dbd5ff3#slide=id.g65a56bf312_0_918)  
[Trello](https://trello.com/b/GeKD7yOD/dathaton)  