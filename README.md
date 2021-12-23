#Instalation
S'assurer que les requirements dans requirements.txt sont bien installé
De plus pour l<installation et le bon fonctionnement de ffmpeg 
il faut le télécharger du site suivant:\
https://ffmpeg.org/download.html#build-windows

##Demucs
conseillé d'installer l'environnement demucs dans anaconda prompt avec ces commandes:
```
cd ./demucs
conda env update -f environment-cpu.yml
conda activate demucs
```

#Training
##Sams-Net
S'assurer de configurer le path dans Config.py pour les trois path puis 
executer cette commande dans le terminal:
```
python Training.py with cfg.unet_spectrogram
```
##Demucs
effectuer cette commande dans anaconda prompt
```
python3 -m demucs -b 4  --musdb MUSDB_PATH
```