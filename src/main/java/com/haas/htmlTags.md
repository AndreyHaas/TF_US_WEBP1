# 🏷️ **HTML-Tags – Vollständige Übersicht**

Hier ist eine strukturierte Sammlung der wichtigsten HTML-Tags nach Kategorien.

---

## 📄 **1. Grundgerüst**

| Tag | Beschreibung | Beispiel |
|-----|--------------|----------|
| `<!DOCTYPE html>` | Dokumenttyp (HTML5) | `<!DOCTYPE html>` |
| `<html>` | Wurzelelement | `<html lang="de">` |
| `<head>` | Metadaten, Titel, Styles | `<head>...</head>` |
| `<title>` | Titel im Browser-Tab | `<title>Meine Seite</title>` |
| `<body>` | Sichtbarer Inhalt | `<body>...</body>` |
| `<meta>` | Metadaten (Charset, Viewport) | `<meta charset="UTF-8">` |

---

## 📝 **2. Textformatierung**

| Tag | Beschreibung | Beispiel |
|-----|--------------|----------|
| `<h1>` bis `<h6>` | Überschriften | `<h1>Hauptüberschrift</h1>` |
| `<p>` | Absatz | `<p>Textabsatz</p>` |
| `<br>` | Zeilenumbruch | `Zeile 1<br>Zeile 2` |
| `<hr>` | Horizontale Linie | `<hr>` |
| `<strong>` | Wichtiger Text (fett) | `<strong>Achtung!</strong>` |
| `<b>` | Fett (optisch) | `<b>Fett</b>` |
| `<em>` | Betont (kursiv) | `<em>wichtig</em>` |
| `<i>` | Kursiv (optisch) | `<i>kursiv</i>` |
| `<mark>` | Markiert | `<mark>hervorgehoben</mark>` |
| `<small>` | Kleinerer Text | `<small>Kleingedrucktes</small>` |
| `<del>` | Durchgestrichen | `<del>alt</del>` |
| `<ins>` | Eingefügt (unterstrichen) | `<ins>neu</ins>` |
| `<sub>` | Tiefgestellt | `H<sub>2</sub>O` |
| `<sup>` | Hochgestellt | `E = mc<sup>2</sup>` |

---

## 🔗 **3. Links & Navigation**

| Tag | Beschreibung | Beispiel |
|-----|--------------|----------|
| `<a>` | Hyperlink | `<a href="https://example.com">Link</a>` |
| `<nav>` | Navigationsbereich | `<nav><a href="/">Start</a></nav>` |

**Wichtige Attribute:**
- `href` – Ziel-URL
- `target="_blank"` – in neuem Tab öffnen
- `rel="noopener"` – Sicherheit für `_blank`

---

## 🖼️ **4. Multimedia**

| Tag | Beschreibung | Beispiel |
|-----|--------------|----------|
| `<img>` | Bild | `<img src="bild.jpg" alt="Beschreibung">` |
| `<picture>` | Responsive Bilder | `<picture><source srcset="..."></picture>` |
| `<video>` | Video | `<video src="video.mp4" controls></video>` |
| `<audio>` | Audio | `<audio src="audio.mp3" controls></audio>` |
| `<figure>` | Medienelement mit Beschriftung | `<figure><img ...><figcaption>Text</figcaption></figure>` |
| `<figcaption>` | Bildunterschrift | `<figcaption>Bild 1</figcaption>` |

---

## 📋 **5. Listen**

| Tag | Beschreibung | Beispiel |
|-----|--------------|----------|
| `<ul>` | Ungeordnete Liste (Aufzählung) | `<ul><li>Punkt</li></ul>` |
| `<ol>` | Geordnete Liste (nummeriert) | `<ol><li>Erster</li></ol>` |
| `<li>` | Listenelement | `<li>Element</li>` |
| `<dl>` | Definitionsliste | `<dl><dt>Begriff</dt><dd>Definition</dd></dl>` |

---

## 📊 **6. Tabellen**

| Tag | Beschreibung | Beispiel |
|-----|--------------|----------|
| `表` | Tabelle | `表...表` |
| `<thead>` | Tabellenkopf | `<thead><tr><th>Name</th></tr></thead>` |
| `<tbody>` | Tabellenkörper | `<tbody><tr><td>Daten</td></tr></tbody>` |
| `<tfoot>` | Tabellenfuß | `<tfoot><tr><td>Summe</td></tr></tfoot>` |
| `<tr>` | Tabellenzeile | `<tr>...</tr>` |
| `<th>` | Tabellenkopfzelle | `<th>Überschrift</th>` |
| `<td>` | Tabellenzelle | `<td>Inhalt</td>` |
| `<caption>` | Tabellenüberschrift | `<caption>Tabelle 1</caption>` |

---

## 📦 **7. Container & Struktur**

