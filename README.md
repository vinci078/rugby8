<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Rugby - Passione e Storia</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background-image: url('rugby.jpg'); /* Sostituisci con il percorso dell'immagine */
      background-size: cover;
      background-position: center;
      color: white;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
    }

    .main-container {
      position: relative;
      width: 80%; /* Distanza maggiore dai bordi */
      height: 80%; /* Maggiore altezza per evitare tagli */
      display: flex;
      justify-content: center;
      align-items: center;
      position: relative;
    }

    .central-title {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background-color: rgba(0, 0, 0, 0.6);
      color: white;
      padding: 20px 40px;
      border-radius: 15px;
      font-size: 28px;
      font-weight: bold;
      z-index: 1;
    }

    /* Le bolle sono ora più piccole e più distanti tra loro */
    .bubble {
      padding: 15px 25px;
      border-radius: 50%;
      text-decoration: none;
      color: white;
      font-weight: bold;
      text-align: center;
      width: 130px; /* Ridotto per evitare il taglio */
      height: 70px; /* Ridotto per evitare il taglio */
      display: flex;
      justify-content: center;
      align-items: center;
      position: absolute;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
      transition: box-shadow 0.3s ease, background-color 0.3s ease;
    }

    /* Distanza aumentata tra le bolle con un cerchio più grande */
    .bubble-1 { background-color: #C82333; transform: rotate(0deg) translateY(-250px); }
    .bubble-2 { background-color: #0056B3; transform: rotate(60deg) translateY(-250px); }
    .bubble-3 { background-color: #155724; transform: rotate(120deg) translateY(-250px); }
    .bubble-4 { background-color: #856404; transform: rotate(180deg) translateY(-250px); }
    .bubble-5 { background-color: #6C757D; transform: rotate(240deg) translateY(-250px); }
    .bubble-6 { background-color: #D63384; transform: rotate(300deg) translateY(-250px); }

    /* Rimuovo la rotazione per "Obiettivi Futuri" */
    .bubble-4 {
      transform: rotate(0deg) translateY(250px); /* Posiziona correttamente la bolla */
    }

    .bubble:hover {
      cursor: pointer;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.5); /* Ombra più intensa durante l'hover */
    }

    /* Media Query per dispositivi mobili e tablet */
    @media (max-width: 768px) {
      .main-container {
        width: 90%;
        height: 80%;
      }

      .bubble {
        width: 120px;
        height: 65px;
        font-size: 14px;
      }

      .central-title {
        font-size: 22px;
        padding: 12px 25px;
      }
    }

    @media (max-width: 480px) {
      .main-container {
        width: 100%;
        height: 60%;
      }

      .bubble {
        width: 110px;
        height: 60px;
        font-size: 12px;
      }

      .central-title {
        font-size: 18px;
        padding: 10px 20px;
      }
    }
  </style>
</head>
<body>
  <div class="main-container">
    <a href="storiadelrugby.html" class="bubble bubble-1">Storia del Rugby</a>
    <a href="regoleprincipali.html" class="bubble bubble-2">Regole Principali</a>
    <a href="miglioricampionati.html" class="bubble bubble-3">Migliori Campionati</a>
    <a href="obiettivifuturi.html" class="bubble bubble-4">Obiettivi Futuri</a>
    <a href="storiapersonale.html" class="bubble bubble-5">Storia Personale</a>
    <a href="valoridelrugby.html" class="bubble bubble-6">Valori del Rugby</a>
    <div class="central-title">Il Mondo del Rugby</div>
  </div>
</body>
</html>
