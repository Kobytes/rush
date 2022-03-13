Rush | V.2 - All Bonus ✅
===================== 
Sujet commun
-------------------
Écrire la fonction rush prenant en paramètre deux variables de type entier nommées respectivement x et y. La fonction rush devra afficher à l’écran un rectangle de x caractères de largeur, et y caractères de hauteur.

Exemples
-------------------

#### rush(5, 5) :
```
o---o
|   |
|   |
|   |
o---o
```

#### rush(10, 5)
```
o--------o
|        |
|        |
|        |
o--------o
```

#### rush(20, 1)
```
o------------------o
```
------
Pseudo-Code
-------------------
<dl>
  <dt>Prototypage de ft_putchar</dt>
  <dd>Le prototypage est nécessaire car la Norminette interdit d'include des fichiers au format .c . Ainsi a la compilation avec <b>cc</b>, le compilateur ira chercher les fonctions de ft_putchar.</dd>

  <dt>Instanciation de la fonction ft_write</dt>
  <dd>ft_write va servir à l'application de la partie <b>logique</b> mais aussi de <b>l'affichage</b>.</dd>
</dl>

<dl>
  <dt>Affichage de V1</dt>
  <dd>V1, V2 et V3 servent a stocker les signes permettant la mise en forme du résultat. (Cf. tableau ⬇).</dd>
</dl>

#### Ici pour le rush 01, les symboles seront :

| V1 | V2 | V3 |
|--|--|--|
| / | * | \ |

| V1 | V2 | V3 |
|--|--|--|
| * | *vide* | * |

| V1 | V2 | V3 |
|--|--|--|
| \ | * | / |

------
<dl>
  <dt>w_i = 0;</dt>
  <dd>On démarre w_i a 0, il va nous servir de compteur.</dd>
  
  <dt>while (w_i++ < x - 2)</dt>
  <dd>TANT QUE la valeur de w_i plus 1 est inférieure à <b>x</b> ( <i>qui peut stocker la valeur de x ou y </i>) moins le signe de départ et de fin (-2). </dd>
</dl>

<dl>
  <dt>ft_putchar(v2);</dt>
  <dd>Si c'est le cas, alors on affiche le deuxième caractère (ici *).</dd>

  <dt>if (x > 1)</dt>
  <dd>On vérifie si x est supérieure à 1, cela permet de savoir si on se situe a la fin de la ligne.</dd>
</dl>

<dl>
  <dt>ft_putchar(v3);</dt>
  <dd>Si c'est le cas, alors on affiche le dernier caractère (ici \).</dd>

  <dt>ft_putchar('\n');</dt>
  <dd>Après avoir print la dernière valeur, on veut faire un retour a la ligne pour continuer ou simplement pour arrêter si il n'y a pas de nouvelle ligne a éxécuter.</dd>
</dl>

------

Pour la fonction rush
-------------------

<dl>
  <dt>int i;</dt>
  <dd>On instancie i, il va nous servir de compteur.</dd>
  
  <dt>if (x > 0 && y > 0)</dt>
  <dd>Ici, on vérifie <b>LE PLUS IMPORTANT !</b> C'est a dire qu'on verifie si l'utilisateur n'est pas nulle</dd>
</dl>
