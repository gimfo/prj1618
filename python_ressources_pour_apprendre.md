ANNEXE. APPRENDRE PYTHON : DE DÉBUTANT À EXPERT
1. INTRODUCTION
Cette partie offre des suggestions pour apprendre Python soi-même et pour l'enseigner à des étudiants (certaines références peuvent aussi être utiles pour les programmeurs connaissant déjà Python.). Un très large travail pédagogique a déjà été réalisé sur ces sujets et il serait dommage de se priver des ressources proposées, d'autant plus qu'elles sont nombreuses à être accessible gratuitement sur internet. Il est aussi particulièrement aisé de trouver en ligne des informations à jour par rapport à la dernière version de Python. Cette partie est donc largement constituée de pointeurs, sélectionnés pour leur intérêt.

1.1 OBTENIR PYTHON

Python est installé en standard par la plupart des distributions Linux, et dans Mac OS X. Si nécessaire, il est possible d'obtenir une version adaptée à de nombreux systèmes d'exploitation via le site officiel (http://www.python.org/download/) — il existe même une version pour téléphone portable !

Que ce soit pour apprendre soi-même le langage ou pour l'enseigner, il est utile d'employer une version récente de Python : le langage évolue en fournissant des outils de plus en plus pratiques, tout en continuant d'observer un principe de simplicité très appréciable. Les adresses web indiquées ici ont donc été choisies de façon à fournir des informations les plus récentes possibles.

1.2 PYTHON INTERACTIF

Le shell Python, qui peut se lancer via la commande python, est une ressource pédagogique importante : il interprète les commandes Python entrées, permet de remonter dans l'historique de ces commandes ou d'y effectuer des recherches, etc. Une excellente alternative au shell standard est IPython (http://ipython.scipy.org/moin/), qui rend la vie du programmeur encore plus facile, avec en particulier la complétion des noms (de variable, de fonction, etc.) et un accès immédiat au débogueur standard de Python (pdb). Ces deux shells sont très pratiques pour effectuer des tests, même complexes, et il serait dommage de s'en priver.

1.3 ÉDITER LE CODE PYTHON

De nombreux éditeurs aident à écrire en Python, en fournissant au minimum une coloration syntaxique (où par exemple les mots-clés sont mis dans une couleur particulière) et parfois une aide à la complétion des noms de variable, etc. Sous Unix, on peut citer les deux célèbres éditeurs emacs et vim. Python vient en standard avec l'environnement de développement intégré IDLE (qui peut se lancer avec la commande idle). Komodo Edit, qui a l'avantage d'être gratuit et multiplateforme, est aussi un choix que l'on peut faire, parmi d'autres. Bref, les éditeurs facilitant l'écriture en Python ne manquent pas !

2. APPRENDRE SOI-MÊME PYTHON
2.1 PYTHON QUAND ON N'A JAMAIS PROGRAMMÉ

Il existe de nombreux textes d'enseignement de Python destinés aux débutants en programmation.

2.1.1 RESSOURCES INTERNET GRATUITES

Les ressources internet gratuites présentées ci-dessous permettent d'apprendre Python par soi-même. Elles sont ordonnées et commencent par la référence que je recommande le plus.

Il s'agit du livre Think Python: An Introduction to Software Design [Downey] ; il présente de nombreux exemples de bonnes pratiques et contient des exercices.

Une autre référence à considérer, qui couvre de nombreux sujets, est Programming for Non-Programmers: How to Write Your Own Software Using Python [Lott (a)]. Bien qu'il soit restreint actuellement à Python 2.4, il n'en offre pas moins une présentation intéressante du langage ; il contient lui aussi des exercices.

Un livre destiné plus particulièrement aux jeunes à partir de 8 ans est Snake Wrangling for Kids [Briggs] ; il peut être cependant intéressant à consulter, pour les programmeurs débutants. Il s'agit encore d'un livre qui contient des exercices.

On peut citer le cours de l'Institut Pasteur [Schuerer (a)], qui fournit une bonne introduction à Python plus particulièrement utile aux scientifiques. Il est fort complet, tout en étant toujours en train d'être étoffé. Il propose de nombreux exemples et, lui aussi, des exercices.

A Byte of Python [Swaroop], quant à lui, est un bon livre d'introduction qui peut s'avérer utile malgré son caractère légèrement aride (peu d'illustrations, quelques listes de fonctions plus utiles comme référence que comme introduction à la programmation). Il a été utilisé dans plusieurs universités, ainsi qu'à la NASA.

Enfin, le seul livre en français de cette liste s'intitule simplement Apprendre à programmer avec Python [Swinnen], que je mentionne pour ceux qui ne maîtrisent pas la langue de Shakespeare ; mais attention : Apprendre à programmer avec Python n'emploie pas toujours de bonnes pratiques de programmation en Python (par exemple avec les boucles p. 90, qui sont inutilement compliquées).

Des références additionnelles peuvent être obtenues sur le site officiel de Python (http://wiki.python.org/moin/BeginnersGuide/NonProgrammers).

2.1.2 LIVRES

Si l'usage d'un livre est préféré à celui des ressources en ligne (malgré le fait que les livres informatiques sont assez rapidement obsolètes), on pourra profiter de la publication prochaine de Think Python: An Introduction to Software Design [Downey], présenté ci-dessus.

On peut aussi mentionner un livre que je trouve moins enthousiasmant que le premier, qui est plus ancien (le shell Python utilisé est celui de Python 2.1), mais qui propose une approche plus progressive : Python Programming: An Introduction to Computer Science [Zelle (b)]. Il contient lui aussi des exercices.

Enfin le livre Python: How to Program [Deitel] peut être utile à considérer : il couvre certaines notions avancées de Python, contient des conseils de bonnes pratiques parfois très pertinents, et inclut des exercices. Cependant, ce livre utilise une version ancienne de Python et nombre des exemples fournis ne sont pas à suivre, tant ils manquent d'élégance et ne sont qu'une mauvaise traduction en Python de code C.

L'offre en librairie est donc moins intéressante que les ressources internet, que je recommande car elles sont plus accessible et plus souvent mises à jour.

2.2 PYTHON POUR LES PROGRAMMEURS

Pour ceux qui savent déjà programmer, apprendre les bases de Python devrait être rapide. Des ressources gratuites que je considère particulièrement utiles sont recensées ci-dessous, en commençant encore par ma première recommandation.

Une initiation efficace peut être trouvée sur http://hetland.org/writing/instant-python.html. Comme son titre l'indique (« Instant Python »), ce site présente très rapidement Python ; cela peut s'avérer extrêmement utile pour mieux comprendre d'autres introduction à Python. Learn Python in 10 minutes (http://www.poromenos.org/tutorials/python) est aussi à recommander.

Il est possible d'apprendre presque tout les concepts Python grâce au tutoriel officiel (http://docs.python.org/tut/), que je trouve excellent.

Le livre de S. Lott destiné aux débutants en programmation présenté ci-dessus [Lott (a)] est complété par un ouvrage pour programmeurs : Building Skills in Python: A Programmer's Introduction to Python [Lott (b)]. Ce livre a l'avantage d'être à la fois gratuit et récent. Il contient des exercices et des exemples de projets informatiques.

Il est important de mentionner aussi Dive into Python [Pilgrim], qui est très clair et progressif, et développe des sujets intéressants (comme les tests unitaires). Bien qu'il soit limité à Python 2.3, il reste une référence très utile.

Un autre cours de l'Institut Pasteur, cette fois-ci destiné aux programmeurs, vaut la peine d'être consulté [Schuerer (b)], même s'il s'adresse en particulier à des biologistes. Il est très concis et s'apparente parfois à un dictionnaire, ce qui peut être utile.

Cette liste des ressources sélectionnées est complétée par celle du site officiel (http://wiki.python.org/moin/BeginnersGuide/Programmers), qui en recense de nombreuses.

2.3 ÉVITER DES PROBLÈMES DE DÉMARRAGE

Malgré la simplicité de Python, il est naturel de tomber dans quelques pièges. Le site officiel regroupe des liens qui permettent de ne pas trop se faire surprendre lors de l'écriture des premiers programmes [PythonWarts] et de mettre ainsi initialement en œuvre ses connaissances de façon moins frustrante.

2.4 PRENDRE UN STYLE « PYTHONIQUE »

Pour bien commencer, il est important d'acquérir un bon style de programmation. Python encourage à suivre des conventions communes simples, qui permettent de rendre son propre style plus lisible et de pouvoir relire plus facilement celui des autres. Les deux guides officiels peuvent être trouvés sur http://www.python.org/doc/essays/styleguide/.

Quand on ne connaît que certains autres langages de programmation, il est utile de se débarrasser de certaines habitudes prises avec des langages de plus bas niveau (C, C++, Fortran ou même Java) ; ainsi, traduire littéralement en Python du code C résulte généralement en un code qui est inefficace (en plus d'être inélégant). Un exemple est la transformation de tous les éléments d'une liste avec le code C for (i=0; i < len_list1; i++) { list2[i] = f(list1[i]); }, qui s'écrit plus simplement list2 = map(f, list1) en Python.

Pour de nombreuses façons efficaces et lisibles de coder en Python, on pourra consulter Python Black Magic, qui contient en fait plus d'idiomes standards que de magie noire (http://blog.odonnell.nu/blackmagic/), Code Like a Pythonista [Goodger], et Python Tips, Tricks, and Hacks (http://www.siafoo.net/article/52).

2.5 PYTHON AU JOUR LE JOUR : AIDE STANDARD

Python offre en standard un système d'aide rapide, pratique et très complet, accessible par la commande pydoc. Elle peut être utilisée pour obtenir des informations sur toutes les facettes du langage et des modules (mots clés, classes objet standard, modules, etc.). Malgré la simplicité de Python, il peut arriver que l'on oublie certains détails sur l'usage de commandes moins souvent utilisées : pydoc est un précieux allié dans le travail de tous les jours et lorsque l'on apprend le langage.

Bien que la documentation accessible via pydoc soit déjà très fournie, il est utile de connaître l'astuce suivante : cette commande indique parfois une adresse web indiquée par « MODULE DOCS », qui pointe vers des informations souvent plus complètes (au moins sous Python 2.5).

2.6 UTILISER LE TRAVAIL DES AUTRES : MODULES ET RECETTES

Il arrive parfois que l'on ne voie pas immédiatement comment coder une tâche particulière ou qu'il semble trop long de le faire soi-même. Le programmeur n'est pas sans ressources, dans le monde de Python : des modules et des recettes sont disponibles pour l'aider.

2.6.1 LES MODULES

L'une des forces de Python réside dans son offre très large de modules, qui fournissent des outils puissants pour effectuer des tâches diverses (accès au web, graphiques, etc.). La liste des modules disponibles sur une machine peut être obtenue grâce à la commande pydoc -p 2000 (où 2000 est un port choisi assez arbitrairement), suivie d'une connexion à l'adresse http://localhost:2000.

2.6.2 LA BIBLIOTHÈQUE STANDARD

Il n'est pas aisé de trouver ce que l'on cherche à partir de la liste de modules donnée par pydoc, mais le tutoriel cité plus haut en offre un aperçu efficace (http://docs.python.org/tutorial/stdlib.html et http://docs.python.org/tutorial/stdlib2.html). Une liste complète des modules de la bibliothèque standard peut être obtenue sur le site officiel de Python, qui en présente une liste très bien organisée (http://docs.python.org/lib/lib.html pour Python 2.5, et http://docs.python.org/library/ pour Python 2.6).

Pour une approche pratique aux modules standards, on pourra consulter The Standard Python Library (http://effbot.org/librarybook/), excellente référence de Fredrik Lundh. Une autre très bonne source d'informations concrètes sur ces modules est le site Python Module of the Week, de Doug Hellmann (http://www.doughellmann.com/PyMOTW/). Ces deux sites permettent de comprendre rapidement quelles sont les principales fonctions de nombreux modules standard.

2.6.3 MODULES SUPPLÉMENTAIRES

Pour éviter de réinventer la roue, il ne faut pas hésiter à faire appel à l'un des nombreux modules non standard centralisés dans le Python Package Index (PyPI), aussi appelé la Cheese Shop (allusion aux Monty Python) [CheeseShop]. Le classement par catégories et la fonction de recherche permettent de localiser relativement aisément les modules potentiellement utiles à la tâches que l'on souhaite réaliser.

La plupart de ces modules s'installent aisément : soit automatiquement avec la commande easy_install (après avoir installé setuptools [http://pypi.python.org/pypi/setuptools/]), soit manuellement via un téléchargement, puis la commande python setup.py install (éventuellement précédée d'un sudo). La documentation de ces modules peut être obtenue via la commande pydoc que nous avons vue plus haut ou, mieux, via la page web du module.

2.6.4 DES RECETTES

Parfois, aucun module ne contient ce que l'on cherche à obtenir, bien que le code à produire ne semble pas évident ou serait un peu trop long à écrire soi-même. Des « recettes » sont heureusement disponibles sur internet, dans les Python Recipes (http://code.activestate.com/recipes/langs/python/). Ces recettes sont de plus souvent écrites dans un bon style Python dont il est utile de s'inspirer.

2.7 QUE FAIRE EN CAS DE PANNE

Grâce à la disponibilité de modules et de recettes, le programmeur Python peut se concentrer sur une écriture de code largement spécifique à son problème. Il peut alors lui arriver de bloquer parce qu'il ne paraît pas évident de coder simplement en Python la tâche à effectuer. Ou bien le résultat produit par le code ne correspond pas à ce que l'on attend. Dans ces cas-là, la Foire aux Questions (FAQ) officielle peut être salvatrice (http://www.python.org/doc/faq/). Les Infrequently Asked Questions de Peter Norvig sont aussi intéressantes (http://www.norvig.com/python-iaq.html). Poser une question dans le très actif groupe usenet comp.lang.python permettra souvent de la résoudre [Ertl].

2.8 DEVENIR UN PYTHONISTA CHEVRONNÉ

Même si Python est un langage simple à apprendre, il est inhabituel, au début, d'avoir en tête tous les outils offerts par le langage.

2.8.1 PYTHON RÉSUMÉ

Il existe des résumés de Python : ils sont très utiles pour vérifier que l'on connaît les principaux concepts du langage. À cet effet, je recommande chaudement la Python Quick Reference de Richard Gruet (http://rgruet.free.fr/), dont la version HTML est particulièrement lisible, ainsi que la Python Quick Reference Card de Laurent Pointal (http://www.limsi.fr/Individu/pointal/python/pqrc/).

2.8.2 INFORMATIONS OFFICIELLES PRÉCIEUSES

Le site officiel de Python contient essentiellement tout ce que l'on peut avoir besoin de connaître sur Python. Cependant, certaines informations d'usage assez courant s'y trouvent essaimées dans des documents différents.

Ainsi, l'importante référence qu'est le tutoriel permet d'apprendre des notions importantes comme la programmation objet (chapitre Classes [http://docs.python.org/tutorial/classes.html]), les exceptions (chapitre Exceptions [http://docs.python.org/tutorial/errors.html]) et les itérateurs et générateurs (section [http://docs.python.org/tutorial/classes.html#iterators]).

Une référence moins essentielle (du moins initialement) est la Python Library Reference ; contrairement à ce que son intitulé suggère, ce document ne contient pas seulement des informations sur les modules de la bibliothèque standard, mais aussi des informations sur des fonctions fondamentales du langage, qu'il est utile de maîtriser assez rapidement. On y trouvera ainsi les types standard dans le chapitre Built-in Types (http://docs.python.org/library/stdtypes.html) et en particulier les très utiles types fichier et itérateur. La liste importante des fonctions standards (any,…) figure dans un chapitre Built-in Functions (http://docs.python.org/library/functions.html). Les exceptions levées par Python, que l'on finit toujours par rencontrer, sont, quant à elles, décrites dans Built-in Exceptions (http://docs.python.org/library/exceptions.html).

Enfin, le Python Reference Manual, d'une lecture généralement moins nécessaire, contient malgré tout des notions avancées très pratiques sur les variables, les types, les classes et les méthodes spéciales (par exemple pour la surcharge d'opérateurs) : on les trouvera à l'adresse http://docs.python.org/reference/datamodel.html.

2.8.3 DES DÉTAILS UTILES

Enfin, quelques trucs et astuces rendent la vie du programmeur Python plus faciles : la liste Hidden features of Python du site stackoverflow en contient de nombreux (http://stackoverflow.com/questions/101268/hidden-features-of-python).

3. ENSEIGNER PYTHON
De nombreux cours sur Python sous forme de livre ou de site internet ont été présentés plus haut (sections « Python quand on n'a jamais programmé » et « Python pour les programmeurs ») : ils offrent une multitude de pistes pour enseigner Python et devraient pouvoir relativement aisément être adaptés à différents groupes d'étudiants. Les transparents Teaching Computer Science with Python (http://mcsp.wartburg.edu/zelle/python/sigcse-workshop/) devraient eux aussi pouvoir aider à créer un cours. Enfin, nombre des points suggérés ci-dessus pour l'apprentissage autodidacte de Python sont utiles pour l'enseignement du langage (éditeurs, commande pydoc,…).

3.1 PRATIQUER PYTHON

Pour programmer, il faut… programmer : la pratique doit nécessairement compléter un cours théorique. Organiser très tôt un travail sur machine est donc utile.

Si cela est possible et souhaité par l'enseignant, mettre à disposition des étudiants un shell Python (voir la section « Python interactif » ci-dessus) leur offre la possibilité de répondre rapidement par eux-mêmes aux questions qu'ils se posent (en effectuant des essais) ou encore de poser tôt des questions pertinentes qui ne viennent le plus souvent que par la pratique.

3.1.1 EXERCICES

Si l'on désire proposer des exercices (soit en cours, soit en séance de travaux pratiques), les ressources internet et les livres présentés dans la section « Apprendre soi-même Python » seront une source d'inspiration utile. Le livre Think Python [Downey], que je conseille de consulter en premier, contient des exercices et, contrairement à nombre d'autres sources, de nombreux corrigés. Les deux livres de S. Lott [Lott (a) et Lott (b)] sont une autre bonne source d'énoncés, sans corrigés. Le livre de H. Deitel, malgré les défauts mentionnés plus hauts, a l'avantage de proposer des questions de cours pertinentes et des énoncés intéressants, sans corrigés [Deitel]. Le livre de G. Swinnen est surtout intéressant pour les énoncés (les solutions sont loin d'être toujours des exemples à suivre) [Swinnen]. Enfin, le livre de J. Zelle offre des énoncés utilisables, mais sont là encore sans corrigés [Zelle].

3.1.2 PROJETS

Lancer les étudiants dans des projets en Python est un autre moyen de leur faire pratiquer le langage. Grâce à la grade variété des modules disponibles, de nombreux domaines d'application sont envisageables : les graphiques (à deux ou trois dimensions), les interfaces utilisateur, le réseau (web, e-mail, etc.), le calcul scientifique,…

Les chapitres de livre qui commentent la réalisation d'un programme concret fournissent de bons exemples de projets. Plusieurs références en contiennent [Downey, Lott, Swinnen]. De nombreuses autres idées de projets pour débutants se trouvent aussi à l'adresse http://www.daniweb.com/forums/thread32007.html.

3.2 THÉORIE : MORCEAUX CHOISIS

J'encourage les enseignants qui n'ont pas encore une longue pratique de Python, mais qui l'utilisent déjà un peu à le faire apprendre à des étudiants : le langage est suffisamment simple pour que cela ne pose pas de réel problème. Les divers points qui suivent ne sont pas forcément évidents pour un débutant, car ils viennent souvent avec l'expérience : je les souligne, car ils me semblent tout particulièrement importants à connaître et à enseigner, et ils pourraient passer inaperçus lors d'une première lecture de certaines des références citées plus haut.

3.2.1 ENSEIGNEMENT DU LANGAGE

Peu d'autres langages offrent comme Python un mécanisme de documentation intégré à la syntaxe. Je recommande chaudement d'écrire le plus souvent possible une chaîne de documentation pour chaque fichier Python et fonction qu'il contient. Les informations que l'on indique peuvent s'avérer extrêmement utiles non seulement quand on reprend un programme écrit longtemps auparavant ou par quelqu'un d'autre, mais aussi au moment de la conception du code : décrire la tâche qu'est censée effectuer une fonction fournit un cadre de travail des plus utiles.

Une notion importante à faire comprendre est qu'une variable référençant un objet se comporte comme une étiquette attachée à une boite. Ainsi, lorsque l'on écrit a = b = [0, 1, 2], ajouter un élément à la liste via a.append(3) fait que b renvoie [0, 1, 2, 3] : le contenu de l'objet a changé (il est « mutable ») et il est toujours accessible grâce aux deux « étiquettes » a et b.

Une question classique sur Python est celle du rôle des tuples : quelle est la différence entre le tuple (0, 1, 2) et la liste [0, 1, 2] ? Un point important dont il est utile de se souvenir pour écrire un code qui soit plus facilement lisible est que les éléments d'un tuple pourraient naturellement être nommés et forment un groupe de taille fixée. Par exemple, (0, 1, 2) pourrait représenter les coordonnées d'un point de l'espace (le premier élément est la coordonnée sur l'axe des abscisses, etc.) ; Python 2.6 introduit d'ailleurs les tuples à champs (named tuples), où chaque élément est associé à un nom (on pourrait choisir, ici, x, y, et z). Un tuple ne possède ainsi pas de méthode pour être agrandi : dans notre exemple, cela équivaudrait à ajouter une coordonnée supplémentaire à un point de l'espace ! En revanche, la liste [0, 1, 2] peut être agrandie, ordonnée, etc.

Comme nous l'avons vu plus haut, il est en fait rare d'avoir besoin des éléments d'une liste en même temps que leur index. Cela arrive cependant : il est alors utile de connaître la fonction enumerate(), qui renvoie successivement tous les couples (index, valeur) d'une liste. Dans la même veine, on peut obtenir facilement les paires de valeurs obtenues en parcourant en même temps deux listes de même taille grâce à la fonction « fermeture éclair » zip(). Garder ces deux points en mémoire permettra d'écrire dans un style plus clair et plus léger (sans inutile index de boucle).

3.2.2 ENSEIGNEMENT DES MODULES

Les modules regroupent des fonctionnalités qui sont spécifiques à différents domaines d'application et n'ont donc pas besoin de figurer dans le cœur du langage. Comme la plupart des programmes Python utilisent des modules, un cours sur Python se doit de les évoquer.

Pour que la notion de module soit plus concrète, je recommande d'apprendre aux étudiants à en créer un (ce qui revient essentiellement à introduire __name__ et '__main__'). Ensuite, je recommande de les encourager à écrire tous leurs programmes comme des modules : il n'en résultera qu'un meilleur découpage du code en fonctions et classes séparées, avec une utilisation correctement réduite de variables globales.

Lorsque l'on débute en Python, il n'est pas forcément évident de savoir quels sont les modules que l'on utilisera le plus. Dans les modules standards, il est utile de connaître sys (communication avec l'interpréteur Python), math (opérations mathématiques), os (accès au système d'exploitation), shutils (fonctions sur les fichiers), getopt (gestion des options de ligne de commande), re (expressions régulières), logging (gestion de messages de débogage, etc.), pprint (affichage plus lisible de variables), copy (copie de structures complexes), random (nombres aléatoires), glob (listage de noms de fichier), datetime (heure et date), urllib2 (interactions avec le web), tempfile (fichiers temporaires), codecs (gestion des encodages de texte),… On trouvera dans la bibliothèque standard nombre de modules pour travailler dans des domaines plus spécifiques : analyse de HTML ou de XML, e-mail, stockage d'objets Python dans des fichiers (pickle), bases de données, interface utilisateur, tests unitaires, etc. Certains modules non standards peuvent s'avérer extrêmement utiles. Les applications scientifiques emploieront utilement NumPy (tableaux), SciPy (calculs) et matplotlib (graphiques). Le stockage de données sous un format lisible (YAML) peut être effectué grâce à PyYAML. On peut aussi citer la Python Image Library, qui offre de nombreuses fonctions pour manipuler les images.

L'essentiel des modules peut être trouvé dans la bibliothèque standard et dans la Cheese Shop [CheeseShop] : les chances sont grandes pour que l'on y trouve ce que l'on cherche. Et si tel n'est pas le cas, Python rendra relativement facile l'écriture d'un nouveau module. Il ne restera plus qu'à en faire profiter les autres en le déposant dans la Cheese Shop !

BIBLIOGRAPHIE
Les pages web listées font référence à leur version au 15 septembre 2008.

[Benchmarks] « The Computer Language Benchmarks Game », http://shootout.alioth.debian.org/.

[Briggs] BRIGGS (J. R.), Snake wrangling for kids: learning to program with Python (version 0.7.2), http://www.briggs.net.nz/log/writing/snake-wrangling-for-kids/, 2007.

[CheeseShop] « Python Package Index: Browse », http://pypi.python.org/pypi?%3Aaction=browse, 2008.

[Coverity]Open source report: 2008, http://www.coverity.com/library/pdf/Coverity-Scan_Open_Source_Report_2008.pdf, coverity, 2008.

[Deitel] DEITEL (H. M.) et al. Python: How to Program, Prentice Hall, 2002.

[Dewar] DEWAR (R. B. K.) et SCHONBERG (E.), « Computer Science Education: Where Are the Software Engineers of Tomorrow? », in : CrossTalk, The Journal of Defense Software Engineering, pp. 28-30, jan. 2008. http://www.stsc.hill.af.mil/CrossTalk/2008/01/0801DewarSchonberg.html.

[Downey] DOWNEY (A. B.), Think Python: An Introduction to Software Design, http://www.greenteapress.com/thinkpython/thinkpython.html (version 1.1.17), 2008.

[Eckel] ECKEL (B.), « Strong Typing vs. Strong Testing », http://www.mindview.net/WebLog/log-0025, mai 2003.

[Elkner] ELKNER (J.) « Using Python in a High School Computer Science Program », http://www.python.org/workshops/2000-01/proceedings/papers/elkner/pyYHS.html, 2000.

[Ertl] ERTL (A.), « How popular are various programming languages? » (résultats de mars 2008), http://www.complang.tuwien.ac.at/anton/comp.lang-statistics/.

[Ferg] FERG (S.), « Python & Java: A Side-by-Side Comparison », http://www.ferg.org/projects/python_java_side-by-side.html, mai 2007.

[GitBenchmarks]http://git.or.cz/gitwiki/GitBenchmarks.

[Goodger] GOODGER (D.), « Code Like a Pythonista: Idiomatic Python », http://python.net/~goodger/projects/pycon/2007/idiomatic/presentation.html, 2007.

[Guo] GUO (P.), « Why Python is a great language for teaching beginners in introductory programming classes », http://www.stanford.edu/~pgbovine/python-teaching.htm, 2007.

[Halloway] HALLOWAY (S.), « Ending Legacy Code In Our Lifetime », http://blog.thinkrelevance.com/2008/4/1/ending-legacy-code-in-our-lifetime, avril 2008.

[Isaacson] ISAACSON (D.), « Python Tips, Tricks, and Hacks », http://www.siafoo.net/article/52, juillet 2008.

[Knuth] KNUTH (D.), « Structured Programming with go to Statements », in : ACM Computing Surveys, volume 6, numéro 4, p. 268, déc. 1974.

[Lott (a)] LOTT (S. F.), Programming for Non-Programmers: How to Write Your Own Software Using Python, http://homepage.mac.com/s_lott/books/nonprogrammer.html, 2007.

[Lott (b)] LOTT (S. F.), Building Skills in Python: A Programmer's Introduction to Python, http://homepage.mac.com/s_lott/books/python.html, 2008.

[Loui] LOUI (R. P.), « In Praise of Scripting: Real Programming Pragmatism », in : Computer, volume 41, numéro 7, pp. 22-26, juil. 2008. http://www.cse.wustl.edu/~loui/praiseieee.html.

[McConnell] MCCONNELL (S.), Code complete, deuxième édition, Microsoft Press, 2004.

[Miller] MILLER (P.), « Recursive Make Considered Harmful », http://miller.emu.id.au/pmiller/books/rmch/, 1997.

[NumPyPerf]http://www.scipy.org/PerformancePython.

[Ousterhout] OUSTERHOUT (J. K.), « Scripting: Higher Level Programming for the 21st Century », in : IEEE Computer, mars 1998. http://www.tcl.tk/doc/scripting.html.

[ParallelProcessing] « ParallelProcessing - PythonInfo Wiki », http://wiki.python.org/moin/ParallelProcessing, septembre 2008.

[Pilgrim] PILGRIM (M.), Dive into Python, http://diveintopython.org/index.html, 2004.

[Prechelt] PRECHELT (L.), « Are Scripting Languages Any Good? A Validation of Perl, Python, Rexx, and Tcl against C, C++, and Java », in : Advances in Computers, volume 58, 2002. http://page.mi.fu-berlin.de/~prechelt/Biblio/jccpprt2_advances2003.pdf.

[PythonSpeed] « PythonSpeed – PythonInfo Wiki », http://wiki.python.org/moin/PythonSpeed, 2007.

[PythonWarts] « PythonWarts – PythonInfo Wiki », http://wiki.python.org/moin/PythonWarts, février 2008.

[Reilly] REILLY (D.), « Inside Java: Java myths - fact versus fiction », http://www.javacoffeebreak.com/articles/inside_java/insidejava-may00.html, juin 2006.

[Schools] « SchoolsUsingPython – PythonInfo Wiki », http://wiki.python.org/moin/SchoolsUsingPython, juillet 2008.

[Schuerer (a)] SCHUERER (K.) et al., Introduction to Programming using Python, http://www.pasteur.fr/formation/infobio/python/, 2008.

[Schuerer (b)] SCHUERER (K.) et al., Python course in Bioinformatics, http://www.pasteur.fr/recherche/unites/sis/formation/python/, 2008.

[Scriptol] « List of Hello World Programs in 200 Programming Languages », www.scriptol.org-hello-world-programming-language.php.

[Shootout] « Ubuntu : Intel® Q6600® quad-core Computer Language Benchmarks Game » (résultats de septembre 2008), http://shootout.alioth.debian.org/u32q/benchmark.php?test=all&lang=python&lang2=javaxint.

[SourceForge] « SourceForge.net: Software Map » (résultats de septembre 2008), http://sourceforge.net/softwaremap/trove_list.php?form_cat=178.

[Swaroop] SWAROOP (C. H.), A Byte of Python (version 1.20), http://www.swaroopch.com/notes/Python, 2008.

[Swinnen] SWINNEN (G.), Apprendre à programmer avec Python, http://www.cifen.ulg.ac.be/inforef/swi/python.htm, 2005.

[Tiobe] « TIOBE Programming Community Index » (résultats de septembre 2008), http://www.tiobe.com/index.php/content/paperinfo/tpci/index.html.

[van Rossum] VAN ROSSUM (G.), Computer Programming for Everybody (Revised Proposal), CNRI Proposal #90120-1a, 1999. http://www.python.org/doc/essays/cp4e.html.

[Wikipedia:comparison] « Comparison of programming languages », http://en.wikipedia.org/wiki/Comparison_of_programming_languages#Expressiveness.

[Wikipedia:configure] « Configure script (computing) », http://en.wikipedia.org/wiki/Configure_script.

[Wikipedia:memory] « Working memory », http://en.wikipedia.org/wiki/Working_memory#Working_memory_capacity.

[Zelle (a)] ZELLE (J. M.), « Python as a First Language », http://mcsp.wartburg.edu/zelle/python/python-first.html, 1999.

[Zelle (b)] ZELLE (J. M.), Python Programming: An Introduction to Computer Science, Franklin Beedle & Associates, 2004.

Tags : blender, cache, debian, débogage, diff, fedora, html, https, inkscape, javascript, langages, nombres aléatoires, paradigme, php, python, scilab, sip, stockage, subversion, typage, unity, windows
