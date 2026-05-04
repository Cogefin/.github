# Cogefin : Code Generator For Iot Network


MQTTを用いるIoTネットワークとそれを用いるクラウドアプリケーションの構築を容易にするための
プログラムやプログラムジェネレーターを集めたOrganization.


## [MQTT_Sensor_Generator](https://github.com/Cogefin/MQTT_Sensor_Generator)
MQTTを用いるIoTネットワークに接続するためのセンサ端末をノーコードで試作するためのプログラム生成環境．
対象のハードウェアはARMをコアに採用したMCUやESP32を採用したArduino．

## [MQTT_Sensor_Watch](https://github.com/Cogefin/MQTT_Sensor_Watch)
上記[MQTT_Sensor_Generator](https://github.com/Cogefin/MQTT_Sensor_Generator)で生成されたプログラムで動作するセンサ端末がMQTTブローカーに
送信しているセンサデータを収集し加工した上で，Google spreadsheetやArduino Cloudに中継(アップロード)する機能や，ローカルのファイル(CSVやSQLite)に保存し，JavaScriptで可視化するHTMLをノーコードで生成するプログラム．

## [MQTT_Actuator_Control_Utility](https://github.com/Cogefin/MQTT_Actuator_Control_Utility)
MQTTを用いるIoTネットワークに接続したアクチュエータ端末を制御するMQTTメッセージを送信するためのアプリケーションで，制御コマンドと待ち時間を組み合わせたシナリオファイルに従って，MQTTブローカーにメッセージを送る．


## [MQTT_Actuator_Generator](https://github.com/Cogefin/MQTT_Actuator_Generator)
MQTTを用いるIoTネットワークに接続する，アクチュエータ端末をノーコードで試作するためのプログラム生成環境．
対象のハードウェアはARMをコアに採用したMCUやESP32を採用したArduino．

## [CogefinActuatorHAL](https://github.com/Cogefin/CogefinActuatorHAL)
アクチュエータを構成するIC等のハードウェア用デバイスドライバ(Arduinoにおけるライブラリ)のAPIは統一されていないため，同じ種類のデバイスであっても，機種や型番が異なると
プログラムの大幅な変更が必要になることはめずらしくない．この問題を軽減するため，デバイスの種類ごとに統一したAPIを実現するためのハードウェアアブストラクション層．

