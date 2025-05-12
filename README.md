<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Système de Détection de Niveau d’Eau</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
      line-height: 1.6;
    }
    h1, h2 {
      font-weight: bold;
      color: #2c3e50;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 20px 0;
    }
    th, td {
      border: 1px solid #444;
      padding: 10px;
      text-align: left;
    }
    th {
      background-color: #f0f0f0;
    }
    code {
      background-color: #eee;
      padding: 2px 4px;
      border-radius: 4px;
      font-size: 14px;
    }
  </style>
</head>
<body>

  <h1>Système de Détection de Niveau d’Eau</h1>

  <h2>Auteur</h2>
  <p><strong>Votre nom complet ici</strong></p>

  <h2>Description</h2>
  <p>Ce projet Arduino permet de surveiller le niveau d’eau à l’aide d’un capteur analogique. Selon le niveau détecté, des LED s’allument et un buzzer émet un signal sonore pour signaler un niveau critique.</p>

  <h2>Motivation</h2>
  <p>Ce système est utile pour éviter les débordements ou les niveaux d’eau trop bas dans des réservoirs domestiques ou agricoles.</p>

  <h2>Architecture</h2>
  <p>Le capteur analogique envoie les données à un Arduino UNO qui pilote trois LED (verte, jaune, rouge) et un buzzer selon le niveau mesuré.</p>

  <h2>Diagramme en Blocs</h2>
  <pre>
    Capteur d'eau (A0)
           |
           v
      Arduino UNO
     /     |     \
   LED   LED   LED
  Verte Jaune Rouge
           |
         Buzzer
  </pre>

  <h2>Schéma de câblage</h2>
  <p><em>Voir image ci-jointe dans le dossier du projet.</em></p>
  <img src="A_detailed_digital_illustration_depicts_an_Arduino.png" alt="Schéma de câblage" width="600">

  <h2>Composants</h2>
  <table>
    <tr>
      <th>Appareil</th>
      <th>Utilisation</th>
      <th>Prix</th>
    </tr>
    <tr>
      <td>Arduino UNO</td>
      <td>Microcontrôleur principal</td>
      <td>80 RON</td>
    </tr>
    <tr>
      <td>Buzzer actif</td>
      <td>Alarme sonore</td>
      <td>1.5 RON</td>
    </tr>
    <tr>
      <td>LEDs (x3)</td>
      <td>Indication visuelle (niveaux)</td>
      <td>1.5 RON</td>
    </tr>
    <tr>
      <td>Fils de connexion</td>
      <td>Connexions sur breadboard</td>
      <td>7 RON</td>
    </tr>
    <tr>
      <td>Breadboard</td>
      <td>Support de câblage</td>
      <td>10 RON</td>
    </tr>
  </table>

  <h2>Bibliothèques</h2>
  <table>
    <tr>
      <th>Bibliothèque</th>
      <th>Description</th>
      <th>Utilisation</th>
    </tr>
    <tr>
      <td><code>Arduino.h</code></td>
      <td>Fonctions de base pour Arduino</td>
      <td>Accès aux entrées/sorties</td>
    </tr>
    <tr>
      <td><code>tone(), noTone()</code></td>
      <td>Fonctions natives Arduino</td>
      <td>Générer des sons sur une broche</td>
    </tr>
  </table>

  <h2>Journal de développement</h2>
  <ul>
    <li>✅ Lecture du capteur analogique testée</li>
    <li>✅ Contrôle des LED selon les seuils</li>
    <li>✅ Alerte sonore fonctionnelle</li>
    <li>✅ Test physique sur breadboard</li>
    <li>🔜 Ajout d’un bouton de réinitialisation (facultatif)</li>
  </ul>

</body>
</html>



