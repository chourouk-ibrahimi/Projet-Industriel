# Système de Détection de Collision — Essaim UAV

**École des Sciences de l'Information**  
**Programmation Avancée en C — Pr. Tarik HOUICHIME**  
**Projet Industriel**

---

## 📋 Description du Projet

Système de sécurité pour un essaim de 10 000 micro-drones autonomes. L'algorithme identifie instantanément les deux drones les plus proches dans l'espace 3D pour déclencher une manœuvre d'évitement et prévenir un crash en chaîne catastrophique.

---

## 🏗️ Architecture

| Caractéristique | Détail |
|-----------------|--------|
| **Algorithme** | Sweep Line (Balayage linéaire) + Tri par projection axiale |
| **Complexité** | O(n log n) |
| **Contrainte** | Aucune indexation par crochets — arithmétique pure des pointeurs |
| **Volume de vol** | 1000m × 1000m × 1000m |
| **Nombre de drones** | 10 000 |

---

## ⚙️ Compilation

```bash
gcc -O2 -o uav main.c -lm
