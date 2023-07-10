# Basisimage
FROM python:3.9

# Benutzer hinzufügen
RUN groupadd -r appuser && useradd -r -g appuser appuser

# Arbeitsverzeichnisse erstellen
WORKDIR /app
COPY . /app

# Anforderungen hinzufügen/installieren
RUN pip install --no-cache-dir -r requirements.txt

# Inhaber von /app ändern
RUN chown -R appuser:appuser /app
USER appuser

# Befehle bei Container Start
CMD ["python", "app.py"]