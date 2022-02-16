# Le projet :  créer une application  permettant de mettre en vente des objets
Ce projet à pour but  de créer une application NodeJS, Express et MongoDB.

## Comment participer au projet ?

1. Cloner git

          git clone https://github.com/MaryamVerdon/APIRESTful.git
    
2. En ligne de commande, se placer dans le répertoire "frontend"

         cd frontend
         
         npm install (installer les dépendances)
         
         npm run start

3. Se placer dans le répertoire "backend"  

         cd backend
         npm install
         nodemon server (lancer le serveur)
  
4. Configurer la BDD - MongoDB Atlas
    - Se rendre sur : https://www.mongodb.com/try?initial=true#community et se connecter/s'inscrire.
    - Sur MongoDB Atlas, se créer un cluster et le configurer : 
    
       -Dans le menu sur le côté, cliquer sur "Database Access" puis créer un utilisateur avec les droits écriture/lecture.
       
       -Dans le menu, cliquer sur "Network Access", autorisez toutes les adresses IP ou seulement la votre.
          
5. Connexion de l'API au cluster MongoDB

        cd backend
        npm install mongoose
        
    - ouvrir le fichier app.js et modifier la ligne suivante : 
     mongoose.connect('mongodb+srv://<username>:<password>@cluster0.orpsb.mongodb.net/myFirstDatabase?retryWrites=true&w=majority' 
    (ligne a récupérer sur MongoDB dans votre cluster sur le bouton "Connect" puis "Connect your application").
  
