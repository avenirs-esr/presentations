---
marp: true
theme: gaia
avenirs-toc: Point d'étape - Focus sur la sécurité
paginate: true
_class:
  - invert
  - lead
header: ""
footer: '![height:40px](https://avenirs-esr.github.io/dev-doc/assets/images/avenir-esr-logo_medium.jpg) ![height:40px](https://www.esup-portail.org/sites/default/files/logo-esupportail_1.png)'
style: |
  section::after {
    left: 0;
    right: 0;
    text-align: center;
  }
---

<style>
  :root {
    #--color-background: #ddd;
    #--color-background-code: #ccc;
    --color-background-paginate: rgba(128, 128, 128, 0.05);
    #--color-foreground: #345;
    --color-highlight: #f96;
    --color-highlight-hover: #aaf;
    --color-highlight-heading: #99c;
    --color-header: #fff;
    --color-header-shadow: transparent;
    --marpit-root-font-size: 28px;
    
  }
  section {
    line-height: 1.2;
    padding : 30px 40px;
  }
 
  li {
    font-szie: 1em;
    margin: .1em 0;
  }
  ul > li > ul > li {
  font-size: .9em;
  margin: unset;
}
  footer {
    height: 50px;
    display:grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows:100%;
  }
  footer img:nth-of-type(2) {
    grid-column: 4;
    background-color: #fff;
  }
</style>

# **Focus sur la sécurité**

***16/04/2024***

Julien Gribonvald - Coordinateur Technique ESUP
Arnaud Deman - Architecte et développeur ESUP

---
## Sécurité & confidentialité : contexte

* Problématiques qui ne peuvent plus être traitées à la marge.
* Caratéristiques du projet :
    - Mode SASS / hybride, cadre national.
    - Projet complexe.
    - Forte population d'utilisateurs potentiels.
    - De nombreuses interactions avec des services extérieurs.
  
* Domaine vaste et complexe : un effort de **formalisation nécessaire.**
* Actualisation des connaissances : 
  - [OWASP](https://owasp.org/) : Open Worldwide Application Security Project.
  - [ANNSI](https://cyber.gouv.fr/decouvrir-lanssi) : Agence nationale de la sécurité des systèmes d'information.
  - ...

---

## Security by design
  - Prise en compte de la sécurité dès la conception et à chaque phase du projet. 
  - Repose sur un certain nombre de grands principes : surface d'attaque, moindre privilèges, défense en profondeur, etc.
  - Mise en place de procédures documentées.
  - Puis implémentées : revues de code, vérifications automatiques, etc.
  - ... et révisées régulièrement.
  - Processus d'amélioration continue.
  - Golden Path : baliser au mieux la voie pour atteindre l'objectif.
---

## Mise en oeuvre
- Procédure en cours d'élaboration.
- Documents de sécurité : niveau projet & grands modules fonctionnels.
  - Contexte, surface d'attaque, technologies, etc.
- Documents transversaux : 
  - Dictionnaire des données classifiées par niveau de criticité.
  - Matrices des droits / rôles.
  - Check listes thématiques.
  
---
## Schéma général

<style scoped type="text/css">
  img[alt="Big Picture"] {
    width: 525px;
    margin-left: auto;
    margin-right: auto;
    display: block;
  }
</style>

![Big Picture](../img/security-by-design-big-picture.png)

---

<!--
header: Ressources
-->
## [Pour tout savoir](https://avenirs-esr.github.io/dev-doc/)

### https://avenirs-esr.github.io/dev-doc/
