# Projeto 02 — Semáforo Básico

Neste projeto, você vai montar um semáforo simples utilizando três LEDs (vermelho, amarelo e verde).  
O objetivo é entender como controlar múltiplos pinos digitais ao mesmo tempo e como criar sequências de tempo usando `delay()`.  

---

- Itaquerino  
- 3 LEDs (vermelho, amarelo e verde)  
- 3 resistores de 220 Ω  
- Jumpers  
- Protoboard  
- Adaptador TTL-USB (para gravação)

---

Para carregar o código no Itaquerino, é obrigatório realizar a ligação correta do adaptador TTL-USB.  
Conecte os pinos conforme indicado no esquema a seguir.

---

<div align="center">
  <img src="https://github.com/user-attachments/assets/98dc0dda-41a2-4e1c-87cb-3221c90491b6" alt="Texto alternativo" width="600">
</div>

---

Com o adaptador TTL já conectado, podemos seguir para a montagem da parte responsável pelo funcionamento do semáforo.

---

![Texto alternativo](https://github.com/user-attachments/assets/a5c9f414-80f6-4fc9-95bd-0590617c63c0)

---

Com o circuito montado, podemos seguir para a programação.  
O código completo está disponível abaixo.

```cpp

// Pinos dos LEDs
const int ledVerde = 4;
const int ledAmarelo = 3;
const int ledVermelho = 2;

void setup() {
  pinMode(ledVerde, OUTPUT);
  pinMode(ledAmarelo, OUTPUT);
  pinMode(ledVermelho, OUTPUT);
}

void loop() {
  // Verde aceso (carros podem passar)
  digitalWrite(ledVerde, HIGH);
  digitalWrite(ledAmarelo, LOW);
  digitalWrite(ledVermelho, LOW);
  delay(3000);

  // Amarelo aceso (atenção)
  digitalWrite(ledVerde, LOW);
  digitalWrite(ledAmarelo, HIGH);
  digitalWrite(ledVermelho, LOW);
  delay(1000);

  // Vermelho aceso (pare)
  digitalWrite(ledVerde, LOW);
  digitalWrite(ledAmarelo, LOW);
  digitalWrite(ledVermelho, HIGH);
  delay(3000);
}
```


---


## 📝 Explicação do Código do Semáforo

O programa controla três LEDs conectados aos pinos digitais 4, 3 e 2 do Itaquerino, simulando o funcionamento básico de um semáforo real.  
Cada LED representa uma fase do trânsito:

- **Verde (pino 4):** passagem liberada  
- **Amarelo (pino 3):** atenção  
- **Vermelho (pino 2):** parada obrigatória  

---

### **1. Definição dos pinos**

```cpp
const int ledVerde = 4;
const int ledAmarelo = 3;
const int ledVermelho = 2;
```
Essas variáveis indicam quais pinos do Itaquerino serão utilizados.
Usar const deixa o código organizado e evita alterações acidentais.

2. Configuração inicial
```cpp
void setup() {
  pinMode(ledVerde, OUTPUT);
  pinMode(ledAmarelo, OUTPUT);
  pinMode(ledVermelho, OUTPUT);
}
```
A função setup() roda apenas uma vez.
Aqui configuramos cada LED como saída, permitindo ao microcontrolador ligar ou desligar os pinos.

3. Funcionamento do semáforo
A lógica principal fica no loop(), que se repete continuamente.

🔹 Fase Verde
```cpp
digitalWrite(ledVerde, HIGH);
digitalWrite(ledAmarelo, LOW);
digitalWrite(ledVermelho, LOW);
delay(3000);
```
O LED verde acende por 3 segundos.

🔹 Fase Amarela
```cpp
digitalWrite(ledVerde, LOW);
digitalWrite(ledAmarelo, HIGH);
digitalWrite(ledVermelho, LOW);
delay(1000);
```
O LED amarelo acende por 1 segundo, indicando atenção.

🔹 Fase Vermelha
```cpp
digitalWrite(ledVerde, LOW);
digitalWrite(ledAmarelo, LOW);
digitalWrite(ledVermelho, HIGH);
delay(3000);
```
O LED vermelho acende por 3 segundos, simulando parada obrigatória.

🔄 Ciclo contínuo
Após a fase vermelha, o loop() recomeça automaticamente, repetindo todo o ciclo do semáforo.

