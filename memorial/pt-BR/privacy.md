# Política de Privacidade do Virtual Memorial Space

**Data de vigência: 1º de novembro de 2026**

## 1. Introdução

O Virtual Memorial Space ("o App", "nós") é um app para iOS que permite criar espaços de homenagem privados, realizar rituais de lembrança e escrever cartas. Esta Política de Privacidade explica quais informações o App trata, onde elas ficam armazenadas e quais opções você tem.

O App não exige conta. Seu conteúdo de homenagem fica no seu dispositivo. Nosso servidor é usado apenas para as fichas de homenagem, fichas opcionais dentro do App usadas para estilos de oferenda mais especiais.

Ao usar o App, você reconhece que leu e entendeu esta Política de Privacidade.

## 2. Informações que não coletamos

O App não coleta nem solicita:

- Seu nome, e-mail, número de telefone ou qualquer conta de login
- Os nomes, fotos, datas, descrições, cartas ou mensagens dos seus espaços de homenagem
- Acesso a toda a sua biblioteca de fotos, à câmera, ao microfone, aos contatos ou à localização
- Os dados do seu cartão de pagamento
- Um identificador de publicidade (IDFA). O App não rastreia você em apps ou sites de outras empresas e não exibe o pedido de Transparência de Rastreamento de Apps (ATT).
- Dados analíticos ou eventos de uso. O App não contém nenhum SDK de análise nem publicidade.

## 3. Conteúdo de homenagem armazenado apenas no seu dispositivo

O seguinte é salvo no armazenamento privado do App no seu iPhone ou iPad:

- Espaços de homenagem: nome, tipo (por exemplo, um ente querido, parceiro, amigo ou pet), descrição, data de nascimento, data de lembrança, tema e configuração de lembrete
- As fotos que você adiciona a um espaço de homenagem
- Registros de rituais: qual vela, flor ou oferenda de papel foi usada, o número de fichas gastas, o horário e a mensagem que você adicionar
- As cartas que você escreve, incluindo rascunhos
- Preferências: idioma, efeitos reduzidos, se as oferendas de papel tradicionais são exibidas, se a introdução foi concluída, uma marcação de sincronização de compra pendente e um contador que limita os pedidos de avaliação
- O último saldo de fichas recebido do nosso servidor, usado apenas para exibição offline

Esse conteúdo não é enviado ao nosso servidor, não é usado para publicidade e não é usado em nenhum recurso ou treinamento de inteligência artificial (IA). Se o Backup do iCloud estiver ativado, o iOS pode incluir esses dados no backup do dispositivo, tratado pela Apple na sua Conta Apple. O App não tem sincronização em nuvem própria.

**Fotos.** Você escolhe as fotos pelo seletor de fotos do sistema. O App recebe apenas as fotos que você seleciona e não acessa toda a sua biblioteca de fotos. Uma cópia compactada de cada foto selecionada é salva no armazenamento do App.

## 4. Fichas de homenagem e nosso servidor

As fichas de homenagem são compras no app do tipo consumível. Para que seu saldo seja mantido depois de reinstalar o App, ele fica armazenado no nosso servidor ("appapi"), hospedado na Vercel, que guarda os dados no Vercel KV (Upstash Redis).

O servidor armazena apenas:

- Um ID de usuário gerado aleatoriamente, sem vínculo com seu nome, e-mail ou Conta Apple
- Um resumo (hash) do token de acesso emitido para esse ID de usuário. O token em si não é armazenado no servidor.
- Seu saldo de fichas
- Registros de compra: ID do produto, ID da transação Apple, número de fichas e horário
- Registros de gasto: ID da oferenda (por exemplo, um tipo de vela), número de fichas, a chave de solicitação que evita cobrança em dobro, saldo após o gasto e horário
- Um histórico de créditos, gastos e reembolsos com valores e IDs de transação ou de gasto relacionados

Cada solicitação ao servidor também inclui a versão do App e um identificador do dispositivo (o identifierForVendor do iOS), usados para verificar a assinatura da solicitação. Como em qualquer serviço web, nosso provedor de hospedagem pode tratar seu endereço IP em registros comuns de solicitações para fornecer e proteger o serviço.

O servidor não armazena seu nome, seu e-mail nem nada sobre as pessoas ou pets que você homenageia: nenhum nome, foto, carta ou mensagem de homenagem.

O ID de usuário e o token ficam armazenados nas Chaves do iOS no seu dispositivo. Eles podem ser sincronizados pelas Chaves do iCloud, para que o saldo fique disponível depois de reinstalar o App ou em outro dispositivo conectado à mesma Conta Apple.

## 5. Compras

- **Apple (App Store)** processa todos os pagamentos pela sua Conta Apple. Nunca recebemos os dados do seu cartão de pagamento. Política de privacidade da Apple: https://www.apple.com/legal/privacy/
- **RevenueCat** valida as transações. A RevenueCat recebe o ID de usuário aleatório citado acima, informações da transação (como ID do produto, ID da transação Apple e horário da compra) e informações técnicas básicas, como versão do App, versão do sistema operacional e país da App Store. Nosso servidor pede à RevenueCat que confirme as compras, e a RevenueCat avisa nosso servidor sobre compras e reembolsos, para que as fichas sejam creditadas uma única vez e retiradas após um reembolso. Política de privacidade da RevenueCat: https://www.revenuecat.com/privacy

