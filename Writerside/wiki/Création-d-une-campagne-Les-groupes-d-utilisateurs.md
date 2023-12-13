# Les groupes d&apos;utilisateurs

Maintenant que le profil d'envoie de mail as été correctement configuré, il va falloir créer des listes d'utilisateurs vers qui envoyer les mails de phishing.

Pour cela, et à l'aide du menu de gauche, naviguez vers "Users & Groups" puis sur "New Group".

<img src="group.PNG" alt="Configuration d'un groupe"/>

Pour ajouter des utilisateurs dans un groupe d'envoie, vous aurez deux solutions :

- Ecrire nom, prénom et adresse email à la main;
- Importer un fichier CSV;

<tabs>
    <tab title="CSV">
        Pour importer des utilisateurs avec un fichier CSV, il faudra que votre fichier ai la structure suivante :

<code-block>
            First Name,Last Name,Position,Email
</code-block>

Donc par exemple, je veux importer trois utilisateurs : Jean Bon, Chevalier DeGaulle et Jean-françois Foiros.
Dans ce cas présent, le fichier CSV aura le contenu suivant :

<code-block>
            First Name,Last Name,Position,Email
            Jean,Bon,Administrateur Système,jean.bon@lab.test
            Chevalier,DeGaulle,Directeur,chevalier.degaulle@lab.test
            Jean-François,Foiros,DRH, jean-françois.foiros@lab.test
</code-block>

Dés que le fichier CSV as été édité, vous pourrez l'importer en cliquant sur le bouton "Bulk Import Users". Vous remarquerez aussi qu'à droite du bouton en question, vous pourrez télécharger un template de fichier CSV.
Une fois le fichier CSV importé, vous pourrez observer les noms importés dans la liste.

<img src="csv_import.PNG" alt="Capture d'écran CSV"/>

</tab>
<tab title="A la main">

Pour importer un utilisateur à la main, vous aurez juste à remplir les champs "First Name", "Last Name", "Email", et "Position" puis cliquer sur le bouton "Add".

Cette méthode simpliste est très utile quand on ne veux envoyer le mail de phishing à une poigné de personne mais dés qu'il s'agit de beaucoup de personne en même temps (par exemple une trentaine), il serait préférable d'utiliser le fichier CSV.

<img src="import_hand.PNG" alt="Capture Ecran"/>

</tab>
</tabs>

> **Note :**
> 
> Le champ "position" ne sert principalement qu'à indiquer la position hierarchique de la personne (par exemple "Administrateur Système", "Directeur", etc...).
> 
{style="note"}

Une fois que les utilisateurs ont été importé dans la base de donnée, vous avez plus qu'à cliquer sur "Save Changes" pour valider la création/modification du groupe.
