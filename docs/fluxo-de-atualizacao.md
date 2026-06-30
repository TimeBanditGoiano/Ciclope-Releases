# Fluxo De Atualização Do CICLOPE

Este repositório é a central pública de distribuição do CICLOPE.

O aplicativo instalado deverá consultar o arquivo `version.json`. Quando a versão informada nesse arquivo for maior que a versão instalada localmente, o CICLOPE poderá mostrar uma faixa de aviso dentro do programa.

Fluxo planejado:

1. O CICLOPE instalado lê `version.json`.
2. Se houver versão nova, mostra uma faixa de atualização disponível.
3. O usuário clica na faixa.
4. O CICLOPE baixa o instalador indicado em `download_url`.
5. O CICLOPE fecha o aplicativo atual.
6. O instalador substitui os arquivos do programa.
7. O CICLOPE abre novamente já atualizado.

Os dados do usuário ficam fora da pasta do programa, em `%LOCALAPPDATA%\\CICLOPE`, para não serem apagados durante atualizações.

Arquivos privados não devem ser publicados aqui.
