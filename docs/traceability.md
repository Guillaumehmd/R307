*# Table de traçabilité des exigences

| REQ_ID | Description                                                                               | Module cible      | Test(s) associé(s)      |
|:------:|-------------------------------------------------------------------------------------------|-------------------|-------------------------|
| REQ_001| Initialiser l’UART à **57 600 bauds** en 8N1                                              | r307_driver.c     | test_uart_init          |
| REQ_002| Allumer la LED bleue du R307 pendant l’enrôlement                                         | r307_driver.c     | test_led_enroll         |
| REQ_003| Capturer une empreinte **en < 2 s**                                                       | main.c            | test_capture_time       |
| REQ_004| Rechercher une empreinte et retourner un **score**                                        | r307_driver.c     | test_search_score       |
| REQ_005| Retourner un **code d’erreur explicite** si aucune empreinte n’est détectée               | main.c            | test_error_no_finger    |
| REQ_006| La commande `--enroll` doit stocker l’empreinte sous un **ID libre ≤ 10**                 | gestion_id.c      | test_id_allocation      |
| REQ_007| Éteindre la LED automatiquement **après 5 s d’inactivité**                               | main.c            | test_led_timeout        |
| REQ_008| Afficher la **version logicielle** via l’option de ligne de commande `--version`          | main.c            | test_version_flag       |