| Tag | Beschreibung | Beispiel |
|-----|--------------|----------|
| `<div>` | Block-Container | `<div class="container">...</div>` |
| `<span>` | Inline-Container | `<span class="highlight">Text</span>` |
| `<header>` | Kopfbereich | `<header>Logo + Navigation</header>` |
| `<footer>` | Fußbereich | `<footer>Impressum</footer>` |
| `<main>` | Hauptinhalt | `<main>...</main>` |
| `<section>` | Abschnitt | `<section><h2>Überschrift</h2></section>` |
| `<article>` | Eigenständiger Beitrag | `<article><h3>Blogpost</h3></article>` |
| `<aside>` | Seitenleiste | `<aside>Werbung</aside>` |

---

## 🧾 **8. Formulare**

| Tag | Beschreibung | Beispiel |
|-----|--------------|----------|
| `<form>` | Formular | `<form action="/send" method="post">` |
| `<input>` | Eingabefeld | `<input type="text" name="name">` |
| `<textarea>` | Mehrzeiliges Textfeld | `<textarea rows="5"></textarea>` |
| `<button>` | Button | `<button type="submit">Senden</button>` |
| `<label>` | Beschriftung | `<label for="name">Name:</label>` |
| `<select>` | Dropdown | `<select><option>Option 1</option></select>` |
| `<option>` | Option im Dropdown | `<option value="1">Option 1</option>` |
| `<fieldset>` | Gruppe von Feldern | `<fieldset><legend>Adresse</legend>...</fieldset>` |
| `<legend>` | Gruppenüberschrift | `<legend>Persönliche Daten</legend>` |

**Wichtige `input`-Typen:**
- `text` – Text
- `password` – Passwort
- `email` – E-Mail
- `number` – Zahl
- `date` – Datum
- `checkbox` – Checkbox
- `radio` – Radio-Button
- `submit` – Absenden
- `reset` – Zurücksetzen

---

## 🎨 **9. Semantische Tags (HTML5)**

| Tag | Beschreibung |
|-----|--------------|
| `<header>` | Kopfbereich |
| `<nav>` | Navigation |
| `<main>` | Hauptinhalt |
| `<article>` | Eigenständiger Inhalt |
| `<section>` | Themenabschnitt |
| `<aside>` | Zusatzinformation |
| `<footer>` | Fußbereich |
| `<details>` | Ausklappbare Details |
| `<summary>` | Überschrift für Details |

---

## 📱 **10. Responsive & Metadaten**

| Tag | Beschreibung | Beispiel |
|-----|--------------|----------|
| `<meta viewport>` | Responsive Viewport | `<meta name="viewport" content="width=device-width, initial-scale=1">` |
| `<link>` | Externe Ressourcen | `<link rel="stylesheet" href="style.css">` |
| `<style>` | CSS im Dokument | `<style>body { color: red; }</style>` |
| `<script>` | JavaScript | `<script src="app.js"></script>` |
| `<noscript>` | Fallback ohne JS | `<noscript>JavaScript aktivieren</noscript>` |

---

## 💡 **11. Weitere nützliche Tags**

| Tag | Beschreibung |
|-----|--------------|
| `<iframe>` | Eingebettetes Dokument (z.B. YouTube) |
| `<canvas>` | Grafiken zeichnen mit JavaScript |
| `<svg>` | Vektorgrafiken |
| `<code>` | Code-Snippet |
| `<pre>` | Vorformatierter Text (z.B. Code) |
| `<blockquote>` | Längeres Zitat |
| `<q>` | Kurzes Zitat (inline) |
| `<abbr>` | Abkürzung | `<abbr title="Hypertext Markup Language">HTML</abbr>` |
| `<time>` | Datum/Uhrzeit | `<time datetime="2024-03-24">heute</time>` |
| `<progress>` | Fortschrittsbalken | `<progress value="70" max="100">70%</progress>` |

---

## ✅ **HTML5-Boilerplate (Startvorlage)**

```html
<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Meine Seite</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <nav>
    <ul>
      <li><a href="/">Start</a></li>
      <li><a href="/about">Über uns</a></li>
    </ul>
  </nav>
</header>
<main>
  <section>
    <h1>Willkommen</h1>
    <p>Inhalt...</p>
  </section>
</main>
<footer>
  <p>&copy; 2024 Meine Seite</p>
</footer>
<script src="script.js"></script>
</body>
</html>
```

---

## 🎯 **Zusammenfassung der wichtigsten Tags**

| Kategorie | Wichtigste Tags |
|-----------|-----------------|
| **Grundgerüst** | `<!DOCTYPE>`, `<html>`, `<head>`, `<body>` |
| **Text** | `<h1>`-`<h6>`, `<p>`, `<strong>`, `<em>` |
| **Links** | `<a>` |
| **Bilder** | `<img>` |
| **Listen** | `<ul>`, `<ol>`, `<li>` |
| **Tabellen** | `<table>`, `<tr>`, `<th>`, `<td>` |
| **Container** | `<div>`, `<span>`, `<header>`, `<main>`, `<footer>` |
| **Formulare** | `<form>`, `<input>`, `<button>` |

> **Merke:** Semantische Tags (`<header>`, `<nav>`, `<main>`) sind besser für SEO und Barrierefreiheit als generische `<div>`-Container! 🚀