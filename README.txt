# Sistema Offline/Online (PWA + Firestore + LocalStorage)

Este projeto é um exemplo **offline-first**: os dados são salvos primeiro no **LocalStorage** 
e podem ser sincronizados depois com o **Firestore**.

## Como usar
1. Hospede os arquivos em um servidor estático (ou use uma extensão de servidor local).
2. Edite o `index.html` e coloque suas credenciais do Firebase (apiKey, projectId etc.).
3. Abra `index.html` no navegador (em HTTPS para instalar como PWA).
4. Cadastre dados. Eles ficam locais (⏳ Pendente).
5. Clique em **Sincronizar** para enviar ao Firestore (vira ✅ Sincronizado).

## Estrutura
- index.html — App principal (responsivo, cadastro/consulta/cards).
- manifest.json — Manifesto PWA (nome, ícones, cores).
- sw.js — Service Worker para cache offline.
- icon-192.png / icon-512.png — Ícones do PWA.

## Observações
- A coleção usada no Firestore é `cadastros`.
- Para editar/excluir, use os botões nos cards.
- Para instalar como aplicativo, acesse via HTTPS e aceite o prompt de instalação do navegador.

Bom uso!
