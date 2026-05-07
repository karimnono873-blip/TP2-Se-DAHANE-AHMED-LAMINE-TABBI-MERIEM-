# 🚀 Systèmes Embarqués - Travaux Pratiques (STM32)

Bienvenue dans le dépôt central des Travaux Pratiques de Systèmes Embarqués pour l'année universitaire 2025/2026. Ce projet se concentre sur la programmation matérielle (Bare Metal) des microcontrôleurs de la famille **STM32 (Nucleo-C031C6)** en utilisant la bibliothèque **HAL (Hardware Abstraction Layer)**.

## 🌟 Concept Unique : Les Jumeaux Numériques

Pour chaque TP, en plus du code source C embarqué, ce dépôt inclut un **Rapport de Laboratoire Interactif Web (HTML/CSS/JS)**. Ces rapports ne sont pas statiques : ils intègrent un **Jumeau Numérique (Digital Twin)** permettant de simuler et visualiser le comportement des circuits (LEDs, Boutons, Potentiomètres) directement dans un navigateur web, offrant une expérience d'apprentissage et de démonstration inédite.

---

## 📁 Structure du Dépôt

### 🟢 [TP 1 : Maîtrise des GPIO](./TP1_GPIO)
**Objectif :** Comprendre les entrées/sorties numériques, les résistances de tirage (Pull-up) et la gestion temporelle.
* **Manipulations :** Clignotement simple, contrôle direct par bouton, et création d'un "Variateur de Vitesse" à 3 modes (Lent, Rapide, Fixe).
* **Compétences clés :** Machine à états non-bloquante (`HAL_GetTick()`), anti-rebond logiciel, lecture/écriture des registres de port.
* **Lien vers le Jumeau Numérique :** `compte_rendu_tp1.html`

### 🟠 [TP 2 : Lecture Analogique (ADC)](./TP2_ADC)
**Objectif :** Acquérir et numériser des signaux continus via le Convertisseur Analogique-Numérique (ADC 12 bits).
* **Manipulations :** Lecture d'un potentiomètre sur PA0 avec un mode d'attente active (Polling). Pilotage de la LED sur PA5 en fonction d'un seuil de basculement fixé à VREF/2 (50%).
* **Compétences clés :** Architecture SAR, résolution et quantum, gestion de l'énergie (`HAL_ADC_Stop()`), hystérésis logicielle.
* **Lien vers le Jumeau Numérique :** `compte_rendu_tp2.html`

---

## 🛠️ Outils et Matériel

* **Microcontrôleur :** Carte STM32 Nucleo-C031C6
* **Composants :** LEDs, Résistances, Boutons poussoirs, Potentiomètres rotatifs.
* **IDE & Générateur de code :** STM32CubeIDE avec STM32CubeMX
* **Simulateur Matériel en ligne :** [Wokwi pour STM32](https://wokwi.com/stm32)
* **Technologies Web (Jumeaux Numériques) :** HTML5, CSS3, Vanilla JavaScript

## ⚙️ Comment exécuter les projets ?

### 1. Côté Matériel (C)
1. Importez le dossier du TP souhaité dans **STM32CubeIDE**.
2. Vérifiez le pinout dans le fichier `.ioc`.
3. Compilez et flashez le code sur la carte Nucleo (ou copiez le code `main.c` dans Wokwi).

### 2. Côté Logiciel (Web)
1. Ouvrez le dossier du TP correspondant.
2. Double-cliquez sur le fichier `compte_rendu_tpX.html` pour l'ouvrir dans votre navigateur web préféré.
3. Interagissez avec les éléments visuels de la carte pour simuler le code C !

---

## 👥 Équipe du Projet

* **Binôme :** Dahane Ahmed Lamine & Tabbi Meriem
* **Enseignante Responsable :** Mme. Afaf Saoud
* **Département :** Électronique
* **Année Universitaire :** 2025/2026
