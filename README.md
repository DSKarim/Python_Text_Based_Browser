<h1 align="center">🌐 Text-Based Browser</h1>

<p align="center"><em>Surfe le web en mode texte : juste le contenu, rien que le contenu.</em></p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python 3" />
  <img src="https://img.shields.io/badge/d%C3%A9pendances-3%20externes-orange?style=for-the-badge" alt="3 dépendances externes" />
  <img src="https://img.shields.io/badge/projet%20d%27apprentissage-ff69b4?style=for-the-badge" alt="Projet d'apprentissage" />
</p>

---

## ✨ Pourquoi tu vas l'adorer

- **Le texte utile** : paragraphes, titres `h1` à `h6`, liens et listes.
- **Liens en bleu** dans le terminal, grâce à colorama.
- **Cache intégré** : chaque site est enregistré dans un dossier, donc une deuxième visite se lit sans réseau.
- **Retour arrière** avec `back`.

## 📦 Installation

```bash
pip install requests beautifulsoup4 colorama
```

## 🚀 Lancer

```bash
python3 Code_Python_Text_Based_Browser tb_tabs
```

`tb_tabs` est le dossier de cache des pages. Il est créé automatiquement s'il n'existe pas.

## 🎮 Commandes

| Saisie | Effet |
|---|---|
| `python.org` | Charge `https://python.org` (le préfixe est ajouté si besoin) |
| `back` | Revient à la page précédente |
| `exit` | Quitte le programme |

Si la connexion échoue, le programme affiche `Error: Incorrect URL`.

## 🧠 Sous le capot

- `requests` télécharge la page, `BeautifulSoup` en analyse le HTML.
- Une `deque` sert de pile pour l'historique de navigation.
- Chaque site est enregistré dans `tb_tabs/` sous forme de fichier texte. S'il existe déjà, il est relu sans réseau.

## 🔭 Pistes d'évolution

- Numéroter les liens pour pouvoir les suivre en tapant leur numéro.
- Sécuriser `back` lorsque l'historique est vide.

---

<p align="center"><sub>Fait avec ❤️ et Python par DSKarim</sub></p>
