# fxcm-historical-data-bid

Исторические данные котировок брокера [FXCM](https://www.fxcm.com/) / [intrade.bar](https://intrade.bar/67204) (**только цена bid**)

### Список валютных пар

```
"EURUSD,USDJPY,GBPUSD,USDCHF,USDCAD,EURJPY,AUDUSD,NZDUSD,"
"EURGBP,EURCHF,AUDJPY,GBPJPY,CHFJPY,EURCAD,AUDCAD,CADJPY,"
"NZDJPY,AUDNZD,GBPAUD,EURAUD,GBPCHF,EURNZD,AUDCHF,GBPNZD,"
"GBPCAD,XAUUSD"
```
## Загрузка исторических данных

Для загрузки исторических данных необходимо запустить программу *bin/intrade-bar-downloader-XX.exe* через *bat-файл* *bin/run-intrade-bar-downloader-XX.bat* (XX - версия программы).
По умолчанию программа настроена на загрузку всех данных, кроме текущего дня. Ранее записанные данные не будут загружены, однако может быть обновлен последний день.

Программа *intrade-bar-downloader* скачивает котировки от [FXCM](https://www.fxcm.com/) и записывает их в формате *qhs5*. Все *qhs5-файлы* в данном репозитории расположены в папке *storage*. 
Рекомендую использовать данный репозиторий с загруженными историческими данными, так как программа *intrade-bar-downloader* всегда загружает максимально возможную историю, и **загрузка с полного нуля займет много времени**.

Более подробно про программу *intrade-bar-downloader* можно найти информацию в инструкции *bin/README.md*.
