Survol du calcul différentiel
=============================

Le calcul infinitésimal est une branche des mathématiques qui étudie les
changements continus. On peut le séparer en deux sous-domaines :
- Le calcul *différentiel* cherche à déterminer les *dérivées* de fonctions,
  à savoir leur taux de variation instantané.
- Le calcul *intégral* sert à *intégrer* des fonctions pour calculer
  l'accumulation de leurs valeurs.

Cette vidéo présente un survol du calcul différentiel.

Définissons le problème : on a une fonction :math:`f(x)` dont on cherche à
déterminer le taux de variation, c'est-à-dire l'inclinaison de la pente du
graphe. Une fonction qui augmente rapidement a un taux de variation élevé
tandis qu'une fonction constante a un taux de variation nul parce que la
valeur de :math:`f(x)` ne varie pas selon la valeur de x.

On peut calculer la pente d'une fonction en choisissant deux points et divisant
le changement selon l'axe y par le changement selon l'axe x. 

.. math::
   \\frac{\\Delta y}{\\Delta x} = \\frac{f(a + \\Delta x) - f(a)}{Delta x}

Par exemple, pour la fonction :math:`f(x) = 1 + 2x`, on peut choisir deux
points - l'un noté :math:`a` et l'autre, décalé d'une valeur :math:`\\Delta x`.
On applique la formule pour obtenir une pente de 2, ce qui signifie qu'en
augmentant :math:`x` d'une unité, la fonction :math:`f(x)` augmente de deux
unités. Le résultat s'obtient facilement dans ce cas-ci parce que la pente est
identique partout sur la fonction, mais les choses se corsent pour des
fonctions plus complexes.

Par exemple, essayons de calculer la pente de la fonction :math:`f(x) = x^2` au
point :math:`x = 1`. La pente représente la vitesse à laquelle la valeur
:math:`f(x)` varie. On peut l'illustrer avec une tangente - une ligne qui touche
la fonction en un seul point. Pour approximer la valeur de la pente, on peut
utiliser l'équation précédente.

.. math::
   \\frac{\\Delta y}{\\Delta x} = \\frac{f(a + \\Delta x) - f(a)}{Delta x}

On a besoin de deux points. On choisit :math:`x = 1; f(x) = 1` pour le premier
et :math:`x = 2; f(x) = 4` pour le second. La ligne qu'on obtient avec cette
méthode se nomme sécante et l'on voit qu'elle est une mauvaise approximation de
la tangente. Afin d'améliorer le calcul de la pente, on peut rapprocher le
second point du premier. Par exemple, en choisissant
:math:`x = 3/2; f(x) = 9/4`, on obtient une sécante plus près de la valeur
recherchée. On peut continuer ainsi en choisissant des points de plus en plus
rapprochés pour améliorer le calcul de la pente. Plus formellement, ce
processus est représenté par la formule

.. math::
   f'(x) = lim_{\\Delta x \\to 0}\\frac{f(a + \\Delta x) - f(a)}{Delta x}.

Ce symbole, *la limite quand delta x tend vers 0*, signifie que l'on calcule la
valeur vers laquelle la fonction converge à mesure que :math:`\\Delta x`
s'approche de 0. Voyons voir comment en calculer cette expression.

Partie I : les limites
----------------------

Une limite est la valeur qu'une fonction approche quand l'entrée de la fonction
approche une certaine valeur.

Par exemple, supposons qu'on veuille déterminer la limite de la fonction
:math:`(x^3)/2 - x` quand x approche la valeur 2. En sélectionnant des valeurs
de x qui se rapprochent de 2, on évalue la fonction f(x). Le tableau montre que
la fonction converge vers la valeur 2 et la limite est ainsi égale à deux.

