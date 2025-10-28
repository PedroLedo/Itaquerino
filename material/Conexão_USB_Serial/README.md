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



<div align="center">
  
[![Download CH340 Driver](https://img.shields.io/badge/Baixar-Driver%20CH340-28a745?style=for-the-badge&logo=download)](https://bitabittecnologia.com.br/wp-content/uploads/2022/05/CH341SER_DRIVER.zip)

</div>

---
Após o download, descompacte o arquivo, conecte a placa no computador e execute o instalador como administrador. Esse passo é essencial para garantir que o driver seja instalado corretamente e que o sistema reconheça o dispositivo sem falhas.

<div align="center">
  <img src="https://github.com/user-attachments/assets/d9867847-abd6-4880-bf47-80358e56789a" alt="Texto alternativo" width="600">
</div>

---

<div align="center">
  <img src="https://github.com/user-attachments/assets/a46d4d75-529b-48b7-a7e8-ec75efa76f2e" width="600">
</div>

---
Durante a instalação, autorize o instalador a fazer modificações no seu computador. Essa permissão é necessária para que o driver seja corretamente configurado e integrado ao sistema operacional. Por fim, clique em "Install" para concluir o processo. Após essa etapa, o driver estará pronto para uso e sua placa poderá ser reconhecida corretamente pelo sistema.

<div align="center">
  <img src="https://github.com/user-attachments/assets/3a0b4934-9c11-45cf-a867-7224cd574461" width="600">
</div>

---

## 🔍 Verificando a instalação e a porta COM

Para confirmar se o processo foi concluído com sucesso e identificar em qual porta COM o Itaquerino está conectado:

Clique com o botão direito do mouse no ícone do Windows.

Selecione Gerenciador de Dispositivos.

Na lista, expanda a seção Portas (COM e LPT).

Verifique se o conversor aparece listado e observe o número da porta COM atribuída.

Essa informação será útil para configurar corretamente a comunicação com a placa durante a compilação.

<div align="center">
  <img src="https://github.com/user-attachments/assets/b6896d3b-2dd7-4fef-bf18-e64a1723e475" width="600">
</div>

---

No exemplo acima, a porta aparece como COM10, mas esse número pode variar dependendo da porta USB utilizada e do computador. O importante é identificar corretamente qual porta foi atribuída ao Itaquerino.

Com essa informação em mãos, você já pode abrir a Arduino IDE e configurar a porta correta para seguir com os próximos passos da programação.

---

## 🚀 Primeiro codigo - Blink

Para iniciar sua jornada com o Itaquerino, vamos realizar a primeira compilação utilizando o clássico exemplo do código Blink. Esse teste simples acende e apaga um LED em intervalos regulares, permitindo verificar se a placa está funcionando corretamente e se o ambiente de desenvolvimento está configurado adequadamente.

---
## 🛠️ Selecionando a porta COM na Arduino IDE

Com a Arduino IDE aberta, siga os passos abaixo para configurar a porta correta:

Clique no menu Tools (Ferramentas).

Vá até a opção Port (Porta).

Selecione a porta COM que foi identificada anteriormente no Gerenciador de Dispositivos.

Essa configuração é essencial para garantir que o código seja corretamente enviado à placa Itaquerino.

<div align="center">
  <img src="https://github.com/user-attachments/assets/37ab16a7-55be-4de7-8d87-9f9bde1bf2fb" width="600">
</div>

---
## 🔧 Selecionando o modelo de placa na Arduino IDE

Com a porta COM já configurada, o próximo passo é selecionar o modelo de placa correto. O Itaquerino utiliza o mesmo chip do Arduino Uno, o que o torna totalmente compatível com as definições padrão da IDE.

Para isso:

Acesse o menu Tools (Ferramentas).

Vá até Board (Placa).

Em Arduino AVR Boards, selecione Arduino Uno.

Essa configuração garante que o código seja compilado e enviado corretamente para a placa.

<div align="center">
  <img src="https://github.com/user-attachments/assets/3b2628e6-d8cf-4d8e-9b1a-f0ce0efcc621" width="600">
</div>

---

## 💡 Abrindo o exemplo Blink na Arduino IDE

Agora vamos utilizar o exemplo Blink para testar a comunicação com a placa. Para isso:

Com a Arduino IDE aberta, vá até o menu File (Arquivo).

Selecione Examples (Exemplos).

Acesse a pasta 01.Basics.

Clique em Blink.

Esse exemplo pisca um LED em intervalos regulares e é ideal para verificar se tudo está funcionando corretamente.


<div align="center">
  <img src="https://github.com/user-attachments/assets/bec5a7b6-9b71-4c2d-894c-a40d935abf50" width="600">
</div>

---

Com tudo configurado — porta COM e modelo de placa — basta compilar o código Blink e enviá-lo para a placa. Após a gravação, verifique se o LED está piscando conforme esperado. Isso confirma que a comunicação entre o computador e o Itaquerino está funcionando corretamente.

<div align="center">
  <img src="https://github.com/user-attachments/assets/08e96efc-547c-420d-b761-2c54b555255d" width="600">
</div>

---

## 🔄 Uso de gravador externo: atenção ao reset

Como estamos utilizando um gravador externo, é necessário pressionar o botão Reset da placa no exato momento em que o upload do código começa. Esse procedimento garante que o microcontrolador entre no modo de gravação e receba corretamente o programa enviado pela Arduino IDE.

Fique atento à barra de status da IDE para identificar o início do upload.

<div align="center">
  <img src="https://github.com/user-attachments/assets/4f7af79a-53d2-4299-b24a-52cbacefc09b" width="600">
</div>

Assim que a mensagem "Uploading..." aparecer na barra inferior da Arduino IDE, pressione imediatamente o botão Reset da placa. Esse passo é essencial para que o microcontrolador entre no modo de gravação e aceite o código enviado corretamente.
 
---

<div align="center">

[![Voltar ao Repositório Inicial](https://img.shields.io/badge/Voltar%20ao%20Reposit%C3%B3rio%20Inicial-blue?style=for-the-badge&logo=github)](https://github.com/PedroLedo/Itaquerino/tree/main)

</div>
