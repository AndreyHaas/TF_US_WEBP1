# 🌐 **Grundlagen HTML / CSS / PHP – Einfach & Verständlich**

## 📖 **Inhaltsverzeichnis**

1. [Was ist HTML?](#1-was-ist-html)
2. [Was ist CSS?](#2-was-ist-css)
3. [Was ist PHP?](#3-was-ist-php)
4. [HTML – Die Struktur einer Webseite](#4-html--die-struktur-einer-webseite)
5. [CSS – Das Design](#5-css--das-design)
6. [PHP – Dynamik auf dem Server](#6-php--dynamik-auf-dem-server)
7. [Zusammenarbeit: HTML + CSS + PHP](#7-zusammenarbeit-html--css--php)
8. [Wichtige Befehle im Überblick](#8-wichtige-befehle-im-überblick)
9. [Häufige Fehler & Tipps](#9-häufige-fehler--tipps)

---

## 1. Was ist HTML?

**HTML** = **Hypertext Markup Language**  
Das ist die **Grundstruktur** jeder Webseite. Man kann es mit dem **Skelett** eines Hauses
vergleichen.

```html
<!DOCTYPE html>
<html lang="de">
<head>
  <title>Meine erste Seite</title>
</head>
<body>
<h1>Hallo Welt!</h1>
<p>Das ist meine erste Webseite.</p>
</body>
</html>
```

**Aufgabe von HTML:**

- Strukturieren: Überschriften, Absätze, Listen, Tabellen
- Inhalte einfügen: Text, Bilder, Videos, Links
- Semantik: Bedeutung von Inhalten festlegen

---

## 2. Was ist CSS?

**CSS** = **Cascading Style Sheets**  
Das ist die **Gestaltung** der Webseite – wie **Farbe, Größe, Anordnung**.

```css
/* style.css */
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
}

h1 {
    color: blue;
    font-size: 24px;
}

p {
    color: #333;
    line-height: 1.5;
}
```

**Aufgabe von CSS:**

- Farben, Schriftarten, Hintergründe
- Layout (Positionierung, Abstände)
- Responsive Design (für Handy, Tablet, PC)

---

## 3. Was ist PHP?

**PHP** = **PHP: Hypertext Preprocessor**  
Das ist eine **Serversprache** – sie erzeugt **dynamische Inhalte**.

```php
<?php
$name = "Anna";
$alter = 25;

echo "<p>Hallo $name, du bist $alter Jahre alt.</p>";
?>
```

**Aufgabe von PHP:**

- Daten aus Formularen empfangen
- Mit Datenbanken verbinden (MySQL)
- Benutzer-spezifische Inhalte anzeigen
- Login-Systeme, Warenkörbe, etc.

> 💡 **Wichtig:** PHP läuft **auf dem Server**, nicht im Browser!  
> Der Benutzer sieht nur das **Ergebnis** (HTML).

---

## 4. HTML – Die Struktur einer Webseite

### 📄 **Grundgerüst**

```html
<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Meine Seite</title>
</head>
<body>
<!-- Hier kommt der sichtbare Inhalt -->
</body>
</html>
```

### 🏷️ **Wichtige HTML-Tags**

| Tag                              | Bedeutung            | Beispiel                                  |
|----------------------------------|----------------------|-------------------------------------------|
| `<h1>` bis `<h6>`                | Überschriften        | `<h1>Titel</h1>`                          |
| `<p>`                            | Absatz               | `<p>Text</p>`                             |
| `<a>`                            | Link                 | `<a href="https://example.com">Link</a>`  |
| `<img>`                          | Bild                 | `<img src="bild.jpg" alt="Beschreibung">` |
| `<ul>`, `<ol>`, `<li>`           | Listen               | `<ul><li>Punkt</li></ul>`                 |
| `<div>`                          | Container (Block)    | `<div class="container">`                 |
| `<span>`                         | Container (Inline)   | `<span class="highlight">`                |
| `<header>`, `<main>`, `<footer>` | Semantische Struktur | –                                         |

---

## 5. CSS – Das Design

### 🔗 **CSS einbinden**

**1. Externe Datei (empfohlen):**

```html

<link rel="stylesheet" href="style.css">
```

**2. Im <head> (intern):**

```html

<style>
  body { background: lightblue; }
</style>
```

**3. Direkt am Element (Inline – nur für Ausnahmen):**

```html
<p style="color: red;">Text</p>
```

### 🎨 **CSS-Selektoren**

```css
/* 1. Element-Selektor */
p { color: black; }

/* 2. Klassen-Selektor (.className) */
.artikel { font-size: 16px; }

/* 3. ID-Selektor (#idName) */
#kopf { background: gray; }

/* 4. Kombiniert */
div.artikel p { margin: 0; }
```

### 📦 **Box-Modell**

```
┌─────────────────────────────┐
│         MARGIN              │
│  ┌───────────────────────┐  │
│  │       BORDER          │  │
│  │  ┌─────────────────┐  │  │
│  │  │    PADDING      │  │  │
│  │  │  ┌───────────┐  │  │  │
│  │  │  │  CONTENT  │  │  │  │
│  │  │  └───────────┘  │  │  │
│  │  └─────────────────┘  │  │
│  └───────────────────────┘  │
└─────────────────────────────┘
```

---

## 6. PHP – Dynamik auf dem Server

### 🧩 **PHP-Code in HTML einbetten**

```php
<!DOCTYPE html>
<html>
<body>
    <h1>Willkommen</h1>
    <p>Heute ist <?php echo date("d.m.Y"); ?></p>
</body>
</html>
```

### 📥 **Formular verarbeiten**

**HTML-Formular (form.html):**

```html

<form action="verarbeitung.php" method="post">
  <input type="text" name="name">
  <input type="submit" value="Absenden">
</form>
```

**PHP-Verarbeitung (verarbeitung.php):**

```php
<?php
$name = $_POST['name'];
echo "<p>Hallo, $name!</p>";
?>
```

### 🔁 **Wichtige PHP-Konzepte**

| Konzept       | Beispiel                                       |
|---------------|------------------------------------------------|
| **Variable**  | `$name = "Anna";`                              |
| **Bedingung** | `if ($alter > 18) { ... }`                     |
| **Schleife**  | `for ($i = 0; $i < 5; $i++) { ... }`           |
| **Array**     | `$farben = ["rot", "grün", "blau"];`           |
| **Funktion**  | `function summe($a, $b) { return $a + $b; }`   |
| **Session**   | `session_start(); $_SESSION['user'] = "Anna";` |
| **Datenbank** | `mysqli_query($conn, "SELECT ...");`           |

---

## 7. Zusammenarbeit: HTML + CSS + PHP

### 📁 **Typische Projektstruktur**

```
meinprojekt/
├── index.php
├── style.css
├── img/
│   └── logo.png
└── inc/
    ├── header.php
    └── footer.php
```

### 🔧 **Beispiel: Alles zusammen**

**index.php**

```php
<?php include 'inc/header.php'; ?>

<main>
    <h1>Willkommen <?php echo $_SESSION['name'] ?? 'Gast'; ?></h1>
    
    <div class="produkte">
        <?php
        $produkte = ["Laptop", "Maus", "Tastatur"];
        foreach ($produkte as $produkt) {
            echo "<div class='produkt'>$produkt</div>";
        }
        ?>
    </div>
</main>

<?php include 'inc/footer.php'; ?>
```

**style.css**

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 20px;
    background: #f5f5f5;
}

.produkte {
    display: flex;
    gap: 20px;
}

.produkt {
    background: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}
```

---

## 8. Wichtige Befehle im Überblick

### 📄 **HTML**

```html
<a href="...">Link</a>
<img src="..." alt="...">
<ul>
  <li>Liste</li>
</ul>
<div class="...">Container</div>
```

### 🎨 **CSS**

```css
farbe: color: red;
hintergrund: background: #fff;
schriftgröße: font-size: 16px;
rand: border: 1px solid black;
abstand innen: padding: 10px;
abstand außen: margin: 10px;
```

### 🐘 **PHP**

```php
<?php echo "Hallo"; ?>          // Ausgabe
$var = "Wert";                   // Variable
if ($x > 0) { ... }              // Bedingung
foreach ($array as $item) { ... } // Schleife
$_POST['name']                   // Formular-Daten
$_SESSION['user']                // Session-Daten
include "datei.php";             // Datei einbinden
```

---

## 9. Häufige Fehler & Tipps

### ❌ **Häufige Fehler**

| Fehler                                   | Lösung                                                    |
|------------------------------------------|-----------------------------------------------------------|
| `<?` statt `<?php`                       | Immer `<?php` verwenden (kurze Tags sind oft deaktiviert) |
| Vergessenes `;` am Ende                  | Jede PHP-Anweisung endet mit `;`                          |
| Falscher Dateipfad bei `src` oder `href` | Relativen Pfad prüfen (`img/bild.jpg`, nicht `C:\...`)    |
| CSS-Datei nicht geladen                  | `<link>`-Tag im `<head>` prüfen                           |
| `$_POST` leer                            | `method="post"` im Formular gesetzt?                      |

### ✅ **Tipps für den Einstieg**

1. **Immer mit HTML beginnen** – die Struktur muss stimmen
2. **CSS zuerst mit Klassen** – nicht zu viele IDs
3. **PHP-Fehler anzeigen lassen:**
   ```php
   error_reporting(E_ALL);
   ini_set('display_errors', 1);
   ```
4. **Localhost verwenden** – z.B. XAMPP, MAMP, WAMP
5. **Dateierweiterungen:**
    - Nur HTML → `.html`
    - Mit PHP → `.php`

---

## 🎯 **Zusammenfassung**

| Sprache  | Aufgabe                   | Wo läuft? |
|----------|---------------------------|-----------|
| **HTML** | Struktur                  | Browser   |
| **CSS**  | Design                    | Browser   |
| **PHP**  | Dynamik, Logik, Datenbank | Server    |

> **Merke:**  
> HTML = Skelett  
> CSS = Kleidung  
> PHP = Gehirn (denkt nach und berechnet)

---

## 🚀 **Nächste Schritte**

- [ ] Eigene Seite mit HTML bauen
- [ ] Mit CSS gestalten
- [ ] PHP-Formulare verarbeiten
- [ ] Mit MySQL Datenbank verbinden
- [ ] Ein kleines Projekt: Kontaktformular, Gästebuch, Login

**Viel Erfolg beim Coden!** 💻😊