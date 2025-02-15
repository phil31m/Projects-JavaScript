## Projet 1 : Quiz Generator

1. Fonctionnalités
 - Configuration personnalisée du quiz (nombre de questions, catégorie, difficulté)
 - Système de score en temps réel
 - Chronomètre de 30s par question
 - Affichage dynamique des questions avec mélange des réponses
 - Feedback visuel pour les bonnes/mauvaises réponses

2. Explication du code :
   # HTML :
     - Section `config-box` : Contrôles de configuration
     - Section `quiz` : Panneau de questions masqué initialement
     - Éléments fixes : Score (en haut à droite) et timer (en haut à gauche)

   # CSS :
     - `.option` : Style des réponses avec effets au survol
     - `.score`/`.timer` : Positionnement fixe et styles colorés
     - `transition: background-color 0.3s` : Animation fluide des réponses

   # JavaScript Principales Fonctions:
     - `loadCategories()` : Récupère les catégories depuis l'API
     - `generateQuiz()` : Construit l'URL API et charge les questions
     - `showQuestion()` : Affiche une question avec timer
     - `shuffleAnswers()` : Mélange les réponses aléatoirement
     - `handleAnswer()` : Gère la sélection de réponse et le score




## Projet 2 : Todo List

1. Fonctionnalités
 - Ajout/suppression de tâches
 - Recherche en temps réel
 - Persistance des données (via rechargement de page)
 - Interface responsive
 - Feedback visuel pour la suppression

2. Explication du code :
 # HTML
   - Formulaire d'ajout (`add`)
   - Champ de recherche (`search`)
   - Liste `todos` avec éléments pré-définis
   - Utilisation de classes Bootstrap (`form-control`, `list-group`)

 # CSS 
   - Thème violet (`#352f5b`) pour le fond
   - `.todos li` : Style des éléments de liste
   - `.hidden` : Classe utilitaire pour le filtrage
   - Effets de transparence (`background: rgba(0,0,0,0.2)`)

 # JavaScript Principales Fonctions
   - `addTodo()` : Crée un nouvel élément de liste
   - Événement `submit` sur le formulaire : Gère l'ajout
   - Événement `click` sur la liste : Gère la suppression
   - `filterTodos()` : Filtre les tâches selon la recherche
   - Événement `input` sur la recherche : Déclenche le filtrage
