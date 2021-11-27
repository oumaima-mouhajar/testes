
**Partie I
Informations générales** 
**1- Nom et prénom**
 Mouhajar oumaima 
**1- Actuallement vous**
actuellement étudiante de l’ecole marocaine des sciences de l’ingénieur EMSI
**1-Vous voulez travailler en tant que**
1- A- developpeuse frontend 

**Partie II**
**Questions Générales**
**1 -C'est quoi**
- **Git** est un logiciel de gestion de versions du code d’un projet informatique.il s’agit d’un programme qui créé différentes versions d’un projet au fur et à mesure que les fichiers sont édités.    
**Sass** est un langage de script preprocesseur.qui est compilé ou interprété en css 
**Composer** est un logiciel gestionnaire de dépendances libre écrit en php . Il permet à ses utilisateurs de déclarer et d'installer les bibliothèques dont le projet principal a besoin.
**Object pool pattern** object pool pattern  est un modele de conception de creation de logiciels qui est utilise dans les situations où le coût d'initialisation d'une instance de classe est très élevé.
**A quoi sert la commande git diff** 
   Affiche la différence  entre les commits ,les  branches, les fichiers, et bien plus
  **Javascript**
  **C'est quoi Cors**
 est un mécanisme qui consiste à ajouter des en-têtes HTTP afin de permettre à un agent utilisateur d'accéder     à des ressources d'un serveur situé sur une autre origine que le site courant.
 **C'est quoi la différence entre  == et  === 
  - **==** c'est un test d'égalité est utilisé pour la comparaison entre deux variables quel que soit le type de la variable. par contre  **===**  est utilisé pour une comparaison stricte entre deux variables c’est à dire que cela vérifiera le type et la valeur des deux variables
 **Qu'est ce que return  if("0" == "true")**
 -false 
 **Qu'est ce que  this?**
 est un opérateur et comme tout opérateur il retourne une valeur provient d'un contexte d'exécution.
  **CSS**
  **Expliquez la différence entre le comportement de  inline  et  block**
le comportement de inline il va afficher les  éléments en ligne par contre block il va afficher les éléments
sous forme d’un bloc .
 **Est-il possible de créer un site web responsive sans media queries ?**
Oui c possible car on peut definir les dimension des bloc et division en pourcentages % et les polices en vh ou vw, mais on sera tres limités.
En utilisant les media queries on peut cibler un certain ecran/moniteur selon sa dimension et resolution et définir autant de style pour ces derniers
  **Expliquez les avantages/inconvénients de l'utilisation d'éléments inline-block ,  flex  ou float  .**
    les avantages  de inline-block est un meilleur moyen de  alignDIVs de manière consécutive, ce qui concerne 
    les inconvénients  un élément ne peut être affiché inline-block  s'il était déjà inline par défaut.
     Cela signifie qu'au lieu d'utiliser un élément <div>, vous devez utiliser un élément <span>.
    les avantages du float c'est que  prent automatiquement un comportement de type block s'il était 
    de type inline  ce qui concerne les inconvénients n'est pas adaptée à la mise en page  Un autre inconvénient
     est qu'il nécessite généralement un clearfix sinon, il peut casser les aspects de la page.
     **PHP**
   **Écrivez un programme qui imprimera des nombres de 1 à 100, avec les conditions suivantes :**
   <?php 
   for ($I =0; $I<=100 ; $I++){
     if($I%3==0)
     {
     echo "dev";
    }
    else if($I%5==0){
    echo "Ops";
    }
    else if (($I%3==0 ) && ( $I%5==0)){
     echo "DevOps.";
    }
     **1.  Ecrire une fonction qui vérifie si paramètre est en fait un nombre premier.**  
         <?php 
  function isPrime( $n){
          if(is_int( $n){
          if( $n<2){
         echo "Composite";
         }
         for ( $I =2; $I<( $n-1); $I++){
          if( $n  % $I == 0){
          echo "Composite";
          }
         }
         echo "Prime";
  }
    echo "Composite";

  }
?>
    **Que signifie**
     <?php
         $array= [3, 8, -4, 0, 2, -9];
         foreach ( $array as & $item):
             $item = ( $item >= 0)? $item : pow( $item, 2);
         endforeach;
         print_r( $array);
   
 la boucle foreach  nous permet de parcourir chaque élément du tableau et 
- chaque élément sera teste si il est supérieur ou égala 0 va rester  sans changement sinon va être a la puissance 2;
- quand la boucle foreach termine le tableau va être afficher 
**DATABASE**

**1.  extraire le nombre d'employés par jour s'étant inscrit**
   SELECT  count (id)  FROM employee GROUP BY create_at
   **2.  extraire les employés ayant fait l'inscription le  3/10/2021**
   SELECT id FROM  employee  WHERE create_at =  '2021/10/03'

   3.  **mettre first_name et last_name en lowercase**   
   SELECT LOWER(first_name),lowercase(last_name) FROM employee
   4 .  **modifier la column create_at  par date_creation** 
   ALTER TABLE employee 
  RENAME COLUMN create_at  TO  date_creation
  5  **c'est quoi la differnce entre  delete   et truncate**  
   truncate supprime toujours toutes les lignes d'une table, laissant la table vide et la structure de la table intacte alors que       delete  peut supprimer conditionnellement si la clause where est utilisée.
   ** 6-imprimer la liste des employés qui ont un salaire plus que la somme de deux salaires minimum**
   SELECT id ,MIN(salaire) as sal FROM employee  where salaire > sum(sal +sal )
    Partie III

    Pratique
    cette partie n'est pas bien expliquer.
