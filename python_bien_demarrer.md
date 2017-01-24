# BIEN DÉMARRER AVEC PYTHON
> GNU/Linux Magazine n° 122 | décembre 2009 | Olivier Delhomme. Creative Commons	

# 1. LE LANGAGE
## 1.1 VERSION
Python, malgré son âge (il est né au milieu des années 80) est toujours en mouvement. De nombreuses fonctionnalités très utiles lui sont ajoutées a chaque nouvelle version. C'est une très bonne chose, mais il faut se méfier un peu plus qu'à l'accoutumée. En effet, avant d'écrire un programme, renseignez-vous sur le numéro de version de Python de la plate-forme cible (sur laquelle votre programme va tourner). Certains modules ou certaines définitions du langage n'apparaissent que dans une version donnée. Exemples : le module hashlib apparaît dans la version 2.5 ; multiprocessing apparaît dans la version 2.6 ; la clause « with » fait son entrée dans la version 2.5 (il y a bien d'autres exemples). Inutile d'utiliser ces modules ou cette clause si vous n'avez accès qu'à une version 2.4 ou antérieure.

## 1.2 ÉDITEUR
Le choix d'un éditeur est primordial car la structure du programme est définie par le nombre d'espaces que vous laissez devant vos lignes de code. Aussi, je vous conseille d'en utiliser un qui vous permet d'unifier le fichier en transformant les tabulations en espaces, de supprimer les caractères à la fin du fichier et à la fin des lignes. Le mieux étant que cela soit automatique lors de la sauvegarde du fichier source. En effet, il est préférable de n'avoir qu'un seul type de caractère pour l'indentation, celui recommandé étant l'espace (car c'est celui que l'interpréteur utilise [pep 8]).

Pour ma part, j'ai trouvé celui qui me convient et qui remplit parfaitement sa mission : geany [geany]. Je vous le conseille vivement. C'est un logiciel libre (licence GPL v2) disponible pour une très grande variété de systèmes (GNU/Linux, Windows, MacOS, OpenSolaris, *BSD, …). Il est simple, rapide, agréable à utiliser et propose la complétion automatique (qui fonctionne également avec vos propres classes, fonctions et variables).

## 1.3 LANGAGE INTERPRÉTÉ
Python est un langage interprété. Cela signifie qu'il n'y a pas d'étape de compilation à proprement parler. Il est possible d'écrire les commandes directement dans l'interpréteur, à la manière d'un bon vieux « Basic ». C'est d'ailleurs très pratique pour tester les choses...
```
[GCC 4.3.3] on linux2`
Type "help", "copyright", "credits" or "license" for more information.`
>>> print("Hello World")`
Hello World`
>>>`
```
… avant de les écrire définitivement et pour la postérité dans un fichier source justement nommé :

```
$ cat hello_world.py
#!/usr/bin/env python
# -*- coding: utf8 -*-
print("Hello World")
$ python hello_world.py
Hello World
$
```
Vous aurez remarqué la ligne de commentaire # -*- coding: utf8 -*- dans l'exemple. Il s'agit d'un marqueur (coding: utf8) qui indique le codage utilisé pour le fichier en lui-même. Ce marqueur peut sembler anodin mais, en réalité, il est important pour les chaînes de caractères que vous utilisez dans le programme (code, commentaires et docstrings y compris). C'est une bonne chose de toujours indiquer le codage de votre fichier. Par défaut, l'interpréteur utilise l'encodage ASCII, ce qui ne manquera pas de poser problème à vos accents !

## 1.4 LANGAGE OBJET
Python est un langage objet. En gros, tout est objet. Vous pouvez écrire vos propres classes, faire vos héritages. Je n'ai pas encore poussé mon investigation sur les limites du langage du côté de l'objet. Ce que je peux dire, c'est qu'une classe se crée très facilement.

La souplesse de Python permet l'écriture de programmes qui ne définissent aucune classe ou qui n'utilisent aucun objet (à vous). Vous pouvez parfaitement écrire un programme qui n'utilise que des fonctions (ou pas) et des appels à ces fonctions. Le meilleur exemple étant le hello_world.py que nous avons écrit plus haut.

## 1.5 STRUCTURES DE CONTRÔLE
Les structures de contrôle du langage sont constituées d'espaces ou de caractères de tabulation que vous laissez devant la ligne de code, en fonction du niveau auquel vous souhaitez qu'elle soit exécutée. En effet, il n'existe pas dans ce langage de structures telles les {} ou les BEGIN END pour indiquer les début ou fin de blocs. Ces structures ont été supprimées et c'est l'indentation (série d'espaces ou de tabulations) qui détermine entièrement le bloc. En C, on écrit (si on veut) :
```
if (nombre > 2) {
printf("Nombre : %d > 2", nombre);
  nombre += 1;
} else {
  printf("Nombre : %d < 2", nombre);
nombre *= 2;
}
```
La traduction Python s'écrit de manière directe :
```
if (nombre > 2):
    print('Nombre : %d > 2' % nombre)
    nombre += 1
