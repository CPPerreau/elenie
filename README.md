# elenie

meteoflow webapp to show migrations flows at Dunkirk, mid August 2022
Deployed on http://meteoflow.plumegeo.fr

## Crédits
- Authors of this project are **Elenie Sarciat** (elenie.sarciat@ulb.be) and **Christine Plumejeaud-Perreau** (christine.perreau@univ-poitiers.fr), UMR 7301 Migrinter, Poitiers, France
- Most of the data have been collected by Elenie Sarciat during the 2022 summer at Dunkerque
- A thank-you to the three students of Master SPE M2 at La Rochelle who collaborated during November 2023 on this project : 
                - Md Saiful Islam, M2 GPL - geophysique 
                - Hannah Metaireau, M2 GEEL - biologie 
                - Camille Saint-Picq, M2 GEEL - biologie 
- Data under **Licence CC4.0 BY-NC-SA**

## Lancer l'application

Elle marche avec python 3.10.6 au moins
1. créer et configurer l'environnement virtuel
  
  cd ~/elenie
  virtualenv venv -p /home/plumegeo/python/python310/bin/python3.10
  - entrer
  source venv/bin/activate
  - installer des packages
  pip install -r requirements.txt
  pip install rtree --upgrade
  pip install openpyxl
  - sortir : ~/elenie/deactivate
  
2. installer dans un environnement virtuel

Ajout du path python dans le programme elenie.py
```py
if platform == "linux" or platform == "linux2":
    # linux
    sys.path.append('/home/plumegeo/elenie/venv/lib/python3.10/site-packages')
```

3. lancer le programme dans l'environnement virtuel
   
cd ~/elenie
source venv/bin/activate
python3 elenie.py

5. lancer hors venv
/home/plumegeo/python/python310/bin/python3.10 elenie.py
