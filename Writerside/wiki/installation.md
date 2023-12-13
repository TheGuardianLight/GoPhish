# Installation

Pour débuter l’installation du script, voici les instructions à suivre :

>
> Vous devrez impérativement lancer le script avec les permissions d'administrataurs !
>
{style="warning"}

1. Effectuez un clone de ce dépôt en utilisant la commande :
    ```Bash
    git clone https://TheGuardianLight/GoPhish
    ```
Vous pouvez le faire dans n’importe quel répertoire de travail (par exemple, le répertoire root).

2. Après avoir cloné le dépôt, naviguez jusqu’au dossier du dépôt avec la commande :
    ```Bash
    cd GoPhish
    ```
3. Ajustez les permissions du script pour qu’il puisse être exécuté en utilisant la commande :
    ```Bash
    chmod +x gophish.bash
    ```
4. Suivez les directives fournies par le script et répondez aux questions qui vous seront posées.

> **Pour information :**
>
> Lorsque le script aura achevé l’installation et démarré le logiciel, il affichera dans le terminal l’**identifiant administrateur** par défaut ainsi que **son mot de passe temporaire**.
> 
> <img src="capture_gophish_mdp.png" alt="Capture d'écran mot de passe par défaut GoPhish"/>
> 
> Vous serez invité à modifier ce mot de passe lors de votre première connexion.

{style="note"}

5. Une fois le mot de passe administrateur modifié, utilisez `ctrl + c` pour fermer GoPhish dans le terminal. Cela permettra au script de finaliser l’installation.
6. Lorsque l’installation sera complète, vous pourrez démarrer GoPhish avec la commande :
    ```Bash
    systemctl start gophish
    ```

<seealso>
    <category ref="doc_go">
        <a href="https://getgophish.com/documentation/">Documentation de GoPhish</a>
    </category>
</seealso>