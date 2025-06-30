import PyPDF2
import sys
from collections import Counter
import re

def analyze_pdf(file_path):
    with open(file_path, 'rb') as f:
        reader = PyPDF2.PdfReader(f)
        info = reader.metadata
        print("---- Metadaten ----")
        for k, v in info.items():
            print(f"{k}: {v}")

        text = ""
        for page in reader.pages:
            text += page.extract_text() or ""
        print("\nSeitenanzahl:", len(reader.pages))
        print("Zeichenanzahl:", len(text))
        
        words = re.findall(r'\w+', text.lower())
        print("Wortanzahl:", len(words))
        counter = Counter(words)
        print("\nTop 10 Wörter:")
        for word, count in counter.most_common(10):
            print(f"{word}: {count}")

if __name__ == "__main__":
    if len(sys.argv) != 2:
        print("Usage: python pdf_analyzer.py <file.pdf>")
        sys.exit(1)
    analyze_pdf(sys.argv[1])
