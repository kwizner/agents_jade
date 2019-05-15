# Uruchomienie

Aby uruchomić projekt należy poprawnie skonfigurować proces uruchamiania. W folderze doc znajdują się zrzuty ekranu zawierającą przykładową poprawną konfigurację.

## Main
<img src="/doc/configuration_1.PNG" height="200">
## Arguments
<img src="/doc/configuration_2.PNG" height="200">

# Zasada działania:

1. Jako pierwszy zostaje uruchomiony agent Simulation odpowiadający za start symulacji komunikacji agentów. Do jego zadania należy uruchomienie pozostałych agentów.
2. Następnie zostają uruchomieni agenci IMAgent, którzy nasłuchują wiadomości.
3. Zostaje uruchomiony agent IMMasterAgent, który co dany wyznaczony czas wysyła wiadomość pokolei do każdego z agentów.
4. IMAgent po otrzymaniu wiadomości wysyła odpowiedź.
5. IMMasterAgent po otrzymaniu odpowiedzi wysyła pozdrowienia.