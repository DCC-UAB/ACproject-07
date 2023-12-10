[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/6QlcYoOP)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=13022155&assignment_repo_type=AssignmentRepo)

# Grup 07

## Integrants 
* Ariadna Lucero
* Laura Marín
* Marta Monsó 
* Mercè De la Torre

## Tema
Mental Health Students

Volem respondre: _Quina és l'impacte de l'estat mental dels estudiants sobre el rendiment acadèmic?_

y: mbi_ea

## Evolució projecte

### Starting point 1

### Gaussian Mixture
Tenint que el starting point 1 tracta el model KMeans, hem volgut indagar amb el clustering i provar un altre mètode com el Gaussian Mixture.
Veient els resultats dels clustering que ha generat GM:

               age        jspe   qcae_cog   qcae_aff       amsp  erec_mean  \
Cluster                                                                      
0        21.605210  104.639279  57.476954  34.246493  22.645291   0.713522   
1        28.243243  108.378378  59.689189  32.270270  25.756757   0.694015   
2        22.239617  108.667732  59.923323  36.236422  23.338658   0.736878   

              cesd     stai_t     mbi_ex     mbi_cy     mbi_ea  
Cluster                                                         
0        13.346693  39.140281  15.104208   7.931864  25.410822  
1        13.648649  37.324324  14.567568   9.324324  25.891892  
2        26.591054  50.207668  20.252396  13.680511  21.891374 

No tenim una clara distinció entre els 3 clústers. És cert que el State-Trait Anxiety Inventory (STAI) i mbi de cinisme poden aportar un certa diferència entre els clústers 0 i 1 amb el 2, però no creiem que sigui suficient. Per això, pensem que hem de continuar buscant un altre mètode.

#### Gaussian Mixtrue Modificat
A partir de la implementació de Gaussian Mixture basat en el starting point 1, fem possibles millores del model, com per exemple:
* Utilitzar l'eina GridSearch per trobar els millor paràmetres.
* Definir les hores d'estudi com a numèriques i no com a categòriques com tenim en el starting point 1. 


### Spectral Clustering