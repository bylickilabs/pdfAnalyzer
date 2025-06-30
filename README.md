# PDF Analyzer

**PDF Analyzer** ist ein effizientes Python-Tool zur automatischen Analyse von PDF-Dokumenten.  
Es extrahiert Metadaten, Textinhalte und statistische Kennzahlen und präsentiert diese übersichtlich – per Weboberfläche (Streamlit) oder Kommandozeile.

---

## 🚀 Features

- PDF-Upload per Weboberfläche oder CLI
- Metadaten-Analyse (Autor, Erstellungsdatum, Titel etc.)
- Text- und Seitenstatistiken (Seitenzahl, Wortanzahl, häufigste Begriffe)
- Übersichtliche, sofort verständliche Ausgabe
- Einfache Bedienung, keine Vorkenntnisse notwendig

---

## 🛠️ Installation

1. **Python 3.12.x installieren**  
   [Download-Link (Python.org)](https://www.python.org/downloads/release/python-3124/)  
   Während der Installation unbedingt **„Add Python to PATH“** aktivieren!

2. **Benötigte Pakete installieren**  
   Öffnen Sie die PowerShell (oder Terminal) und geben Sie ein:

```yarn
   pip install PyPDF2 pdfminer.six streamlit
```

3.Code herunterladen
  Laden Sie pdf_analyzer.py aus diesem Repository herunter
  oder klonen Sie das gesamte Repository mit:

```yarn
git clone https://github.com/IHR_GITHUB_BENUTZERNAME/IHR_REPOSITORY_NAME.git
cd IHR_REPOSITORY_NAME
```

---

▶️ Anwendung starten

```yarn
streamlit run pdf_analyzer.py
```

Der Browser öffnet sich automatisch unter http://localhost:8501.
Kommandozeile (CLI):

```yarn
python pdf_analyzer.py IhreDatei.pdf
```

```
python pdf_analyzer.py IhreDatei.pdf
```

- Ersetzen Sie IhreDatei.pdf durch den Namen Ihres PDF-Dokuments.

---

❓ Hinweise
Unterstützt werden unverschlüsselte PDF-Dateien.

Für die Streamlit-Weboberfläche muss pdf_analyzer.py den passenden Code für Streamlit enthalten.

---

📄 Lizenz
MIT License – [LICENSE](LICENSE)