As fichas de homenagem não têm valor monetário real. Os reembolsos são tratados pela Apple de acordo com as regras dela. Os termos de uso são o contrato de licença padrão da Apple: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. Notificações (opcionais)

Se você ativar um lembrete de data de lembrança para um espaço, o App pede permissão para notificações e agenda notificações locais no seu dispositivo. Os lembretes não passam pelo nosso servidor. Você pode desativá-los no App ou nos Ajustes do iOS.

## 7. Como usamos as informações

Usamos as informações acima apenas para:

- Exibir e guardar seus espaços de homenagem, rituais e cartas no seu dispositivo
- Criar sua carteira de fichas, creditar as fichas compradas uma única vez por transação, descontar fichas quando você escolhe uma oferenda premium e retirar fichas após um reembolso
- Verificar solicitações e evitar fraudes ou créditos duplicados
- Responder às suas solicitações de suporte

Não vendemos nem alugamos informações pessoais, não as usamos para publicidade e não criamos perfis de publicidade.

## 8. Compartilhamento

Só compartilhamos informações com os prestadores de serviço necessários para o funcionamento do App (Apple, RevenueCat e Vercel / Upstash para hospedagem e armazenamento), ou quando exigido por lei ou por processo legal válido.

## 9. Excluir seus dados

Nos Ajustes do App:

- **Apagar todos os dados (Delete All Data)** exclui todo o conteúdo de homenagem deste dispositivo: espaços de homenagem, fotos, registros de rituais, cartas e mensagens.
- **Apagar dados de fichas (Delete Token Data)** exclui sua carteira no nosso servidor: o registro do ID de usuário, o hash do token, o saldo, os registros de compra e de gasto e o histórico. Seu saldo vai a zero e não pode ser recuperado. Para impedir que a mesma compra seja creditada de novo, mantemos apenas o ID da transação Apple (com o ID do produto), sem o ID de usuário. Em seguida, o ID de usuário e o token também são removidos das suas Chaves.

Apagar o App remove o conteúdo local do dispositivo, mas **não** exclui sua carteira no nosso servidor. Para excluí-la, use "Apagar dados de fichas" antes de apagar o App ou entre em contato conosco. Dados locais excluídos podem continuar em backups anteriores do iCloud do dispositivo até que a Apple os substitua ou exclua.

Você também pode nos pedir para solicitar à RevenueCat a exclusão do registro de compra que ela mantém.

## 10. Segurança e retenção

As conexões com nosso servidor, com a Apple e com a RevenueCat usam HTTPS criptografado. As solicitações são assinadas, o servidor guarda apenas um hash do seu token e sua identidade fica nas Chaves do iOS. Nenhum método de armazenamento ou transmissão é totalmente seguro.

- O conteúdo local permanece até você excluí-lo ou apagar o App.
- Os dados da carteira no servidor permanecem até você usar "Apagar dados de fichas" ou nos pedir para excluí-los.
- IDs de transação Apple sem ID de usuário são mantidos para evitar créditos duplicados.
- A Apple e a RevenueCat mantêm registros de compra de acordo com suas próprias políticas e obrigações legais.

## 11. Privacidade de crianças

O Virtual Memorial Space não é direcionado a crianças. Não coletamos intencionalmente informações pessoais de crianças menores de 13 anos (ou da idade mínima exigida no seu país). Se você acredita que uma criança nos forneceu informações pessoais, entre em contato e nós as excluiremos.

## 12. Tratamento internacional

Nossos provedores de hospedagem e armazenamento e a RevenueCat podem tratar dados nos Estados Unidos ou em outros países diferentes do seu. Para esse tratamento, contamos com as salvaguardas desses provedores.

## 13. Seus direitos

Dependendo de onde você mora, você pode ter o direito de acessar, corrigir, excluir ou restringir o tratamento das suas informações pessoais. A maioria dos dados está no seu dispositivo e sob seu controle. Para os dados no nosso servidor, use "Apagar dados de fichas" ou entre em contato conosco. Podemos pedir informações que nos ajudem a localizar os registros relacionados.

## 14. Alterações nesta política

Podemos atualizar esta Política de Privacidade. A data no topo mudará quando isso acontecer. Se o App começar a coletar novos tipos de dados, atualizaremos esta política antes.

## 15. Fale conosco

Se tiver dúvidas sobre esta Política de Privacidade, entre em contato:

- E-mail: lpjustdoit@163.com

---

## Outros idiomas

- [English](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/en/privacy.md)
- [简体中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh/privacy.md)
- [繁體中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh-tw/privacy.md)
- [日本語](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ja/privacy.md)
- [한국어](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ko/privacy.md)
- [Deutsch](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/de/privacy.md)
- [Français](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/fr/privacy.md)
- [Español](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/es/privacy.md)
- [Italiano](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/it/privacy.md)
- [Português (Portugal)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-PT/privacy.md)
- [Português (Brasil)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-BR/privacy.md)
- [ไทย](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/th/privacy.md)
- [Tiếng Việt](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/vi/privacy.md)
- [Bahasa Indonesia](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/id/privacy.md)
- [Bahasa Melayu](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ms/privacy.md)
- [العربية](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ar/privacy.md)
