Faire une todolist Symonfy

Je dois pouvoir :
* Je peux ajouter une tâche à faire
* Je peux prioriser une tâche
* Je peux définir une tâche comme faite
* Je peux voir toutes les tâches, faites ou pas
* Je peux filtrer la liste de tâches pour ne voir que les tâches faites
* Je peux filtrer la liste de tâches pour ne voir que les tâches à faire
* Je peux filtrer la liste de tâches pour voir toutes les tâches
* Je peux Associer une tâche à un utilisateur
* Je peux Supprimer une tâche
* Je peux Rajouter des utilisateurs
* Je peux Supprimer des utilisateurs
* Un utilisateur a juste un pseodo et un id



Pour cela il faut :

* Installer un Symfony 3.4
* Enregistrer les tâches dans la session par exemple :

    -> Enregistrement dans la sessions : $this->get('session')->set('tasks', [new Task(1, new User('simon'))]);
    
    -> Récupérer dans la session dump($this->get('session')->get('tasks'));die;

* Il ne faut pas utiliser une base de donnée où doctrine pour ce projet et pas de formulaire symfony.

N'oubliez pas de découper l'application suivant le modèle MVC et avec des classes :) .
