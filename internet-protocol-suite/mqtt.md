# MQTT

Message Queuing Telemetry Transport

## MQTT Compared to HTTP

Both HTTP and MQTT are based on TCP/IP

HTTP uses Request/Response \(1 to 1\)

MQTT uses Publish/Subscribe pattern \(1-to-1 or 1-to-many\)

HTTP is document centric, MQTT is data centric

HTTP is more complex than MQTT which is simple

MQTT message size is smaller, with only a 2 byte header

MQTT offers 3 Quality of Service \(QoS\) settings, with HTTP all messages get same level of service.

## Quality of service \(QoS\)

* 0 = 最多一次傳送（只負責傳送，發送過後就不管數據的傳送情況）
* 1 = 至少一次傳送（確認數據交付）
* 2 = 正好一次傳送（保證數據交付成功）

## MQTT Message Type

| **名稱** | **代表值** | **說明** |
| :--- | :--- | :--- |
| Reserved | 0 | 保留之後使用 |
| CONNECT | 1 | 發出連線請求 |
| CONNACK | 2 | 連線請求的ACK（確認符） |
| PUBLISH | 3 | 發佈訊息 |
| PUBACK | 4 | 發佈訊息ACK \(QoS 1\) |
| PUBREC | 5 | 已收到發佈訊息 \(QoS 2\) |
| PUBREL | 6 | 釋放發布訊息 \(QoS 2\) |
| PUBCOMP | 7 | 訊息發佈完成 \(QoS 2\) |
| SUBSCRIBE | 8 | 發出訂閱請求 |
| SUBACK | 9 | 請求訂閱的ACK |
| UNSUBSCRIBE | 10 | 發出取消訂閱請求 |
| UNSUBACK | 11 | 請求取消訂閱的ACK |
| PINGREQ | 12 | Ping請求 |
| PINGRESP | 13 | Ping回應 |
| DISCONNECT | 14 | 請求斷線 |
| Reserved | 15 | 保留之後使用 |

## Comparison of MQTT Implementations

[https://en.wikipedia.org/wiki/Comparison\_of\_MQTT\_Implementations](https://en.wikipedia.org/wiki/Comparison_of_MQTT_Implementations)