Un autre exemple : on cherche la limite de la fonction :math:`(x^3 -1)/(x -1)`
quand x tend vers 1. La fonction n'est pas définie au point :math:`x = 1` parce
que, si l'on remplace x par cette valeur, on obtient une division par 0. On
peut toutefois évaluer la limite : en choisissant des points qui se rapproche
de :math:`x = 1`, on voit que la fonction s'approche de la valeur 3. Même si la
fonction n'est pas définie à cet endroit, sa limite peut donc être évaluée.

Examinons un autre cas avec la fonction :math:`1/x` où l'on cherche la limite
quand x tend vers 0. On voit sur le graphe que la fonction approche des valeurs
différentes selon le côté d'approche. En partant de la droite, f(x) tend vers
une valeur infinie positive. On représente cette direction d'approche en
ajoutant le symbole "+" dans l'écriture de la limite. On peut aussi approcher
la valeur :math:`x = 0` à partir de la gauche, ce que l'on représente avec le
symbole "moins" et on peut voir que la limite à gauche est moins l'infini.

Revenons au calcul de la dérivée. On cherche à évaluer l'expression

.. math::
   f'(x) = lim_{\\Delta x \\to 0}\\frac{f(a + \\Delta x) - f(a)}{Delta x}

pour obtenir le taux de variation instantané de la fonction. Après avoir
développé et simplifié l'expression, on obtient

.. math:: .. limite de 2a plus delta x quand delta x tend vers 0
   f'(x) = lim_{\\Delta x \\to 0}\\2a + \\Delta x.

Puisque delta x tend vers 0, sa valeur devient de plus en plus négligeable par
rapport au terme 2. La limite de cette expression est donc égale à deux, ce
qui correspond au taux de variation instantané de la fonction :math:`x^2` au
point :math:`x = 1`.

Au lieu de calculer la dérivée en un point particulier, on peut utiliser un
point x quelconque. En réutilisant la démarche précédente et en utilisant cette
fois x à la place de la valeur 1, on arrive au résultat

.. math::
   f'(x) = 2x

À propos, le symbole f'(x), inventé par Euler et popularisée par Lagrange,
n'est pas le seul symbole pour représenter les dérivées. On peut aussi utiliser
la notation de Leibniz - d sur dx, ou encore, la notation de Newton, qui
consiste à ajouter un point sur la variable dépendante.

On peut utiliser la définition de la dérivée et le concept de limite pour
calculer la dérivée d'autres fonctions. Par exemple, en utilisant la même
expression, on peut calculer la dérivée de la fonction :math:`1/x`. Il existe
néanmoins des techniques qui simplifient le calcul des dérivés; nous allons
voir quelques-unes d'entres elles.

Partie II : quelques règles de dérivation
-----------------------------------------

Commençons par la dérivée d'un terme constant : en appliquant la définition de
la dérivée, on obtient une valeur nulle pour toute constante c.

Une autre technique importante est la règle des puissances. Pour une fonction
:math:`x^n`, la dérivée est égale à l'expression :math:`nx^{n - 1}`. On peut
utiliser cette règle pour dériver des fonctions avec des exposants réels,
qu'ils soient positifs, négatifs, ou encore fractionnaires.

La dérivation est une opération linéaire, c'est-à-dire qu'elle satisfait
l'équation suivante :

.. math::
   d/dx ah + bg = ah' + bg'

On en déduit les règles de la multiplication par un scalaire, la règle de la
somme et la règle de la différence.

La règle du produit stipule que la dérivée du produit de deux fonctions *f* et
*g* est égale à

.. math::
   f'g + fg'

On peut combiner la règle du produit avec, par exemple, la règle des puissances
pour calculer la dérivée d'une fonction composée d'un produit.

La règle de la dérivée en chaîne permet de calculer la dérivée d'un fonction
composée - ce qui se produit quand le résultat d'une fonction est utilisé comme
l'argument d'une autre fonction. Par exemple, si :math:`f(x) = x^2` et
:math:`g(x) = x - 1`, alors

.. math::
   f \\circle g = f(g(x)) = {(x - 1)}^2

