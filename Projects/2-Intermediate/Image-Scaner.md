# Escâner de Imagem

**Nível:** 2-Intermediário

Crie um app para Android e iOS para encontrar números de telefone, e-mails e links de sites disponíveis em uma foto e depois organizá-los no app.

## Histórias de Usuário

-   [ ] O usuário pode clicar uma foto ou fazer upload de uma foto da galeria
-   [ ] O processamento é feito na imagem.
-   [ ] Se houver números de telefone, e-mails ou links da web presentes na imagem, eles são listados nos cards devidamente organizados.
-   [ ] Ao tocar nos detalhes, uma opção é fornecida para salvar como contato.
-   [ ] Histórico de resultados de busca é fornecido na visualização de lista

## Funcionalidades Bônus

-   [ ] Fornecer uma opção para adicionar tags para cada resultado de busca.
-   [ ] Adicionar funcionalidade de busca baseada em tags
-   [ ] Adicionar login e sincronizar resultados em múltiplos dispositivos.

## Links e Recursos Úteis

-   Use OCR do Google para ler texto da imagem carregada. https://cloud.google.com/vision/docs/ocr
-   Aplique regex para identificar o número de telefone, e-mails e links de sites no texto identificado pelo OCR.

## Projetos de Exemplo

- App Android para detecção de texto - https://github.com/alexzaitsev/ocr-google-vision