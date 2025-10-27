# 🧭 Primeiros Passos

Bem-vindo(a) ao guia inicial da placa **Itaquerino**!

Aqui você encontrará instruções para:
- Instalar a IDE Arduino;
- Configurar o ambiente;
- Fazer o primeiro upload de código;
- Testar exemplos básicos.

---

⚙️ 1. Instalar a Arduino IDE

A Arduino IDE (Ambiente de Desenvolvimento Integrado) é o software que você usará para escrever o código, compilar e enviá-lo para a sua placa Itaquerino. A instalação é simples, mas requer atenção a alguns detalhes.
Primeiro, você precisa baixar o instalador correto para o seu sistema operacional a partir do site oficial.

<p align="center">
<a href="https://www.arduino.cc/en/software" target="_blank" title="Baixar Arduino IDE">
<img src="https://img.shields.io/badge/Arduino%20IDE-Download-00979D?style=for-the-badge&logo=arduino" alt="Baixar Arduino IDE"/>
</a>
</p>

Ao clicar no botão, você será direcionado para a página de downloads.
Procure pela Arduino IDE 2.x. Esta é a versão mais moderna, rápida e com recursos úteis como autocompletar código, o que facilita muito a programação.
O site geralmente detecta seu sistema operacional (Windows, macOS ou Linux) e sugere o download correto. Clique na opção correspondente para iniciar o download.

 Para Windows
Execute o Instalador: Após o download, você terá um arquivo .exe. Dê um duplo clique para iniciá-lo.

![Texto alternativo](https://github.com/PedroLedo/Itaquerino/issues/1#issue-3558794951)

Contrato de Licença: Concorde com os termos da licença para continuar.

![Texto alternativo](https://private-user-images.githubusercontent.com/91076859/506251393-6212e216-7ffe-4a4d-978c-5c1347c724cb.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjE2MDMyNzQsIm5iZiI6MTc2MTYwMjk3NCwicGF0aCI6Ii85MTA3Njg1OS81MDYyNTEzOTMtNjIxMmUyMTYtN2ZmZS00YTRkLTk3OGMtNWMxMzQ3YzcyNGNiLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUxMDI3VDIyMDkzNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU1NDhjZWI4MjY2NGQ0MWRlMTAyODc0OGUzZjc2YTUyZjczZDlkOGJjMDM1M2FhMGFmZTFjMWQzZGQ0M2ExNWYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.WSWXTb9uJghB21JN3vBEaNeEacNMHJKg6oB92ECdPZM)

Selecione para qual usuário deseja instalar.

![Texto alternativo](https://private-user-images.githubusercontent.com/91076859/506251390-07a69936-89b9-4f42-a03b-fea5b06e1649.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjE2MDMyNzQsIm5iZiI6MTc2MTYwMjk3NCwicGF0aCI6Ii85MTA3Njg1OS81MDYyNTEzOTAtMDdhNjk5MzYtODliOS00ZjQyLWEwM2ItZmVhNWIwNmUxNjQ5LmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUxMDI3VDIyMDkzNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU2YjA5NmYzNTJlMDFjYWJkM2ZlNmVjZmVjY2Q1MzQwNjAwYzEyOTJiOGE4MzFhOGU2NDM1NGYzZTEzN2FiYzQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.vjAx2mhkW6laxXC6iBoichYR22rzqE8vX5TP9hcvY4I)

Diretório de Instalação: Escolha onde o programa será instalado (o local padrão é geralmente a melhor opção) e clique em "Install".

![Texto alternativo](https://private-user-images.githubusercontent.com/91076859/506251392-bdc9e803-c355-4eaa-866e-6a9517a4d543.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjE2MDMyNzQsIm5iZiI6MTc2MTYwMjk3NCwicGF0aCI6Ii85MTA3Njg1OS81MDYyNTEzOTItYmRjOWU4MDMtYzM1NS00ZWFhLTg2NmUtNmE5NTE3YTRkNTQzLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUxMDI3VDIyMDkzNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWY1ZmM0NDJlODc4ZDk3OThlYjBmNWEyNTRkMDEwOTJhODkwMTJmYjFkOGVlYzZmZDc4NjM1ZDdkNjcxMDg4NGUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.chJh_zlyJC5OjYBuu7jlTQyhrU-XzlcKpyxGhA4Dw_4)

Confirmação de Drivers: Durante o processo, o Windows pode pedir sua permissão para instalar os drivers da Arduino. Confirme e autorize todas as solicitações.

Finalização: Ao final, clique em "Close". A Arduino IDE estará instalada e um atalho terá sido criado na sua área de trabalho.

[![Voltar ao Repositório Inicial](https://img.shields.io/badge/Voltar%20ao%20Reposit%C3%B3rio%20Inicial-blue?style=for-the-badge&logo=github)](https://github.com/PedroLedo/Itaquerino/tree/main)

