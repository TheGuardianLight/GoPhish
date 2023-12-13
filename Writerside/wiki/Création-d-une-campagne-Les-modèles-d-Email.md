# Les modèles d&apos;Email

La prochaine étape est de créer un modèle d'Email qui sera envoyé aux cibles de la campagne de Phishing.

Ces modèles vont être ce qui va permettre aux attaquant de tromper les utilisateurs et donc de pouvoir comettre leurs attaques.

Pour en créer une avec GoPhish, naviguez vers "Email Templates" puis "New Template".

<img src="mail_template_vierge.PNG" alt="Capture d'écran template mail"/>

Vous devrez nommer votre modèle en premier lieu dans le champ "Name" sans quoi vous risquez de ne pas retrouver votre template parmis d'autres.

Ensuite viens le champ "Envelope Sender". Dans ce champ vous pouvez mettre un email qui sera affiché dans la plupart des clients web. Vous pouvez le laisser vide pour que l'affichage par défaut qui est l'Email d'envoie que vous avez configuré dans la partie SMTP.

Pour créer un modèle de mail, vous aurez deux moyen. Le premier est de créer le mail en texte brut ou en HTMl, ou alors de l'importer grâce au bouton "Import Mail".

<tabs>
<tab title="Import Mail">

Dans ce premier moyen, la méthode est relativement simple puisqu'il s'agit de copier le code source du mail (qui est écrit en HTML) et de le coller dans le champ prévu à cet effet :

<img src="import_mail.PNG" alt="Capture d'écran import code source mail"/>

Dans notre exemple, nous allons copier et coller le code source d'un email de récupération de Microsoft.

Une fois le code source indiqué, il sera automatiquement affiché avec le bon formatage dans le champ d'édition Text/HTML en dessous, ce qui vous permettra de le modifier par la suite.

<img src="html_filled_import.PNG" alt="Capture d'exemple d'import de mail"/>

> **Information :**
> 
> Le mail, provenant d'un mail de récupération d'un de mes compte personnel, le code ainsi que les indices sur mon adresse mail personnel ont été caché et remplacé par des "x".
> 
{style="note"}

Maintenant qu'on as importé un mail, nous pouvons par la suite le modifier pour le rendre utilisable avec GoPhish.

Nous pouvons par exemple remplacer lal igne "Voici votre code" par "Réinitialisez votre mot de passe" puis en remplacant "Utilisez ce code" par "ce lien".

Nous pouvons également remplacer l'adresse mail mentionné par celle qui sera indiqué dans les listes d'envoie sur GoPhish. Pour cela, on peut utiliser la variable `{{.Email}}`.

Avec cela, notre modèle d'Email ressemblera à ceci :

<img src="mail_filled_import_modified_1.PNG" alt="capture"/>

Cependant, c'est bien beau de demander de cliquer sur un lien. Encore faut-il faire en sorte à ce que ce soit cliquable. Il faut donc ajouter un lien hyper texte sur "ici".

Pour ajouter un lien hypertexte, sélectionner les mots que vous souhaitez transformer en lien hypertexte puis cliquez sur le logo
<img src="logo_hypertexte.PNG" alt="Logo hypertexte"/>

<img src="hypertexte.PNG" alt="interface hypertexte"/>

Dans l'interface qui s'ouvre, vous pourrez configurer dans "Display Text" le texte qui va s'afficher, le protocole si c'est du http ou du https puis l'url vers lequel on sera redirigé en cliquant sur le lien.

Dans le champ "URL" nous allons indiquer la variable {{.URL}} qui est la variable dans lequel sera stocké l'URL phishé, donc l'URL qui permettra à la cible d'aller sur le serveur de phishing.

</tab>
<tab title="Text/HTML">

</tab>
</tabs>