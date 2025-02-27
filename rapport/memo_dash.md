# Application dash
Dash est une librairie python qui permet de creer facilement une application web fonctionnel ,moderne, interactive.
### Avantages de Dash
- Dash est open source et donc libre d'utilisatation contrairement au autres logiciel de dashboarding comme Tableau et Power BI
- Dash utilise Javascript pour produire des choses super pour l'utilisateur bien qu'on ecrit en python
- Il y a peu de code pour obtenir une application web contrairement a des frameworks comme Django

### Relation entre plotly et dash
Ces deux librairies ont ete creer par la meme entreprise. Donc c'est tout naturel qu'ils fonctionnent ensemble.Une application dash peut inclure n'importe quelle graphique construit avec plotly.

### prerequis: dash et plotly installer


### Creation de l'application dash 

Pour commencer on creer un fichier `script.py`, (generalement `app.py`)ensuite insertion du code: 
- De la librairie `dash` importer des modules et objets necessaires pour les blocks a affichees dans l'applications: Exemple:`from dash import Dash, dcc`
- Creer l'application par l'instantiation de l'objet Dash dans le nom de variable de l'application que vous aurez choisit (generalement `app`): `app=Dash() `
- appeler la methode .layout() sur l'application pour afficher au moins un graphique plotly deja concu: app.layout(dcc.Graph(id='id-dugraph-Choisit' , figure=nom_du_graph))
- ecrire le code suivant pour le lancement de l'application:``if __name__ =='__main__':
                                                                 app.run(debug= True, port=8050)```


- lancement de l'application dans le terminal avec la commande: `python chemin_vers_le_script\app.py`

Les applications Dash sont composées de deux parties. La première partie est la "mise en page", qui décrit à quoi ressemble l’application. La deuxième partie décrit l’interactivité de l’application.



