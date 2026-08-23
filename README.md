# 🎵 Nokia Tune - ESP32-C3 Super Mini

Projeto que toca o clássico toque de mensagem da Nokia ao apertar um botão, exibindo uma mensagem personalizada em um display LCD I2C 16x2.

## 🛠️ Componentes utilizados

- ESP32-C3 Super Mini
- Buzzer passivo
- Botão (push button)
- Display LCD 16x2 com módulo I2C

## 🔌 Pinagem

| Componente | Pino |
|---|---|
| Buzzer     | GPIO 0 |
| Botão      | GPIO 4 |
| SDA (LCD)  | GPIO 8 |
| SCL (LCD)  | GPIO 9 |

## ⚙️ Funcionamento

Ao apertar o botão, o dispositivo:
1. Liga o display e mostra a mensagem "Ligacao" / "Julio";
2. Toca a melodia da Nokia Tune pelo buzzer;
3. Ao final, limpa e desliga o display novamente.

## 📚 Bibliotecas necessárias

- [`LiquidCrystal_I2C`](https://github.com/johnrickman/LiquidCrystal_I2C)
- `Wire.h` (nativa do Arduino/ESP32)
