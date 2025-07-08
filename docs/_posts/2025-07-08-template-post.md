---
layout: post
title: "Template Post: Ein Beispiel für Jekyll Posts"
date: 2025-07-08 23:25:00 +0200
author: Arne Magold
categories: [template, beispiel]
tags: [jekyll, markdown, blog]
excerpt: "Dies ist ein Template-Post, der als Vorlage für zukünftige Beiträge dient. Er zeigt die wichtigsten Jekyll-Features und Markdown-Formatierungen."
---

# {{ page.title }}

Dies ist ein Template-Post für das Jekyll-Blog "Denken oder Denken Lassen". Dieser Beitrag dient als Vorlage und Referenz für zukünftige Posts.

## Front Matter Erklärung

Das Front Matter am Anfang jeder Jekyll-Post-Datei enthält wichtige Metadaten:

- `layout: post` - Verwendet das Post-Layout des Themes
- `title` - Der Titel des Posts
- `date` - Datum und Zeit der Veröffentlichung (Format: YYYY-MM-DD HH:MM:SS +TIMEZONE)
- `author` - Autor des Posts
- `categories` - Kategorien für die Organisation
- `tags` - Tags für bessere Auffindbarkeit
- `excerpt` - Kurze Zusammenfassung für Übersichtsseiten

## Markdown-Formatierung

### Überschriften

Verwende `#` für Überschriften verschiedener Ebenen:

```markdown
# Hauptüberschrift (H1)
## Unterüberschrift (H2)
### Weitere Unterüberschrift (H3)
```

### Text-Formatierung

- **Fett** mit `**Text**`
- *Kursiv* mit `*Text*`
- `Code` mit Backticks
- ~~Durchgestrichen~~ mit `~~Text~~`

### Listen

Ungeordnete Liste:
- Punkt 1
- Punkt 2
  - Unterpunkt
  - Weiterer Unterpunkt

Geordnete Liste:
1. Erster Punkt
2. Zweiter Punkt
3. Dritter Punkt

### Links und Bilder

[Link-Text](https://example.com)

Für Bilder:
```markdown
![Alt-Text](pfad/zum/bild.jpg)
```

### Code-Blöcke

Für Code-Beispiele:

```python
def beispiel_funktion():
    print("Hallo Welt!")
    return True
```

### Zitate

> Dies ist ein Zitat. Es kann verwendet werden, um wichtige Aussagen oder Zitate aus anderen Quellen hervorzuheben.

### Tabellen

| Spalte 1 | Spalte 2 | Spalte 3 |
|----------|----------|----------|
| Wert 1   | Wert 2   | Wert 3   |
| Wert 4   | Wert 5   | Wert 6   |

## Jekyll-spezifische Features

### Liquid-Tags

Jekyll verwendet Liquid für dynamische Inhalte:

- Aktuelles Datum: {{ site.time | date: "%d.%m.%Y" }}
- Autor: {{ page.author }}
- Kategorien: {{ page.categories | join: ", " }}

### Includes und Layouts

Posts verwenden automatisch das `post`-Layout. Für wiederverwendbare Inhalte können Includes verwendet werden.

## Datei-Namenskonvention

Jekyll-Posts müssen folgende Namenskonvention befolgen:
```
YYYY-MM-DD-titel-des-posts.md
```

Beispiele:
- `2025-07-08-mein-erster-post.md`
- `2025-07-15-ki-und-kreativitaet.md`
- `2025-08-01-experiment-ergebnisse.md`

## Kategorien und Tags

Verwende Kategorien für die Hauptthemen und Tags für spezifische Schlagwörter:

```yaml
categories: [ki, philosophie, experiment]
tags: [chatgpt, claude, denkprozess, automation]
```

## Tipps für gute Posts

1. **Aussagekräftige Titel** - Beschreibe klar, worum es geht
2. **Gute Struktur** - Verwende Überschriften zur Gliederung
3. **Excerpt verwenden** - Für bessere Übersichtsseiten
4. **Konsistente Kategorisierung** - Halte Kategorien und Tags einheitlich
5. **Datum beachten** - Posts werden chronologisch sortiert

## Fazit

Dieser Template-Post zeigt die wichtigsten Elemente eines Jekyll-Posts. Kopiere diese Datei als Ausgangspunkt für neue Beiträge und passe Inhalt, Titel, Datum und Metadaten entsprechend an.

---

*Erstellt am {{ page.date | date: "%d.%m.%Y um %H:%M Uhr" }}*
