# 💻 Conexão via USB-TTL

A placa Itaquerino não possui gravador usb interno, portanto, é necessario utilizar um gravador externo, que neste caso é o com chip CH340.

<div align="center">
  <img src="https://github.com/user-attachments/assets/2de064fc-d060-4de1-8695-da79a4c40526" alt="Texto alternativo" width="600">
</div>

---

## 🛠️ 1. Conexões

## Ligações da placa Itaquerino com o conversor TTL

<div align="center">
  
| Itaquerino | Conversor |
|---|---|
| GND | GND |
| TXD | RXD |
| RXD | TXD |
| 5V | 5V |

</div>

---

Esta conexão permite tanto a compilação dos códigos quanto a alimentação da placa. No entanto, lembre-se: caso seu projeto exija uma corrente elevada, é altamente recomendável utilizar uma fonte de alimentação externa conectada ao borne da placa. Isso garante maior segurança e estabilidade no funcionamento do sistema.

<div align="center">
  <img src="https://github.com/user-attachments/assets/98dc0dda-41a2-4e1c-87cb-3221c90491b6" alt="Texto alternativo" width="600">
</div>

---
## 🚀 Instalação Driver CH340

Antes de tudo, para que o computador reconheça corretamente o conversor, é necessário realizar o download e a instalação do driver de comunicação. Esse passo é essencial para garantir que a interface entre o computador e a placa funcione de forma adequada durante a compilação e a transferência de dados.

---

<div align="center">
  
[![Download CH340 Driver](https://img.shields.io/badge/Baixar-Driver%20CH340-28a745?style=for-the-badge&logo=download)](https://bitabittecnologia.com.br/wp-content/uploads/2022/05/CH341SER_DRIVER.zip)

</div>

---

Para iniciar sua jornada com o Itaquerino, vamos realizar a primeira compilação utilizando o clássico exemplo do código Blink. Esse teste simples acende e apaga um LED em intervalos regulares, permitindo verificar se a placa está funcionando corretamente e se o ambiente de desenvolvimento está configurado adequadamente.

---
<div align="center">

[![Voltar ao Repositório Inicial](https://img.shields.io/badge/Voltar%20ao%20Reposit%C3%B3rio%20Inicial-blue?style=for-the-badge&logo=github)](https://github.com/PedroLedo/Itaquerino/tree/main)

</div>
