# Frontend Mentor - Social Links Profile

Ce projet est une intégration d'un composant de profil avec des liens sociaux, basé sur un défi proposé par la plateforme Frontend Mentor. L'objectif était de reproduire fidèlement le design fourni tout en adoptant une structure de code logique et maintenable.


## Présentation du projet

Le projet consiste en une carte de profil épurée présentant l'avatar d'une développeuse front-end, sa localisation, une courte biographie, ainsi qu'une liste de boutons cliquables redirigeant vers ses différents réseaux sociaux (GitHub, Frontend Mentor, LinkedIn, Twitter et Instagram).

## Ma démarche et processus de développement

### 1. Structure HTML5 sémantique
Pour ce projet, j'ai mis un point d'honneur à utiliser des balises HTML5 sémantiques afin de garantir une bonne accessibilité et un code compréhensible :
- L'utilisation de la balise `<main>` pour envelopper le contenu principal de la page.
- Une division (`<div>`) centrale faisant office de conteneur pour le composant carte.
- Une balise `<nav>` dédiée pour regrouper l'ensemble des liens sociaux, ce qui est structurellement plus logique pour les lecteurs d'écran qu'une simple suite de boutons isolés.
- Un élément `<footer>` en bas de page pour l'attribution du défi, séparé du flux principal.

### 2. Choix de l'architecture CSS
Le style a été embarqué directement dans le document via une balise `<style>` pour centraliser l'exercice de manière autonome. 
- **Polices et typographie :** Intégration de la police Google Fonts "Inter", avec une gestion précise des graisses (`font-weight: 700`) et des tailles relatives pour correspondre au modèle.
- **Réinitialisation des marges :** Application de classes spécifiques (`.en-tête`) pour neutraliser les marges par défaut des balises de titre (`<h2>`, `<h5>`) afin d'éviter les décalages imprévus causés par les styles natifs des navigateurs.

### 3. Gestion du positionnement et de l'alignement
Le positionnement de la carte s'appuie sur des valeurs de marges calculées en pourcentage (`margin-left`, `margin-top`) pour centrer le bloc sur l'écran de manière fluide. 

Pour le bloc de navigation interne, l'utilisation de Flexbox (`display: flex`) configuré en colonne (`flex-direction: column`) a permis d'aligner verticalement et de centrer parfaitement tous les boutons d'interaction, assurant une régularité visuelle sur l'ensemble du profil.

## Technologies utilisées

- HTML5 (Sémantique)
- CSS3 (Flexbox, sélecteurs d'identifiants et de classes)
- Google Fonts (Famille de polices Inter)
- Cloudinary (Hébergement et optimisation de la ressource d'image de l'avatar)

## Optimisations 

Intégration du @media querry afin de rendre le design responsive sur les appareils mobiles 
 ```css
 @media (max-width: 480px) and (min-width: 360px) {
  
  main {
    width: 100vw;       
    height: auto;      
    margin-left: 0;     
    min-height: 100vh;  
    padding-bottom: 40px; 
  }

  /* Ta logique de carte fluide qui est excellente */
  div {
    width: 86vw;        
    height: auto;       
    margin-left: auto;  
    margin-right: auto; 
    margin-top: 20%;    
    padding-bottom: 30px;
  }
  button {
    width: 85%;         
  }
}
```
