# Radar Ultrassônico com Display OLED
## Descrição

Este projeto demonstra um radar ultrassônico utilizando um sensor HC-SR04 e um display OLED. O código proporciona uma visualização gráfica da função do sensor, exibindo a distância medida e representações gráficas de diferentes níveis de proximidade.

## Mapa de Pinos

Sensor HC-SR04
| Sensor HC-SR04     | ESP32 Pino |
| ------------------ | ---------- |
| - Trigger          | 18         |
| - Echo             | 19         |
| - VCC              | 5V         |
| - GND              | GND        |


Display OLED
| Display OLED       | ESP32 Pino |
| ------------------ | ---------- |
| - SCL (ou SCK)     | 21         |
| - SDA              | 22         |
| - VCC              | 3.3-5V     |
| - GND              | GND        |

## Diagrama

![Diagrama](https://github.com/alexxsouzaa/Radar_Ultrassonico/assets/132787362/230c82c2-278b-4742-a622-e2031d314222)

## Bibliotecas Utilizadas

- [UltraSonic_HC_SR04](https://github.com/alexxsouzaa/UltraSonic_HC_SR04)
- [U8g2](https://github.com/olikraus/u8g2)

## Licença

Este projeto é disponibilizado sob a [Licença MIT](LICENSE).

## Como Utilizar

1. Clone o repositório: `git clone https://github.com/alexxsouzaa/Radar_Ultrassonico.git`
2. Instale as bibliotecas necessárias (UltraSonic_HC_SR04 e U8g2).
3. Conecte o sensor HC-SR04 e o display OLED conforme o mapa de pinos.
4. Carregue o código para o seu ESP32.
5. Monitore as leituras de distância e a representação gráfica no display OLED.

