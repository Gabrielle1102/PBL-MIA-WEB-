# 📒 Mon carnet de bord

**Nom :** BARBIER 

**Prénom :** Gabrielle 

**Adresse de mon site :** (https://gabrielle1102.pythonanywhere.com/)

> Modifiez ce fichier directement sur GitHub (icône crayon ✏️) pour répondre aux questions de chaque exercice.
> Écrivez avec vos propres mots : une réponse courte et juste vaut mieux qu'un long copier-coller ! 🙂

---

## 🟢 Exercice 1 — Mon premier déploiement

1. Où se trouve physiquement le code qui fabrique votre page : sur votre ordinateur, sur GitHub ou sur PythonAnywhere ?

   > _Ma réponse :Le code se trouve sur github 

2. Pourquoi votre voisin(e) peut-il voir votre site, alors que vous n'avez rien installé sur son ordinateur ?

   > _Ma réponse : Mon voisin peut voir mon code car il est mis en ligne sur pythonanywhere.

---

## 🟢 Exercice 2 — Les URL et les routes

1. Dans l'URL `https://www.google.com/maps`, quel est le nom de domaine ? Quel est le chemin ?

   > _Ma réponse :Nom de domaine : www.google.com       Chemin : /maps

2. Que veut dire le message *Not Found* ? Qui l'a envoyé : votre navigateur ou le serveur ?

   > _Ma réponse : le serveur qui envoie ce message au navigateur car il ne trouve pas de page associée

3. Que se passe-t-il si deux fonctions portent le même nom dans `flask_app.py` ? (Indice : essayez, puis lisez l'Error log.)

   > _Ma réponse : Si deux fonctions portent le même nom dans flask_app.py Flask peut afficher une erreur au lancement de l’application car les fonctions ont le même nom. Il faut donc leur donner des noms différents 

---

## 🔵 Exercice 3 — Le langage HTML

1. Quelle est la différence entre ce que le serveur **envoie** et ce que le navigateur **affiche** ?

   > _Ma réponse : La différence, c’est que le serveur envoie le code HTML au navigateur, mais le navigateur interprète ce code pour afficher une page web avec du texte, des titres et des images.

2. À quoi servent les balises `<h1>`, `<p>`, `<ul>` et `<li>` ?

   > _Ma réponse :  Les balises <h1>, <p>, <ul> et <li> servent à organiser le contenu d’une page web. <h1> sert à faire un titre principal, <p> à écrire un paragraphe, <ul> à créer une liste à puces et <li> à ajouter un élément dans cette liste.

3. Pourquoi l'image s'affiche-t-elle alors qu'elle n'est pas sur votre serveur ?

   > _Ma réponse : L’image s’affiche même si elle n’est pas sur notre serveur parce qu’elle est hébergée sur un autre serveur. Le navigateur va chercher l’image à l’adresse indiquée dans la balise HTML et l’affiche sur la page.

---

## 🔵 Exercice 4 — Les templates

1. Pourquoi est-ce une bonne idée de séparer le code Python et le HTML ? (Pensez à une équipe avec un développeur et un graphiste.)

   > _Ma réponse : 1. Ça permet au développeur de gérer Python et au graphiste de modifier le HTML sans se gêner.

2. Les `{{ prenom }}` sont-ils remplacés par le serveur ou par le navigateur ? Comment l'avez-vous vérifié ?

   > _Ma réponse : ls sont remplacés par le serveur grâce à Flask. Je l’ai vérifié en regardant le code source de la page.

---

## 🔵 Exercice 5 — Le CSS et les liens

1. Quelle est la différence de rôle entre le HTML et le CSS ?

   > _Ma réponse : Le nom du paramètre est search_query et sa valeur est chat.

2. Pour afficher votre page `/presentation`, combien de fichiers le navigateur doit-il télécharger ? (Vous pourrez le vérifier à l'exercice suivant !)

   > _Ma réponse :Le serveur plante avec a=bonjour car il essaie sûrement de faire un calcul avec une valeur qui est du texte. Il faudrait vérifier la valeur reçue avant de l'utiliser.

3. Pourquoi faut-il parfois faire **Ctrl + F5** pour voir les changements de CSS ?

   > _Ma réponse : C'est dangereux car l'utilisateur pourrait envoyer du code malveillant qui serait exécuté sur la page. Il faut donc sécuriser les données avant de les afficher.

---

## 🟣 Exercice 6 — Espionner le navigateur

1. Que signifie HTTP ? Qui envoie la **requête** et qui envoie la **réponse** ?

   > _Ma réponse : HTTP signifie HyperText Transfer Protocol. Le navigateur envoie la requête et le serveur envoie la réponse.

2. Combien de requêtes votre page `/presentation` a-t-elle déclenchées ? Lesquelles ?

   > _Ma réponse : Ma page /presentation a déclenché 2 requêtes : une pour le fichier HTML et une pour l'image.

3. Que signifie le code `200` ? Et le code `404` de la favicon ?

   > _Ma réponse :Le code 200 signifie que la requête a réussi. Le code 404 signifie que la ressource demandée, ici la favicon, n'a pas été trouvée.
   
4. Pourquoi les modifications faites dans l'onglet Éléments ne sont-elles pas visibles par les autres visiteurs ?

   > _Ma réponse : Les modifications dans l'onglet Éléments sont seulement visibles sur mon navigateur et ne modifient pas les fichiers du serveur.

---

## 🟣 Exercice 7 — Envoyer des informations dans l'URL

1. Dans l'URL `https://www.youtube.com/results?search_query=chat`, quel est le nom du paramètre ? Quelle est sa valeur ?

   > _Ma réponse :Le nom du paramètre est search_query et sa valeur est chat
   
2. Pourquoi le serveur plante-t-il avec `a=bonjour` ? Que faudrait-il faire pour l'éviter ?

   > _Ma réponse :le serveur plante car il essaie de faire un calcul avec du texte. Il faut vérifier les données reçues avant de les utiliser.

3. Pourquoi est-il dangereux d'afficher **tel quel** ce que l'utilisateur envoie ?

   > _Ma réponse : C'est dangereux car l'utilisateur peut envoyer du code malveillant qui pourrait être exécuté sur la page.

---

## 🟣 Exercice 8 — Les formulaires

1. Quelle est la différence visible entre GET et POST ?

   > _Ma réponse : Avec GET, les données apparaissent dans l’URL. Avec POST, elles sont envoyées dans le corps de la requête.

2. Pour un formulaire de **recherche**, quelle méthode choisiriez-vous ? Et pour un formulaire de **connexion avec mot de passe** ? Pourquoi ?

   > _Ma réponse : Pour une recherche, je choisirais GET car on voit les mots recherchés dans l’URL. Pour une connexion, je choisirais POST car le mot de passe n’apparaît pas dans l’URL.

3. Les données envoyées en POST sont-elles vraiment « secrètes » ? (Pensez à ce que vous avez vu dans l'onglet Réseau.)

   > _Ma réponse : Non, les données envoyées en POST ne sont pas vraiment secrètes, car on peut les voir dans l’onglet Réseau du navigateur. Il faut utiliser HTTPS pour sécuriser les échanges.

---

## 🔴 Exercice 9 — Les codes de statut

1. Quelle est la différence entre une erreur `4xx` et une erreur `5xx` ? Qui est « fautif » dans chaque cas ?

   > _Ma réponse : Une erreur 4xx vient généralement d'un problème dans la requête du client. Une erreur 5xx vient d'un problème du serveur.

2. Comment fonctionne une redirection ? Qui fait la deuxième requête : le serveur ou le navigateur ?

   > _Ma réponse : Le serveur envoie une réponse qui indique une nouvelle adresse, puis le navigateur fait la deuxième requête.

3. Donnez un exemple de situation où un vrai site utilise une redirection.

   > _Ma réponse :Par exemple, quand on se connecte à un site, il peut nous rediriger vers notre page de profil.

   
---

## 🔴 Exercice 10 — Ce que le serveur sait de vous

1. Citez trois informations que le serveur connaît sur vous, sans que vous ayez rien rempli.

   > _Ma réponse : Le serveur connaît mon adresse IP, mon navigateur et mon système d’exploitation.

2. À quoi peut servir l'en-tête `Accept-Language` pour un site comme Wikipédia ?

   > _Ma réponse : Accept-Language permet à Wikipédia de choisir la langue qui correspond à celle de mon navigateur.

3. Dans l'Access log, retrouvez une requête qui a reçu un code `404`. Quelle page était demandée ?

   > _Ma réponse :_ La page demandée était une page qui n’existait pas sur le serveur, par exemple /favicon.ico.

4. Après cet exercice, que pensez-vous de la notion de « navigation anonyme » ?

   > _Ma réponse : Je pense que la navigation anonyme est difficile, car les sites récupèrent déjà plusieurs informations sur nous sans qu’on ait besoin de remplir quoi que ce soit.

---

## 🔴 Exercice 11 — Le Web des machines : API et JSON

1. Quelle est la différence entre une page HTML et une réponse JSON ? À qui chacune est-elle destinée ?

   > _Ma réponse :_ 

2. Dans la page `/horloge`, quel code s'exécute sur le **serveur** et quel code s'exécute dans le **navigateur** ?

   > _Ma réponse :_ 

3. Citez une application de votre téléphone qui, selon vous, utilise une API. Quelles données échange-t-elle ?

   > _Ma réponse :_ 

---

## 🏁 Pour conclure

En quelques phrases, expliquez à un ami ce qui se passe entre le moment où il tape une adresse dans son navigateur et celui où la page s'affiche :

> _Ma réponse :_ 