La règle de la dérivée en chaîne est donnée par l'équation suivante :

.. math::
   f(g(x))' = f'(g(x)) g'(x)

En reprenant l'exemple précédent, on calcule ainsi :

.. math::
   \\frac{d}{dx} {(x - 1)}^2 = 2{(x - 1)}^{2 -1} \\frac{d}{dx} x = 2(x - 1)

Il existe beaucoup d'autres règles pour dériver des fonctions, par exemple,
trigonométriques, exponentielles ou logarithmiques, qui sont présentées dans
des ressources plus complètes. 

Partie III : valeurs maximales et minimales
-------------------------------------------

Le calcul différentiel peut servir à déterminer l'emplacement des maximums et
minimums - les extrêmes - d'une fonction, c'est-à-dire des valeurs de f(x) qui
sont plus grandes ou plus faibles que les valeurs environnantes. On remarque
que si la pente est positive, on peut trouver une valeur de x à sa droite qui
entraîne une valeur de f(x) plus grande. Si la pente est négative, on peut
trouver une valeur de x à gauche qui entraîne une valeur de f(x) plus grande.
Par conséquent, les extrêmes sont forcément situés à des points où la dérivée
de la fonction est nulle. Pour trouver les extrêmes d'une fonction, il suffit
donc de la dériver et de trouver ses racines.

Par exemple, en reprenant la fonction :math:`f(x) = (x^3)/2 - x`, on applique
la règle des puissances pour trouver sa dérivée : :math:`f'(x) = 3/2 x^2 - 1`.
En résolvant pour trouver les racines, on peut déduire l'emplacement des
extrêmes.

Partie IV : quelques applications du calcul différentiel
--------------------------------------------------------

Les dérivées sont utilisées dans de très nombreux domaines; cette section
présente quelques exemples d'applications simples.

On peut utiliser la dérivation pour calculer la vélocité d'un objet en fonction
de sa position. Disons que la fonction :math:`x(t)` décrit la position en
mètres d'un objet en fonction du temps *t* en secondes. La vélocité correspond
à la vitesse à laquelle la position change; on peut ainsi l'obtenir en dérivant
la position pour arriver à :math:`x'(t)`, en mètres par secondes.
L'accélération décrit la vitesse à laquelle la vélocité change; on peut donc
l'obtenir en dérivant la vélocité, ce qui nous donne :math:`x''(t)` en mètres
par secondes par secondes. Les fonctions de la vitesse et de l'accélération
permettent ensuite d'obtenir des informations utiles pour comprendre la
trajectoire de l'objet, par exemple, les moments où l'objet est immobile ou les
périodes d'accélération plus intenses.

Les dérivées permettent aussi de comprendre les circuits électriques. Un
condensateur, par exemple, est un composant simple qui peut emmagasiner des
charges électriques. Le courant électrique *i* qui traverse le condensateur en
fonction du temps est lié à la capacité *C* spécifique au composant et à la
dérivée de la tension électrique.

.. math::
   i(t) = C \\frac{dv(t)}{dt}

La dérivation permet ainsi de comprendre les courants électriques dans les
circuits.

Le calcul différentiel est intimement lié au calcul intégral. L'intégration est
en fait l'opération inverse de la dérivation. Elle permet de calculer une
accumulation de valeurs afin d'obtenir, par exemple, l'aire exacte de surfaces
irrégulières ou encore la position d'un objet en fonction de sa vitesse.


En résumé
- Le calcul différentiel est le domaine du calcul infinitésimal qui sert à
  déterminer le taux de variation instantané d'une fonction.
- À l'aide de la notion de limite, on élabore la définition de la dérivée.
- Il existe des règles qui permettent de dériver des fonctions plus facilement
  sans passer par l'évaluation de limites.
- Enfin, le calcul différentiel est utilisés dans les problèmes où l'on
  s'intéresse à la rapidité avec laquelle des valeurs changent.