else:
    print('Nombre : %d < 2' % nombre)
    nombre *= 2
```
Notez l'absence de ; à la fin des lignes, la virgule du printf qui se change en % dans l'appel à print (ici utilisé comme fonction, conformément aux usages dans Python 2.x). Remarquez que le seul caractère structurant restant est le : que l'on retrouvera systématiquement derrière les définitions de classes, de fonctions, les mots-clés if, while, else, elif (le else if), for, with, ..., j'en oublie certainement. Pour écrire selon les conventions, ne laissez pas d'espace avant et passez à la ligne directement après.

En parlant de passer à la ligne, il est conseillé de ne pas dépasser les fameux 80 caractères d'une ligne, cela tant pour des raisons historiques que pratiques. Avant, je n'y faisais pas vraiment attention. Mais maintenant que j'ai un portable dont l'écran fait 10,2 pouces de large, je suis reconnaissant à ceux qui ont limité leurs lignes à 80 caractères. J'en fais donc autant. Le caractère pour aller à la ligne est l'antislash \. Toutefois, le passage à la ligne est possible directement (sans caractère spécifique) entre une parenthèse ouvrante et une parenthèse fermante.

Personnellement, je trouve que le : est de trop. Je l'oublie très souvent et il n'apporte rien de plus au programme. Pour en savoir plus sur ce caractère de contrôle, visitez les pointeurs [contrôles] qui m'ont été indiqués par Victor Stinner.

1.6 LA BOUCLE 'FOR', UNE PARTICULARITÉ INTÉRESSANTE
La définition d'une boucle 'for' en Python se rapproche furieusement de celle que l'on peut écrire en bash. En effet, elle n'utilise pas de compteur spécifique comme en C ou en Pascal (les variables i et j classiques). Au lieu de cela, l'itération s'effectue sur une liste en égrenant les éléments les uns après les autres :

liste = ['navet', 'carotte', 'chou', 'poireau']
for legume in liste:
    print('%s est un légume !' % legume)
print('Il me manque quoi pour faire une potée ?')
Du coup, si l'on souhaite utiliser un compteur classique, soit on écrit la liste à la main, soit on utilise l'une des fonctions range([start,] stop [, step]) ou xrange([start,] stop [, step]). Les arguments start et step sont optionnels. Si vous n'indiquez qu'un seul argument, il s'agit de la valeur de fin. Ces fonctions génèrent des listes de nombres allant de start à stop avec un pas de step. Par exemple, on peut faire :

for i in xrange(2, 42, 3):
    print('%d' % i)
Il est préférable d'utiliser la fonction xrange() car elle génère les nombres au fur et à mesure. Elle est plus rapide car le temps de prégénération de la liste est supprimé. Elle est moins gourmande en mémoire car elle ne stocke pas la liste complète.

Toutefois, si vous voulez réaliser une boucle sur une liste ou un objet sur lequel vous pouvez faire des itérations, utilisez la première méthode. Elle est bien plus élégante et lisible. Si, comme moi, vous avez eu le vieux réflexe du compteur explicite, reprenez votre code pour le corriger en le supprimant. Le résultat n'en sera que meilleur !

1.7 LES TUPLES
Les tuples ressemblent en quelque sorte à une structure de données, sans en être vraiment une. Je ne vois pas vraiment d'équivalent parmi les langages que je connais. Je fais énormément usage des tuples dans les quelques programmes Python que j'ai écris. Je vois les tuples comme une liste de valeurs dont le type n'est pas forcément uniforme. Par exemple mon_tuple = ('rouge', 3, None, factorielle) est un tuple.

Les nombreux avantages des tuples :

- Il est très facile de regrouper plusieurs valeurs dans un même tuple (structure). On peut dès lors récupérer les valeurs avec une commande similaire : couleur, n, forme, fonction = mon_tuple . On me souffle que l'on peut utiliser les slices pour ne récupérer qu'une partie d'un tuple : n, forme = mon_tuple[1:2].

- Les valeurs d'un tuple peuvent être n'importe quoi, même des fonctions (qui ne sont finalement que des objets particuliers).

Le principal inconvénient réside dans le fait qu'il n'est pas possible de modifier une valeur dans un tuple. La seule façon de le faire consiste à recréer le tuple : mon_tuple = ('rouge', 3, rond, factorielle)

1.8 FONCTIONS
1.8.1 DÉFINITION

En Python, comme en C, il n'y a pas de différence (au niveau du langage) entre fonctions et procédures. Une procédure n'est qu'une fonction qui renvoie void en C et None en Python. Elles se définissent avec le mot-clé def :

def factorielle(n):
    if n < 0:
        return None
    elif n <= 1:
        return 1
    else:
        return n * factorielle(n-1)
Dans cet exemple, notez :

- l'usage de l'instruction elif (pour 'else if') ;

- None correspond en quelque sorte à NULL en C ou NIL en Pascal.

Notez également :

- qu'il est possible de définir des fonctions récursives ;

- que le code de retour n'est pas forcément d'un unique et même type (ceci impliquera obligatoirement une gestion de ce code).

1.8.2 PARAMÈTRES

Les fonctions ont le plus souvent des paramètres qui sont plutôt des paramètres obligatoires (comme dans l'exemple précédent). En Python, il est possible d'utiliser d'autres types de paramètres. Pour moi, le langage en définit quatre types en tout : les paramètres obligatoires classiques, les paramètres optionnels, les paramètres arbitraires et, enfin, les paramètres non explicites. Les deux derniers types sont laissés à la découverte du lecteur curieux ou feront l'objet d'un prochain article...

Réécrivons la fonction factorielle avec un paramètre optionnel :

def factorielle(n, debug=False):
    if n < 0:
        return None
    elif n <= 1:
        return 1
    elif debug == True:
        print('%d' % n)
        facto = n * factorielle(n-1, debug)
        print('%d : %d' % (n, facto))
        return facto
    else:
        return n * factorielle(n-1)
factorielle(5, True)
5
4
3
2
2 : 2
3 : 6
4 : 24
5 : 120
print('%d' % factorielle(4))
24
Vous noterez que :

- True et False s'écrivent avec la première lettre en majuscule ! Si vous l'oubliez, l'interpréteur vous le rappellera sèchement !

- Les paramètres optionnels sont nécessairement situés après les paramètres obligatoires. De plus, il n'est pas possible d'ajouter des paramètres obligatoires après des paramètres optionnels (un peu comme une va_list en C).

- Lorsque les paramètres optionnels sont omis lors d'un appel à la fonction, c'est leur valeur par défaut qui est utilisée.

Si vous utilisez une fonction qui comporte plusieurs paramètres optionnels, il est possible de les nommer lors de l'appel. Ce mécanisme permet d'omettre un (ou plusieurs) paramètre(s) optionnel(s), même s'il se trouve au milieu d'autres :

def change_user(uid, gid=600, shell='/bin/bash',
                comment='Un utilisateur'):
    """ici une fonction utile qui fait quelque chose !"""
On pourra par exemple appeler cette fonction comme suit :

change_user(530, shell='/bin/zsh')
change_user(530, gid=530, comment='Olivier DELHOMME')
En réalité, les appels seront respectivement identiques à :

change_user(530, 600, '/bin/zsh', 'Un Utilisateur')
change_user(530, 530, '/bin/bash', 'Olivier DELHOMME')
1.9 CLASSES
À parler de Python comme je le fais, on en oublie presque qu'il s'agit d'un langage objet et qu'à ce titre, il est possible de définir ses propres classes ! Le mot-clé pour définir une classe est class (en minuscules) !!

class une_classe:
    un_attribut = 'une chaine de caractères'
    def methode_speciale(self):
        print('%s' % self.un_attribut)
La classe s'utilise en donnant naissance à un objet :

>>> mon_objet = une_classe()
>>> mon_objet.methode_speciale()
une chaine de caractères
>>> mon_objet.mon_attribut = 'une autre chaine'
>>> mon_objet.methode_speciale()
une autre chaine
L'interpréteur appelle chaque méthode d'une classe avec comme premier paramètre le mot-clé self qui indique l'objet en cours lui-même. C'est pratique pour faire référence aux attributs ou aux méthodes de l'objet dans une de ses propres méthodes.

Ce qui, à mon avis, est intéressant, c'est qu'il est possible de définir des méthodes qui seront alors utilisées par l'interpréteur :

- __init__() qui est appelée lors de la naissance de l'objet. En général, on y initialise les valeurs par défaut des attributs. En tout état de cause, c'est une bonne idée de faire cela systématiquement dans cette fonction car j'ai eu quelques surprises en oubliant l'initialisation d'un attribut ;

- __len__() qui fournira la taille en nombre d'éléments de l'objet ;

- __iter__() qui devra fournir un itérateur permettant de parcourir les éléments ;

- __str__() qui renverra une représentation de l'objet sous la forme d'une chaîne de caractères (permet d'écrire : print('%s' % str(mon_objet))) ;

- __cmp__(autre_objet) que vous définirez si votre objet est comparable et dont le résultat sera fonction de la comparaison avec 'autre_objet' : 0 si les deux objets sont égaux, un entier négatif si autre_objet est inférieur et un entier positif si autre_objet est supérieur (à l'objet auquel s'applique la méthode de comparaison) ;

- et quelques dizaines d'autres possibilités, permettant notamment la définition d'objets multipliables, additionnables, inversables, etc. (pensez aux matrices, par exemple).

L'héritage est possible en spécifiant, lors de la définition de la classe, de quelle autre classe elle dérive : class portable(ordinateur):. Le langage semble posséder toutes les propriétés classiques d'un langage objet. Ne m'étant pas encore plongé dans cette partie, je vous laisse la découvrir !

2. DOCUMENTATION DU CODE
Pour moi, ce qui est très intéressant et qui se trouve directement au niveau du langage, c'est la possibilité de documenter le code que vous écrivez. Il y a deux mécanismes imbriqués pour réaliser cela. Les docstrings et les doctests.

2.1 DOCSTRINGS
Les docstrings sont des chaînes de caractères écrites directement après la déclaration d'une fonction, d'une classe ou d'un module (programme, un peu comme une unit en Pascal). Il faut les écrire au format de texte brut (préformaté). Elles sont encadrées par trois guillemets comme dans l'exemple de notre fonction factorielle :

def factorielle(n, debug=False):
    """fonction factorielle
    
    Retourne la factorielle de n si elle est définie
    et 'None' sinon. Le calcul est effectué
    récursivement.
    Lorsque debug est positionné à True, la fonction
    indique ce qu'elle fait."""
    
    if n < 0:
…
Ce qui est bien pratique, c'est qu'on peut demander l'aide de la fonction dès qu'on le souhaite. Dans l'interpréteur, on tapera volontiers help(factorielle) tandis que, dans le programme, on écrira, par exemple, print('%s' % factorielle.__doc__).

Bien entendu, toutes les fonctions de Python ont des docstrings qui documentent leurs usages respectifs. Cela facilite l'utilisation de Python et de ses fonctions.

2.2 DOCTESTS
Alors là, les doctests sont les outils indispensables qu'il faudrait rajouter à tous les langages qui n'ont pas la chance d'avoir un mécanisme similaire. Il s'agit de définir les cas d'utilisation des fonctions, des classes ou des modules. Ils s'insèrent dans les docstrings déjà écrits. Ainsi, ils seront affichés dans l'aide de la fonction.

C'est un excellent mécanisme pour réaliser les tests de cas d'utilisation, mais aussi ceux de non-régression. Il s'agit d'écrire un petit bout de code (en général un appel à la fonction elle-même). Ce code sera exécuté et sa valeur de retour comparée à une valeur attendue. Si ces dernières sont égales, tout va bien. A l'inverse, s'il y a une différence, une erreur est remontée.

Le code à exécuter est précédé de >>> ou de .... La valeur de retour attendue n'est précédée d'aucun signe. Lorsque vos fonctions renvoient à des objets ou à des structures complexes, l'astuce consiste à écrire, en plus de l'appel à la fonction, un test simple sur les attributs intéressants (ceux modifiés par la fonction, par exemple).

Voyons un exemple concret et parlant avec notre fonction factorielle :

def factorielle(n, debug=False):
    """fonction factorielle
    
    Retourne la factorielle de n si elle est définie
    et 'None' sinon. Le calcul est effectué
    récursivement.
    Lorsque debug est positionné à True, la fonction
    indique ce qu'elle fait.
    
    >>> factorielle(-1)
    None
   
    >>> factorielle(4)
    24
    """
    
    if n < 0:
…
Pour les cas plus complexes, scinder en tests basiques simplifie grandement :

>>> context = fss_tests_init(('/tmp/fss', '', 3))
>>> path, current_path, nb_tests = context
>>> path == '/tmp/fss' and nb_tests == 3 and current_path != ''
True
En effet, ici current_path dépend des traitements effectués dans la fonction fss_tests_init. Or, il se trouve que ces traitements sont dépendants d'appels précédents (n'ayant pas forcément eu lieu lors des appels successifs des tests, par exemple). Il n'est donc tout simplement pas possible d'indiquer une chaîne de caractères comme étant celle d'un répertoire attendu.

Le module doctest fournit des outils pour exécuter tous les doctests trouvés dans un module. Si vous écrivez un programme conséquent, vous pourrez utilement utiliser le script suivant (qui est basé sur un script original de Victor Stinner, merci à lui) qui exécutera tous les doctests des modules que vous lui indiquerez (en lieu et place de fss, cpu_stress, stress et stresssuite).

#!/usr/bin/env python
# -*- encoding: utf8 -*-
#
# testscases for the StressSuite tools !
#
# (C) Copyright 2009 Olivier Delhomme
# e-mail : olivier.delhomme@free.fr
#
# This program is free software; you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation; either version 2, or (at your option)
# any later version.
# [...]
# This file is heavyly based on test_doc.py that you will found in the
# hachoir project thanks to Victor Stinner
import os
import sys
import doctest
def importModule(name):
    mod = __import__(name)
    components = name.split('.')
    for comp in components[1:]:
        mod = getattr(mod, comp)
    return mod
#
def testModule(name):
    print('--- Test module "%s"' % name)
    module = importModule(name)
flags = doctest.REPORT_UDIFF
failure, nb_test = doctest.testmod(module, optionflags=flags)
    print('--- End of test for module "%s" (%d passed and %d failed)' % \
         (name, nb_test, failure))
    if failure:
        sys.exit(1)
#
def main():
    cwd = os.path.dirname(__file__)
    sys.path.append(cwd)
    # Test some functions/classes
    # Please add here modules to be tested
    testModule('fss')
    testModule('cpu_stress')
    testModule('stress')
    testModule('stresssuite')
#
if __name__ == "__main__":
main()
2.3 EN RÉSUMÉ
Un programme sans docstring ou sans doctest est un programme sans avenir. Pensez-y lorsque vous en écrivez un. La doc, la doc, la doc. Et les tests, les tests, les tests... ;-)

3. BONNES HABITUDES SYNTAXIQUES [PEP8]
Je vais ici tenter de donner quelques astuces afin de prendre de bonnes habitudes syntaxiques dès vos premiers programmes. La première remarque est plutôt d'ordre général car il s'agit d'avoir, dans un projet, une uniformité syntaxique. Si vous écrivez d'une certaine manière, conservez-la une fois pour toute. Si vous participez à un projet et que les habitudes syntaxiques du projet ne sont pas les vôtres, pliez-vous à celles du projet en gardant en tête que l'uniformité syntaxique améliore la lisibilité.

Respecter l'uniformité syntaxique vous contraint, par exemple, à écrire les conditions if sur plusieurs lignes. En effet, toutes les conditions d'un projet ne tiennent pas nécessairement sur une seule ligne...

Les règles sont celles du français écrit :

- Lorsque vous utilisez le caractère , pour séparer des valeurs dans un tuple, les arguments d'une fonction ou les éléments d'une liste, ne laissez pas d'espace avant et laissez une espace après le caractère.

- Avec les parenthèses, ne mettez pas d'espace après la parenthèse ouvrante, ni avant la parenthèse fermante.

- Utilisez des paragraphes pour aérer votre code et le rendre encore plus compréhensible.

Lorsque vous définissez une fonction ou lorsque vous appelez une fonction, ne mettez pas d'espace devant la parenthèse ouvrante.

Mettez une espace devant et derrière le signe = lorsqu'il s'agit d'une affectation. Ne mettez aucune espace lorsqu'il s'agit de paramètres optionnels à une fonction : resultat = factorielle(4, debug=True)

Utilisez la fonction print() plutôt que l'instruction, c'est une bonne pratique apparue dans les versions 2.x qui est obligatoire dans les versions 3.x ; autant prendre les devants !

Lorsque j'écris une classe, j'aime bien y écrire explicitement les attributs avec un commentaire associé dans le code. Idéalement, ce commentaire sera différent de ce que vous aurez pris soin d'écrire dans le docstring.

Personnellement, j'ai un mal fou avec les fonctions et les classes qui semblent ne pas se terminer. Pour m'éviter ce problème, je mets une ligne de commentaire à la fin de la fonction ou de la classe : # fin de la fonction super_bidule(). Ça m'aide bien aussi pour me repérer lorsque les classes ou les fonctions sont un peu trop grandes... D'ailleurs, à ce propos, ne faites pas comme moi, écrivez plutôt des fonctions courtes qui tiennent dans 20/25 lignes. La compréhension du programme n'en sera que facilitée.

Usez et abusez des docstrings et doctests, ce sont d'excellents mécanismes qui améliorent grandement la qualité globale d'un programme.

Enfin, n'oubliez pas ces deux recommandations :

- Ne dépassez pas les 80 caractères d'une ligne.

- Ne mettez pas d'espace avant le :, passez à la ligne directement.

CONCLUSION
Cet article n'est qu'une très petite introduction à Python. Vous trouverez de nombreux livres et sites web pour aller plus loin. Pour ma part, j'utilise le livre de Tarek ZIADÉ [ziade] et la documentation en ligne du site web officiel [web-python].

Vous verrez comme on s'habitue vite à la souplesse de Python et comme on retient vite sa syntaxe simplifiée. Si vous êtes comme moi, lorsque vous reprendrez de vieux scripts écrits en bash ou en perl pour les modifier, vous vous demanderez « comment ça s'écrit déjà ?? ».

Message personnel : maintenant Guillaume, tu n'as plus d'excuse ! Il ne te reste plus qu'à te mettre à psycopg (je te laisse deviner le genre de module dont il s'agit ;-) !!

Je remercie tous mes relecteurs, ma copine pour sa patience et tous les codeurs qui ont fait de Python ce qu'il est aujourd'hui : formidable !

RÉFÉRENCES
[pep8] http://www.python.org/dev/peps/pep-0008/

[geany] http://www.geany.org/

[contrôles] 
http://python-history.blogspot.com/2009/01/pythons-design-philosophy.html
http://mail.python.org/pipermail/python-ideas/2009-
February/002642.html
http://www.python.org/doc/faq/general/#id56

[ziade] ZIADE (Tarek), Programmation Python - conception et optimisation, éditions Eyrolles, avril 2009, ISBN : 2-212-12483-5, 547 pages.

[web-python] http://www.python.org/

[gnulinuxmag] GNU/Linux Magazine France hors-série, n°40 « Explorer les richesses du langage Python »

Tags : bash, diff, html, langages, python, sauvegarde, windows, zsh
