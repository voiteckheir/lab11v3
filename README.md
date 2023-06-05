# lab11v3

komenda do uruchomienia:
`docker compose up -d --build`

komenda do zatrzymania i usunięcia kontenerów:
`docker compose down`

Port 6666 jest domyślnie zastrzerzony
Odblokowanie portu 6666:
https://thegeekpage.com/err-unsafe-port/

wyświetlana strona:<br/>
![image](https://github.com/VoiteckHeira/lab11v3/assets/91530837/561b9ca7-d8a8-4b5d-ba6d-25802b5e57f9)


Reprezentacja graficzna <br/>
https://blog.baslijten.com/how-to-visualize-your-docker-composition/ <br/>
komendę odpalamy znajdując się w folderze z docker-compose.yml
komenda:<br/>
`
docker run --rm -it --name dcv -v ${PWD}:/input pmsipilot/docker-compose-viz render -m image docker-compose.yml --output-file=achmea.techday.png --force 
`
<br/>
wynik:<br/>
 ![tch_lab11_wizualizacja](https://github.com/VoiteckHeira/lab11v3/assets/91530837/efb7de20-fe80-4463-ba11-bd930e778cc9)