---
marp: true
theme: default
size: 16:9
paginate: true
footer: "Veille technologique · OFPPT Solicode · Novembre 2026"
style: |
  section {
    font-family: 'Segoe UI', 'Inter', Roboto, Arial, sans-serif;
    background: #ffffff;
    color: #0D2A4D;
    font-size: 25px;
    padding: 56px 68px 60px 68px;
  }
  section::before { content: ""; position: absolute; top: 0; left: 0; right: 0; height: 10px; background: #1565C0; }
  section h1 { color: #0D2A4D; font-size: 1.5em; margin: 0 0 0.55em 0; letter-spacing: -0.5px; }
  section h2 { color: #1565C0; font-size: 1em; margin: 0.2em 0 0.3em 0; text-transform: uppercase; letter-spacing: 1px; }
  section h3 { color: #1565C0; margin: 0.1em 0 0.3em 0; font-size: 1em; }
  section strong { color: #1565C0; }
  section a { color: #1565C0; text-decoration: none; }
  section li { margin: 0.22em 0; }
  section footer, section::after { color: #78909C; font-size: 14px; }
  section code { background: #E3F2FD; color: #0D2A4D; border-radius: 4px; padding: 1px 6px; font-size: 0.85em; }
  section.cover, section.dark {
    background: linear-gradient(135deg, #0D2A4D 0%, #1565C0 100%); color: #fff; justify-content: center;
  }
  section.cover::before, section.dark::before { background: #64B5F6; height: 14px; }
  section.cover h1, section.dark h1 { color: #fff; font-size: 2.3em; line-height: 1.1; }
  section.cover h2, section.dark h2 { color: #90CAF9; }
  section.cover strong, section.dark strong { color: #90CAF9; }
  section.cover footer, section.dark footer, section.cover::after, section.dark::after { color: #BBDEFB; }
  .cover-logos { display: flex; align-items: center; justify-content: center; gap: 24px; margin-bottom: 20px; }
  .logo-solicode { width: 280px; height: 90px; object-fit: cover; object-position: center; }
  .logo-ofppt { width: 92px; height: 92px; object-fit: contain; }
  .kicker { color: #1565C0; font-size: 0.62em; font-weight: 700; letter-spacing: 2px; text-transform: uppercase; margin-bottom: 4px; }
  section.cover .kicker, section.dark .kicker { color: #90CAF9; }
  .cols { display: grid; grid-template-columns: 1.15fr 1fr; gap: 32px; align-items: start; }
  .cols.even { grid-template-columns: 1fr 1fr; }
  .flow { display: flex; align-items: center; justify-content: center; gap: 12px; margin: 16px 0; }
  .box { background: #E3F2FD; border: 2px solid #1565C0; border-radius: 12px; padding: 12px 18px; text-align: center; font-size: 0.82em; flex: 1; }
  .box.dark { background: #0D2A4D; color: #fff; border-color: #0D2A4D; }
  .box.dark strong { color: #90CAF9; }
  .arrow { font-size: 1.4em; color: #1565C0; font-weight: 700; }
  .badge { display: inline-block; background: #1565C0; color: #fff; font-weight: 800; font-size: 0.6em; padding: 4px 14px; border-radius: 20px; letter-spacing: 1px; margin-bottom: 10px; }
  .path { font-family: Consolas, 'Courier New', monospace; background: #E3F2FD; border-radius: 6px; padding: 6px 12px; font-size: 0.78em; display: block; margin: 8px 0; }
  .goal { background: #E3F2FD; border-left: 6px solid #1565C0; padding: 8px 14px; border-radius: 6px; font-size: 0.88em; margin-bottom: 10px; }
  .result { background: #F5F9FF; border: 2px solid #1565C0; border-radius: 10px; padding: 9px 14px; font-size: 0.82em; margin-top: 10px; }
  .note { background: #FFF8E1; border-left: 6px solid #FFB300; padding: 8px 14px; border-radius: 6px; font-size: 0.8em; margin-top: 10px; }
  .small { font-size: 0.72em; color: #607D8B; }
  .card { background: #F5F9FF; border-radius: 12px; padding: 12px 18px; border-top: 5px solid #1565C0; }
  .plan { list-style: none; padding: 0; counter-reset: p; }
  .plan li { counter-increment: p; margin: 0.45em 0; font-size: 1.05em; }
  .plan li::before { content: counter(p); display: inline-block; width: 1.6em; height: 1.6em; line-height: 1.6em; text-align: center; background: #1565C0; color: #fff; border-radius: 50%; margin-right: 0.7em; font-weight: 700; font-size: 0.85em; }
  table { font-size: 0.78em; border-collapse: collapse; width: 100%; }
  th { background: #0D2A4D; color: #fff; padding: 9px; text-align: left; }
  td { padding: 9px; border-bottom: 1px solid #CFD8DC; }
---

<!-- _class: cover -->
<!-- _paginate: false -->

<div class="cover-logos">
<img src="./images/logo_solicode.png" alt="Logo Solicode" class="logo-solicode">
<img src="./images/ofppt_logo.png" alt="Logo OFPPT" class="logo-ofppt">
</div>

<div class="kicker">Veille technologique</div>

# Android Development
## Getting Started : installer son environnement

Android Studio · Android SDK · Émulateur

OFPPT Solicode · Novembre 2026

---

<div class="kicker">Sommaire</div>

# Plan

<ol class="plan">
<li>Introduction</li>
<li>Problématique</li>
<li>Le développement mobile</li>
<li>L'écosystème Android</li>
<li>Installation et configuration (démonstration)</li>
<li>Analyse : difficultés, comparaison et bonnes pratiques</li>
<li>Conclusion</li>
</ol>

---

<div class="kicker">Introduction</div>

# Introduction

- Les **applications mobiles** font partie du quotidien : communication, services, loisirs
- **Android** est l'un des deux grands systèmes mobiles, aux côtés d'iOS
- Pour créer une application Android, il faut un **environnement de développement** adapté
- Google fournit des **outils officiels** : Android Studio, Android SDK, émulateur
- Le langage **Kotlin** et la bibliothèque **Jetpack Compose** sont recommandés pour Android

---

<!-- _class: dark -->

<div class="kicker">Problématique</div>

# Problématique

## Comment préparer un environnement de développement Android fiable, et quels outils le composent ?

- Quels sont les **composants** de l'écosystème Android ?
- Comment **installer et configurer** ces outils ?
- Comment **vérifier** que l'environnement est opérationnel ?

---

<div class="kicker">I · Le développement mobile</div>

# Applications mobiles : trois approches

| | **Native** | **Cross-platform** | **PWA** |
|---|---|---|---|
| **Principe** | Une application par système | Un code partagé entre systèmes | Site web installable |
| **Exemples** | Kotlin pour Android | Flutter, React Native | HTML, CSS, JavaScript |
| **Accès au téléphone** | Complet | Bon (via des plugins) | Limité par le navigateur |

👉 Cette présentation se concentre sur le **natif Android**.

---

<div class="kicker">II · L'écosystème Android</div>

# Qu'est-ce qu'Android ?

- Un **système d'exploitation mobile** basé sur le noyau **Linux**
- Construit sur **AOSP** (*Android Open Source Project*), un projet **open source**
- Il équipe des smartphones, des tablettes et d'autres appareils
- Les applications sont distribuées via un **magasin d'applications**

<div class="flow">
<div class="box">Matériel</div><div class="arrow">→</div>
<div class="box">Noyau Linux</div><div class="arrow">→</div>
<div class="box">Android</div><div class="arrow">→</div>
<div class="box dark">Applications</div>
</div>

---

<div class="kicker">II · L'écosystème Android</div>

# Android, Kotlin, SDK, Studio : quatre notions distinctes

<div class="cols even">
<div class="card">

**Android** → le système d'exploitation

**Kotlin** → un langage de programmation

**Android SDK** → outils et bibliothèques pour créer des applications

**Android Studio** → l'IDE officiel

</div>
<div>

⚠️ **Kotlin ne fait pas partie d'Android.**

C'est un langage qui **peut être utilisé** pour développer sur Android (et ailleurs). Google le recommande pour le développement Android.

*Analogie : Android = la route · Kotlin = la langue · SDK = la caisse à outils · Studio = l'atelier.*

</div>
</div>

---

<div class="kicker">II · L'écosystème Android</div>

# Les cinq outils principaux

| Outil | Rôle |
|---|---|
| **Android Studio** | IDE officiel : écrire, compiler, tester, déboguer |
| **Kotlin** | Langage pour écrire le code |
| **Jetpack Compose** | Création de l'interface en code (approche déclarative) |
| **Gradle** | Compile le projet et gère les dépendances |
| **Android Emulator** | Exécute l'application sur un téléphone virtuel |

---

<div class="kicker">II · L'écosystème Android</div>

# Comment les outils travaillent ensemble

<div class="flow">
<div class="box">Code <strong>Kotlin</strong><br>+ <strong>Compose</strong></div><div class="arrow">→</div>
<div class="box"><strong>Gradle</strong><br>compile le projet</div><div class="arrow">→</div>
<div class="box">Application<br>Android</div><div class="arrow">→</div>
<div class="box dark"><strong>Émulateur</strong><br>ou téléphone</div>
</div>

<div class="flow">
<div class="box dark" style="flex:none; width:85%">Pilotés depuis <strong>Android Studio</strong>, qui s'appuie sur l'<strong>Android SDK</strong></div>
</div>

---

<div class="kicker">II · L'écosystème Android</div>

# Avantages du développement natif

- **Outils officiels** et documentation maintenue par Google
- **Accès complet** aux fonctions du système
- **Kotlin** : langage moderne et concis
- **Jetpack Compose** : interface moderne, moins de code
- **Aperçu et débogage** intégrés à l'IDE
- **Grande communauté** et nombreux exemples

<p class="small">Limite : le code natif Android ne s'exécute pas tel quel sur iOS.</p>

---

<div class="kicker">III · Installation et configuration</div>

# Prérequis matériels et logiciels

<div class="cols even">
<div class="card">

### Matériel (minimum officiel)
- **8 Go de RAM** (16 Go conseillés)
- **8 Go d'espace disque** (IDE + SDK + émulateur)
- Écran **1280 × 800** minimum
- Processeur 64 bits avec **virtualisation**

</div>
<div class="card">

### Logiciel
- Windows, macOS, Linux ou ChromeOS, en **64 bits**
- Connexion **Internet**
- **Aucun JDK à installer** : Android Studio inclut le sien

</div>
</div>

<p class="small">Versions exactes du système : developer.android.com/studio</p>

---

<!-- _class: dark -->

<div class="kicker">III · Installation et configuration</div>

# Démonstration

## Cinq étapes pour un environnement prêt

<div class="flow">
<div class="box dark" style="border-color:#90CAF9">1<br>Installer<br>Android Studio</div><div class="arrow" style="color:#90CAF9">→</div>
<div class="box dark" style="border-color:#90CAF9">2<br>Assistant de<br>configuration</div><div class="arrow" style="color:#90CAF9">→</div>
<div class="box dark" style="border-color:#90CAF9">3<br>SDK<br>Manager</div><div class="arrow" style="color:#90CAF9">→</div>
<div class="box dark" style="border-color:#90CAF9">4<br>Créer<br>un AVD</div><div class="arrow" style="color:#90CAF9">→</div>
<div class="box dark" style="border-color:#90CAF9">5<br>Vérifier</div>
</div>

---

<span class="badge">ÉTAPE 1 / 5</span>

# Télécharger et installer Android Studio

<div class="cols">
<div>

<div class="goal">🎯 <strong>Objectif :</strong> installer l'IDE officiel.</div>

1. Ouvrir **developer.android.com/studio**
2. Cliquer sur **Download Android Studio** et accepter la licence
3. **Windows** : lancer l'installateur `.exe` et suivre l'assistant
4. **macOS** : ouvrir le `.dmg`, glisser dans **Applications**
5. Lancer Android Studio

</div>
<div>

<div class="result">✅ <strong>Résultat attendu :</strong> la fenêtre <strong>Welcome to Android Studio</strong> s'ouvre.</div>

<div class="note">⚠️ Télécharger uniquement depuis le <strong>site officiel</strong>.</div>

</div>
</div>

---

<span class="badge">ÉTAPE 2 / 5</span>

# Assistant de première configuration

<div class="cols">
<div>

<div class="goal">🎯 <strong>Objectif :</strong> installer les composants de base.</div>

1. Choisir l'installation **Standard**
2. Laisser les **paquets SDK recommandés** se télécharger
3. Accepter les **licences** demandées
4. Cliquer sur **Finish** et patienter

</div>
<div>

<div class="result">✅ <strong>Résultat attendu :</strong> SDK et outils installés, l'IDE est prêt.</div>

<div class="note">⏱️ La durée dépend de la connexion Internet.</div>

</div>
</div>

---

<span class="badge">ÉTAPE 3 / 5</span>

# Configurer l'Android SDK

<div class="cols">
<div>

<div class="goal">🎯 <strong>Objectif :</strong> vérifier les composants du SDK.</div>

<span class="path">Settings › Languages & Frameworks › Android SDK</span>

1. Onglet **SDK Platforms** : une version d'Android installée
2. Onglet **SDK Tools** : *Build-Tools*, *Platform-Tools*, *Emulator*
3. **Apply** pour installer un élément manquant

</div>
<div>

<div class="result">✅ <strong>Résultat attendu :</strong> les composants nécessaires sont marqués <em>Installed</em>.</div>

<p class="small">Raccourci : menu <strong>Tools › SDK Manager</strong>. Sur macOS : <em>Preferences</em>.</p>

</div>
</div>

---

<span class="badge">ÉTAPE 4 / 5</span>

# Créer un émulateur Android (AVD)

<div class="cols">
<div>

<div class="goal">🎯 <strong>Objectif :</strong> disposer d'un téléphone virtuel.</div>

<span class="path">Device Manager › Create Virtual Device</span>

1. Choisir un **modèle** d'appareil (ex. un Pixel) → **Next**
2. Choisir une **System Image** et la **télécharger**
3. Nommer l'AVD → **Finish**

</div>
<div>

<div class="result">✅ <strong>Résultat attendu :</strong> l'AVD apparaît dans la liste des appareils.</div>

<div class="note">💡 <strong>AVD</strong> = <em>Android Virtual Device</em>, le téléphone virtuel.</div>

</div>
</div>

---

<span class="badge">ÉTAPE 5 / 5</span>

# Démarrer l'émulateur et vérifier

<div class="cols">
<div>

<div class="goal">🎯 <strong>Objectif :</strong> confirmer que tout fonctionne.</div>

1. Dans **Device Manager**, cliquer sur **▶** à côté de l'AVD
2. Attendre le **démarrage** du téléphone virtuel
3. Vérifier que l'écran d'accueil Android répond

</div>
<div>

<div class="result">✅ <strong>Résultat attendu :</strong> un téléphone Android virtuel s'affiche et répond.</div>

<div class="note">⏱️ Le <strong>premier démarrage</strong> est le plus lent.</div>

</div>
</div>

---

<div class="kicker">III · Installation et configuration</div>

# Vérification de l'environnement

<div class="cols even">
<div class="card">

- ✅ Android Studio **se lance** sans erreur
- ✅ **SDK Manager** : plateforme et outils installés
- ✅ **Device Manager** : au moins un AVD
- ✅ L'**émulateur démarre** et répond

</div>
<div>

**Quatre points validés** : l'environnement de développement Android est opérationnel.

En cas d'échec, voir les difficultés fréquentes présentées ensuite.

</div>
</div>

---

<div class="kicker">IV · Analyse</div>

# Difficultés fréquentes et solutions

| Problème | Piste de solution |
|---|---|
| **L'émulateur ne démarre pas** | Activer la **virtualisation** (BIOS / paramètres du système) |
| **Composants manquants** | Les installer via le **SDK Manager** |
| **Téléchargement interrompu** | Vérifier la connexion Internet, puis relancer |
| **Machine lente** | Fermer d'autres applications, vérifier RAM et disque |
| **Aucun appareil disponible** | Créer ou démarrer un AVD dans **Device Manager** |
| **Espace disque insuffisant** | Libérer de l'espace avant l'installation |

---

<div class="kicker">IV · Analyse</div>

# Android natif, Flutter, React Native

| | **Android natif** | **Flutter** | **React Native** |
|---|---|---|---|
| **Langage** | Kotlin | Dart | JavaScript / TypeScript |
| **Plateformes** | Android | Plusieurs | Plusieurs |
| **Interface** | Jetpack Compose | Widgets Flutter | Composants React |
| **Atout** | Outils officiels, accès complet | Un code pour plusieurs OS | Écosystème JavaScript |
| **À considérer** | Code propre à Android | Apprendre Dart | Dépendance à des bibliothèques |

**Le bon choix dépend du projet, de l'équipe et des plateformes visées.**

---

<div class="kicker">IV · Analyse</div>

# Bonnes pratiques

- **Télécharger** Android Studio depuis le **site officiel**
- **Garder** l'IDE à jour (**Help › Check for Update**)
- **Lire** les messages d'erreur : ils indiquent souvent la solution
- **S'appuyer** sur la documentation officielle d'Android Developers
- **Avancer** par petites étapes et tester souvent
- **Vérifier** l'environnement avant de commencer un projet

---

<!-- _class: dark -->

<div class="kicker">Conclusion</div>

# Conclusion

- **Android** est un système ; **Kotlin**, le **SDK** et **Android Studio** sont des outils distincts
- L'installation se fait en **cinq étapes** : Android Studio, assistant, SDK, AVD, vérification
- Un environnement **vérifié** évite la plupart des blocages
- **Perspective :** créer un premier projet avec **Kotlin** et **Jetpack Compose**

---

<!-- _class: dark -->

<div class="kicker">Webographie</div>

# Ressources officielles

- 🔗 **Android Developers** : developer.android.com
- 🔗 **Android Studio** : developer.android.com/studio
- 🔗 **Installation** : developer.android.com/studio/install
- 🔗 **Kotlin sur Android** : developer.android.com/kotlin
- 🔗 **Jetpack Compose** : developer.android.com/develop/ui/compose

**Merci pour votre attention. Questions ?**