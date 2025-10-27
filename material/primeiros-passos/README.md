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

![Texto alternativo](https://private-user-images.githubusercontent.com/91076859/506251394-1e169372-60b0-403b-9848-087504d9c52d.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjE2MDI4NDYsIm5iZiI6MTc2MTYwMjU0NiwicGF0aCI6Ii85MTA3Njg1OS81MDYyNTEzOTQtMWUxNjkzNzItNjBiMC00MDNiLTk4NDgtMDg3NTA0ZDljNTJkLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUxMDI3VDIyMDIyNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTM3OTI5NWYzZDAxMWY4NmE1N2M1ZWQ1MDA2NGQzZWM4ZTc2ZmI0ZTRmZTkzYTUxNzNmZjgxMDBjOWYwNDQzODAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.8OFImEAzhxmL0M3pYYClIbNie3yHTQKz_gNPyM_VEx4)

Contrato de Licença: Concorde com os termos da licença para continuar.

![Texto alternativo](https://private-user-images.githubusercontent.com/91076859/506251393-6212e216-7ffe-4a4d-978c-5c1347c724cb.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjE2MDI4NDYsIm5iZiI6MTc2MTYwMjU0NiwicGF0aCI6Ii85MTA3Njg1OS81MDYyNTEzOTMtNjIxMmUyMTYtN2ZmZS00YTRkLTk3OGMtNWMxMzQ3YzcyNGNiLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUxMDI3VDIyMDIyNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTU4MjhlNDU5M2RkMTRjOGVjZjE1ZTk4YjlmYmUzYWQ4ZTg5NjViNmFiMWYxNmZlOWUzNGRjMGI5NTAyN2Y1OTImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.MgEidRy1nE-17K91vZveg-SeH2alR7MvAt9D4NCwxc8)

Selecione para qual usuário deseja instalar.

![Texto alternativo](https://private-user-images.githubusercontent.com/91076859/506251392-bdc9e803-c355-4eaa-866e-6a9517a4d543.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjE2MDI4NDYsIm5iZiI6MTc2MTYwMjU0NiwicGF0aCI6Ii85MTA3Njg1OS81MDYyNTEzOTItYmRjOWU4MDMtYzM1NS00ZWFhLTg2NmUtNmE5NTE3YTRkNTQzLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUxMDI3VDIyMDIyNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTIxYWNjZWNiYzQ1ZDFhZDAwMzU1NjE5MDk1ZTYyZmQ5YWI3YzcxZjc2YjlmMzk5NDFiNDgyNzkyN2FlYTFkMjgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.owQXpR3sqUUaKPPrstJsORifbzQ3pXq1amzkVXSnHQQ)

Diretório de Instalação: Escolha onde o programa será instalado (o local padrão é geralmente a melhor opção) e clique em "Install".

![Texto alternativo](https://private-user-images.githubusercontent.com/91076859/506251392-bdc9e803-c355-4eaa-866e-6a9517a4d543.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjE2MDI4NDYsIm5iZiI6MTc2MTYwMjU0NiwicGF0aCI6Ii85MTA3Njg1OS81MDYyNTEzOTItYmRjOWU4MDMtYzM1NS00ZWFhLTg2NmUtNmE5NTE3YTRkNTQzLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUxMDI3VDIyMDIyNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTIxYWNjZWNiYzQ1ZDFhZDAwMzU1NjE5MDk1ZTYyZmQ5YWI3YzcxZjc2YjlmMzk5NDFiNDgyNzkyN2FlYTFkMjgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.owQXpR3sqUUaKPPrstJsORifbzQ3pXq1amzkVXSnHQQ)

Confirmação de Drivers: Durante o processo, o Windows pode pedir sua permissão para instalar os drivers da Arduino. Confirme e autorize todas as solicitações.

Finalização: Ao final, clique em "Close". A Arduino IDE estará instalada e um atalho terá sido criado na sua área de trabalho.

[![Voltar ao Repositório Inicial](https://img.shields.io/badge/Voltar%20ao%20Reposit%C3%B3rio%20Inicial-blue?style=for-the-badge&logo=github)](https://github.com/PedroLedo/Itaquerino/tree/main)

