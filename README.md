1) Wgrać kod na ESP z poziomu katalogu firmware (sprawdzić, czy w
ServerManager.hh ustawione są prawidłowe hasło i ssid do WiFi)
2) Zalogować się na EMQX
3) Zalogować się na InfluxDB
4) W InfluxDB wejść w dashboard "Monitoring hałasu"
5) W katalogu backend: sudo docker build -t iot-backend .
6) sudo docker run -d -p 8000:8000 --env-file .env --name moj-most-iot iot-backend
7) W katalogu frontend: firefox index.html
