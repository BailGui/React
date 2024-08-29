# React

## Démarrage rapide

Bienvenue dans la documentation React ! Dans cette page, vous allez découvrir les 80% de concepts React que vous utiliserez sans doute au quotidien.
Vous allez apprendre

    Comment créer et imbriquer des composants
    Comment ajouter du balisage et des styles
    Comment afficher des données
    Comment faire un rendu conditionnel et traiter des listes
    Comment réagir à des événements et mettre à jour l’affichage
    Comment partager des données entre composants

## Créer et imbriquer des composants

Les applis React sont constituées de composants. Un composant, c’est un bout d’UI (User Interface, donc interface utilisateur) avec son comportement et son apparence propres. Un composant peut être aussi petit qu’un bouton, ou aussi grand qu’une page entière.

## Les composants React sont des fonctions JavaScript qui renvoient du balisage :

```
function MyButton() {
return (
<button>Je suis un bouton</button>
);
}
```

## À présent que vous avez déclaré MyButton, vous pouvez l’imbriquer dans un autre composant :

```
export default function MyApp() {
return (
<div>
<h1>Bienvenue dans mon appli</h1>
<MyButton />
</div>
);
}
```

Remarquez que <MyButton /> commence par une majuscule. C’est comme ça que React sait qu’il s’agit d’un composant. Les noms de composants React doivent toujours démarrer par une majuscule, alors que les balises HTML doivent être en minuscules.

## Voyons ce que ça donne :

```
function MyButton() {
return (
<button>
Je suis un bouton
</button>
);
}

export default function MyApp() {
return (
<div>
<h1>Bienvenue dans mon appli</h1>
<MyButton />
</div>
);
}
```
