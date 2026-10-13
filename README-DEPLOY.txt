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
