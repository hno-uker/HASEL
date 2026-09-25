Mit Github Desktop (o.ä) Hazel clonen unter
C:\Repositories\HASEL
quelle: https://github.com/hno-uker/HASEL
das selbe für cotracker (benötigt von VFLabel)
C:\Repositories\HASEL
quelle: https://github.com/facebookresearch/co-tracker

Anaconda Prompt
```bash
conda create --name VFLabel python=3.12
conda activate VFLabel
```

In das verzeichnis/repo von HASEL wechseln
```bash
cd C:\Repositories\HASEL
pip install -r requirements.txt
pip install -e .
pip install -e ..\co-tracker
```

Modelle runterladen von
https://drive.google.com/drive/folders/1U525TcxZ1nhIp5yNJiyW-avK6qZG4rVV
und abspeichern unter
C:\Repositories\HASEL\assets\models
Zusätzlich runterladen
https://huggingface.co/facebook/cotracker3/resolve/main/scaled_offline.pth
und abspeichern unter
C:\Repositories\HASEL\assets\models

HASEL ausführen:
```bash
python VFLabel\main.py
```