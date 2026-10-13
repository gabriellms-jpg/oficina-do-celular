OFICINA DO CELULAR — GESTÃO V9 FIREBASE

Esta versão é um PWA com Firebase Authentication e Cloud Firestore.

CONFIGURAÇÃO JÁ FEITA
- Projeto Firebase: oficinadocelular-gestao
- App Web registrado
- Login por e-mail/senha
- Firestore criado
- Os aparelhos são gravados por usuário em users/{uid}/aparelhos

PUBLICAÇÃO
1. Publique todos os arquivos desta pasta em um servidor HTTPS.
2. Abra o endereço HTTPS no Safari do iPhone.
3. Faça login com o usuário criado no Firebase Authentication.
4. Safari > Compartilhar > Adicionar à Tela de Início.

REGRAS DO FIRESTORE
O arquivo firestore.rules contém as regras recomendadas para esta versão.
No Firebase Console: Firestore Database > Regras > substitua as regras atuais pelo conteúdo desse arquivo e publique.

IMPORTANTE
A configuração web do Firebase fica no index.html porque este é um PWA estático. A apiKey do Firebase Web não é uma senha; a proteção dos dados é feita pelas regras do Firestore e pelo Firebase Authentication.


VERSÃO CORRIGIDA
- O botão "Testar Firebase" grava/lê/exclui um documento de diagnóstico.
- O botão Salvar agora grava primeiro no Firestore e só depois atualiza o armazenamento local.
- Erros do Firestore aparecem na tela com código e mensagem.
- Fotos são comprimidas para reduzir o risco do limite de 1 MiB por documento.
