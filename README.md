# Radar Ultrassônico com Display OLED para ESP32

<div align="center">
  <img src="https://github.com/alexxsouzaa/Radar_Ultrassonico_ESP32/assets/132787362/f621006f-db7d-4df4-ba98-3c5848ca72a2" alt="CAPA DO REPOSITORIO">
</div>

## Descrição

Este projeto demonstra um radar ultrassônico utilizando um sensor HC-SR04 e um display OLED com o ESP32. O código proporciona uma visualização gráfica da função do sensor, exibindo a distância medida e representações gráficas de diferentes níveis de proximidade.

## Requisitos

Antes de utilizar este projeto, certifique-se de ter os seguintes componentes:

- Sensor HC-SR04
- Display OLED de 1.3 ou 0.96 polegadas

## Mapa de Pinos

### Sensor HC-SR04
| Sensor | ESP32 Pino |
| -------------- | ---------- |
| - Trigger      | 18         |
| - Echo         | 19         |
| - VCC          | 5V         |
| - GND          | GND        |

### Display OLED
| Display  | ESP32 Pino |
| ------------  | ---------- |
| - SCL (ou SCK)| 21         |
| - SDA         | 22         |
| - VCC         | 3.3-5V     |
| - GND         | GND        |

Certifique-se de conectar os pinos corretamente conforme indicado na tabela para garantir o funcionamento adequado do sensor HC-SR04 e do display OLED.

## Diagrama

![Diagrama](https://github.com/alexxsouzaa/Radar_Ultrassonico/assets/132787362/230c82c2-278b-4742-a622-e2031d314222)

## Configurando o Display OLED

O código disponibilizado suporta dois drivers de display OLED, dependendo do modelo que você está utilizando. É crucial escolher o driver correto para garantir que o display funcione corretamente. Abaixo estão os dois drivers suportados:

```cpp
U8G2_SH1106_128X64_NONAME_F_HW_I2C u8g2(U8G2_R0, U8X8_PIN_NONE); // Driver do display OLED de 1.3 Polegadas
OU
U8G2_SSD1306_128X64_NONAME_F_HW_I2C u8g2(U8G2_R0, /* reset=*/ U8X8_PIN_NONE, /* clock=*/ SCL, /* data=*/ SDA); // Driver do display OLED de 0.96 Polegadas
```

## Bibliotecas Utilizadas

- [UltraSonic_HC_SR04](https://github.com/alexxsouzaa/UltraSonic_HC_SR04)
- [U8g2](https://github.com/olikraus/u8g2)

## Licença

Este projeto é licenciado sob a licença [MIT](https://github.com/alexxsouzaa/Radar_Ultrassonico/blob/main/LICENSE), o que significa que você é livre para utilizá-lo e modificar o código conforme necessário. Consulte o arquivo de licença para obter mais detalhes.

## Como Utilizar

1. Clone o repositório: `git clone https://github.com/alexxsouzaa/Radar_Ultrassonico.git`
2. Instale as bibliotecas necessárias (UltraSonic_HC_SR04 e U8g2).
3. Conecte o sensor HC-SR04 e o display OLED conforme o mapa de pinos.
4. Carregue o código para o seu ESP32.
5. Monitore as leituras de distância e a representação gráfica no display OLED.

