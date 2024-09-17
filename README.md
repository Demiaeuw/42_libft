# 42 Libft

## Description

Libft est un projet de l'école 42 dont l'objectif est de recréer une bibliothèque standard en C. Cette bibliothèque contient un ensemble de fonctions essentielles qui permettent de manipuler des chaînes de caractères, de la mémoire, et des fichiers, ainsi que d'autres opérations de base utilisées fréquemment dans les programmes C.

Libft vous permettra de mieux comprendre le fonctionnement interne de certaines fonctions standard de C, telles que celles présentes dans <stdlib.h>, <string.h>, et d'autres.
Fonctionnalités

  Manipulation de chaînes de caractères : fonctions comme ft_strlen, ft_strcpy, ft_strdup, etc.
  Gestion de la mémoire : fonctions comme ft_memset, ft_memcpy, ft_bzero, etc.
  Fonctions d'entrées et sorties : ft_putchar, ft_putstr, ft_putnbr, etc.
  Listes chaînées : implémentation de fonctions pour gérer des listes chaînées.
  Manipulation d'éléments de tableaux et gestion dynamique de la mémoire.

## Installation

Pour utiliser Libft, suivez les étapes suivantes :

1. Clonez le dépôt :

```bash

git clone https://github.com/Demiaeuw/42_libft.git
```
2. Accédez au répertoire du projet :

```bash

cd 42_libft
```
3. Compilez la bibliothèque avec make :

```bash

make
```
4. Une fois compilée, la bibliothèque libft.a sera générée. Vous pouvez l'inclure dans vos projets en utilisant l'option -L et -l lors de la compilation de vos projets.

## Utilisation

### Inclure Libft dans un projet C

Après avoir compilé Libft, vous pouvez inclure cette bibliothèque dans vos projets. Assurez-vous d'inclure l'en-tête libft.h dans vos fichiers .c et d'ajouter la bibliothèque lors de la compilation.

Exemple de compilation :

```bash

gcc -Wall -Wextra -Werror main.c -L. -lft
```
  -L. : Spécifie le répertoire contenant la bibliothèque (libft.a).
  -lft : Lie le fichier binaire avec libft.a.

### Utilisation des fonctions

Voici un exemple d'utilisation de Libft dans un fichier source :

```c

#include "libft.h"

int	main(void)
{
	char	*str;

	str = ft_strdup("Bonjour 42 !");
	ft_putstr(str);
	free(str);
	return (0);
}
```
## Dépendances

Aucune dépendance externe n'est requise. Libft utilise uniquement les bibliothèques standard de C.

## Contributeurs

[Adrien Cabarbaye](https://github.com/Demiaeuw)

## Licence

Ce projet est sous la licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus d'informations.
