# webduino-flashing
Wgranie oprogramowanie ESPEasy do Webduino

potrzebujemy pobrać http://www.letscontrolit.com/downloads/ESPEasy_R120.zip

# Podłączenie przewodów webduino <-> USB UART

Potrzebny do tego celu jest USB UART oraz webduino i oprogramowanie pobrane z oficjalnej strony ESPeasy.

Webduino TX     <->     RX USB UART (komunikacja)
Webduino RX     <->     TX USB UART (komunikacja)
Webduino GND    <->     GND USB UART (masa -)
Webduino 3.3V   <->     3.3V USB UART (zasilanie 3.3V!)
Webduino GPIO0  <->     GND USB UART (to połączenie jest potrzebne do uruchomienia trybu flashowania)

Wszystko musi być podłączone przed włożeniem USB UART do komputera.

Po podłączeniu USB UART do komputera na Webduino tylko 1 raz mignie LED i zgaśnie.

# Flashowanie Webduino
Następnie uruchamiamy FlashESP8266.exe wybieramy port COM oraz firmware na dzień dzisiejszy jaki miałem to: ESPEasy_v2.0.0-dev12_normal_4096.bin
Klikamy FLASH i koniec czekamy do końca procesu i to wszystko. Odłączamy przewody podłączamy zasilanie poprzez USB do webduino i powinno wszystko działąć z nowym oprogramowaniem.

Po uruchomieniu webduino sprawdzamy czy rozgłasza nam sieć bezprzewodową ESPeasy_0 (coś takiego) podłączamy się do tej sieci hasłem configesp i konfigurujemy by podłączył się do naszej sieci domowej.

Reszty nie bedę opisywał bo jak ktoś chce flashować webduino to wie po co ;)


# Help Sources / pomocne źródła
źródło gdzie znalazłem pomoc :http://www.cnblogs.com/sjqlwy/p/smart_all_in_1.html
loading firmware: https://www.letscontrolit.com/wiki/index.php/ESPEasy#Loading_firmware
