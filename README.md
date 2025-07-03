# 🐦 Nestflix ESP32

**Nestflix** est un projet personnel d’électronique embarquée : un **nichoir à oiseaux intelligent** combinant une STM32 et une ESP32.  
Ce dépôt contient le **firmware ESP32**, conçu pour la connectivité, l’interface web/API, et la communication entre les modules.

---

## 🧠 Objectif du projet

L’ESP32 agit comme une **passerelle intelligente** pour permettre à l'utilisateur de :
- Accéder aux **informations** du nichoir à distance (état, présence, images)
- Déclencher des **actions** (prise de photo, ouverture de trappe, éclairage LED, etc.)
- Transmettre les données du nichoir vers une **application mobile ou web**
- Interfacer avec la STM32 via **UART ou Bluetooth**
- Fournir une **API REST locale** ou **serveur BLE** simple pour contrôle externe
- Être autonome via **batterie + panneau solaire**

---

## ⚙️ Fonctionnalités actuelles

- 🔌 Connexion Wi-Fi en mode **Station (STA)**
- 🌐 Lancement d’un **serveur HTTP** sur le réseau local
  - Endpoint `/` répond avec : `Nestflix ESP32 ready!`

---

## 🚀 Mise en route

### 📦 Prérequis

- ESP32 DevKit (n’importe quelle version)
- [ESP-IDF](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/) (v5 recommandé)
- VS Code avec l’extension **ESP-IDF**

### 🔧 Configuration Wi-Fi

Lance la configuration avec :
```bash
idf.py menuconfig
