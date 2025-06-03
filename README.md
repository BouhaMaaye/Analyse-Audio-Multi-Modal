🎵 Analyse Audio Multi-Modal

📖 Description
Ce projet propose une analyse complète et automatisée de signaux audio utilisant des techniques de traitement du signal pour classifier et caractériser différents types de contenus sonores : voix féminine, voix masculine, chant, musique instrumentale et mélanges audio.

🎯 Objectifs
Classification automatique de contenus audio (parole vs chant vs musique)
Extraction de caractéristiques temporelles, fréquentielles et spectro-temporelles
Analyse comparative de signatures acoustiques
Visualisation interactive des propriétés audio

🔬 Analyses Implémentées

📊 1. Analyse Temporelle

Ondes temporelles : Visualisation de l'amplitude dans le temps
Détection d'onsets : Identification des attaques sonores
Calcul RMS : Énergie moyenne du signal
Durée et segmentation : Structure rythmique

🎼 2. Analyse Fréquentielle

Transformée de Fourier (FFT) : Spectre de puissance
Fréquence fondamentale (F0) : Détection de hauteur
Fréquences dominantes : Pics spectraux principaux
Analyse harmonique : Contenu spectral

🔥 3. Analyse Spectro-Temporelle

Spectrogrammes : Évolution fréquentielle dans le temps
Détection de formants : Caractéristiques vocales
Analyse temps-fréquence : Dynamique spectrale


⚡ 4. Caractéristiques Avancées

Zero Crossing Rate (ZCR) : Mesure de complexité spectrale
Classification automatique : Algorithmes de reconnaissance
Métriques acoustiques : Paramètres quantitatifs

📁 Structure du Projet
audio-analysis/
├── data/
│   ├── voix_feminine.wav
│   ├── voix_masculine.wav
│   ├── voix_musique.wav
│   └── musique_instrumentale.wav
├── notebooks/
│   └── audio_analysis_demo.ipynb
└── README.md

🛠️ Technologies Utilisées

Python 3.8+
Librosa : Analyse audio et extraction de caractéristiques
NumPy/SciPy : Calculs scientifiques et traitement de signal
Matplotlib/Seaborn : Visualisations et graphiques
Pandas : Manipulation de données
Scikit-learn : Algorithmes de classification

📦 Installation


# Installer les dépendances
pip install -r requirements.txt
🚀 Utilisation
Analyse Rapide
python
from src.audio_processor import AudioAnalyzer

# Initialiser l'analyseur
analyzer = AudioAnalyzer()

# Charger et analyser un fichier audio
results = analyzer.analyze_file('data/voix_feminine.wav')

# Afficher les résultats
analyzer.plot_analysis(results)
Analyse Comparative
python
# Comparer plusieurs fichiers
files = ['voix_feminine.wav', 'voix_masculine.wav', 'musique.wav']
comparison = analyzer.compare_files(files)
analyzer.plot_comparison(comparison)
📊 Résultats Principaux


🎤 Classification par Type Audio
Type Audio	F0 Moyen (Hz)	ZCR Moyen	RMS Max	Caractéristiques
Voix Féminine	228.2	0.1337	0.539	Formants nets, structure segmentée
Voix Masculine	272.6	0.1608	0.752	Chant continu, richesse harmonique
Voix + Musique	123.9	0.1267	0.205	Mélange complexe, basses dominantes
Musique Instrumentale	120.7	0.0513	0.192	Signal tonal, faible ZCR

🔍 Découvertes Clés
ZCR discriminant : Permet de distinguer contenu vocal (ZCR élevé) vs instrumental (ZCR bas)
Formants vocaux : Signature spectro-temporelle unique pour identifier la parole
F0 pour genre : Différenciation masculine/féminine par fréquence fondamentale
Analyse temporelle : Structure segmentée (parole) vs continue (chant/musique)

📈 Visualisations Générées
Ondes temporelles : Amplitude vs temps
Spectres FFT : Contenu fréquentiel
Spectrogrammes : Cartes temps-fréquence
Courbes ZCR : Évolution de la complexité spectrale
Analyses comparatives : Métriques multi-fichiers


🎯 Applications
Reconnaissance vocale : Préprocessing et caractérisation
Classification musicale : Genre et style automatiques
Qualité audio : Évaluation de signaux
Forensique audio : Analyse de contenu
Accessibilité : Transcription et sous-titrage

🤝 Contributions
Les contributions sont les bienvenues !

Fork le projet
Créer une branche feature (git checkout -b feature/nouvelle-fonctionnalite)
Commit les changements (git commit -m 'Ajout nouvelle fonctionnalité')
Push sur la branche (git push origin feature/nouvelle-fonctionnalite)
Ouvrir une Pull Request

📄 Licence
Ce projet est sous licence MIT. Voir le fichier LICENSE pour plus de détails.

👥 Auteurs
MAAYE BOUHA- Développement principal - @votre-github
🙏 Remerciements

Librosa pour les outils d'analyse audio
Matplotlib pour les visualisations
Communauté Python pour l'écosystème scientifique

📚 Références
Müller, M. (2015). Fundamentals of Music Processing
McFee, B. et al. (2015). librosa: Audio and music signal analysis in python
Serra, X. (2007). Musical Sound Modeling with Sinusoids plus Noise

⭐ N'hésitez pas à star le projet si vous le trouvez utile ! ⭐

