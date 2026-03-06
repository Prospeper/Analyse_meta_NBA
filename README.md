# nba_winning_team_clustering
Analyse et clustering des joueurs NBA 2010-2025 pour créer une équipe type gagnante
On cherche dans un premier temps à identifier la meta de la NBA par saison en fonction du profil des joueurs par équipe. 
Document à lire en premier: "CHOIX_STATS"
Pour cela on a dans un premier temps extrait et nettoyer un dataset contenant les statistiques de tous les joueurs ayant évolué en NBA au cours des 15 dernières années.
Le dataframe comporte les statistiques suivantes:
Season: année de la saison
player: Nom du joueur
player_id: identifiant unique de chaque joueur(clé primaire) 
age: age du joueur au moment de la saison
team: abbréviation de l'équipe dans laquelle il joue
pos: position du joueur
g: nombre de matchs joués
gs: nombre de matchs dans lequel il fait parti du starting five
mp: minutes jouées
per: player efficiency rating
ts_percent: true shoot %
x3p_ar: nombre de tirs à 3 points pris par rapport au nombre de tirs
f_tr: free throw
orb_percent: pourcentage de rebond offensif
drb_percent: pourcentage de rebond deffensif 
trb_percent: pourcentage de rebonds
ast_percent: pourcentage d'assist
stl_percent: pourcentage de steal
blk_percent: pourcentage de blocks
tov_percent: pourcentage de turnover
usg_percent: pourcentage d'utilisation
ows: offensive winshare
dws: defensive winshare
ws:winshare
ws_48: winshare par 48 minutes 
obpm: offensive box plus minus
dbpm: defensive box plus minus
vorp: value over replacement

Le premier notebook cherche a déterminer les statistiques les plus pertinentes à utiliser par poste . Pour cela il faut que la statistique soit discriminante afin de pouvoir identifier des types de joueurs aux caractéristiques différentes. 

Ensuite il faut lire les 5 documents "nba_clustering_poste":
chaque document analyse les différents types de joueurs par poste , ainsi que l'évolution de la composition de la ligue par type au cours des 15 dernières années. 

Enfin le dernier document de l'analyse de meta , il s'agit d'analyser l'évolution de la meta de la ligue afin de déterminer quel type de composition d'équipe permet de performer en fonction de la composition de la ligue par saison. 
Bonne lecture! 