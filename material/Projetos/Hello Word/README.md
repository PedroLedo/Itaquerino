# Projeto 01 — Hello World (Blink + Serial)

Este primeiro projeto apresenta o funcionamento básico do Itaquerino:
Controlar um pino digital e enviar mensagens pelo Monitor Serial.
Como a placa não possui interface USB integrada, é obrigatório utilizar um adaptador TTL-USB para fazer a gravação e comunicação serial.

Materiais:

1. Itaquerino
2. Adaptador TTL-USB (CH340, FT232 ou equivalente)
3. Cabo USB
4. Jumpers macho–fêmea
5. Ligação do adaptador TTL-USB

Conexões recomendadas:

---

<div align="center">
  
| Itaquerino | Conversor |
|---|---|
| GND | GND |
| TXD | RXD |
| RXD | TXD |
| 5V | 5V |

</div>

---

Esta conexão permite tanto a compilação dos códigos quanto a alimentação da placa.

<div align="center">
  <img src="https://github.com/user-attachments/assets/98dc0dda-41a2-4e1c-87cb-3221c90491b6" alt="Texto alternativo" width="600">
</div>

---

Copie e cole na IDE do Arduino o codigo disponibilizado abaixo:

```cpp

void setup() {
  pinMode(13, OUTPUT);         // Configura o pino 13 como saída
  Serial.begin(9600);          // Inicia o Monitor Serial
  Serial.println("Hello, Itaquerino!");
}

void loop() {
  digitalWrite(13, HIGH);      // Liga o LED
  Serial.println("LED ON");
  delay(500);

  digitalWrite(13, LOW);       // Desliga o LED
  Serial.println("LED OFF");
  delay(500);
}

```

---

Como funciona:

setup() roda só uma vez, após o reset.

loop() roda repetidamente.

digitalWrite() altera o estado lógico do pino 13.

Serial.begin(9600) habilita o envio de dados para o computador via TTL.

As mensagens “LED ON/OFF” aparecem no Monitor Serial.

---

Erros comuns:

1. Inverter RX e TX.
2. Usar tensão errada (3.3V em placa que exige 5V).
3. Abrir o Monitor Serial em velocidade diferente de 9600 baud.
4. Usar adaptador sem DTR e não resetar a placa na hora certa para gravar.

---

## Desafios

1. Alterar a frequência do piscar.
2. Alternar entre dois LEDs externos.
3. Criar uma animação de piscadas.

---

<a href="./material/Projetos">
  <img src="https://img.shields.io/badge/📘%20Acessar%20Projetos-blue?style=for-the-badge" alt="Projetos">
</a>

---
