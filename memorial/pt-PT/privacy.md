# Política de Privacidade da Virtual Memorial Space

**Data de entrada em vigor: 1 de novembro de 2026**

## 1. Introdução

A Virtual Memorial Space ("a App", "nós") é uma app para iOS que permite criar espaços de homenagem privados, realizar rituais de lembrança e escrever cartas. Esta Política de Privacidade explica que informações a App trata, onde são guardadas e que opções tem ao seu dispor.

A App não exige conta. O seu conteúdo de homenagem fica no seu dispositivo. O nosso servidor é utilizado apenas para as fichas de homenagem, fichas opcionais dentro da App usadas para estilos de oferenda mais elaborados.

Ao utilizar a App, reconhece que leu e compreendeu esta Política de Privacidade.

## 2. Informações que não recolhemos

A App não recolhe nem pede:

- O seu nome, endereço de e-mail, número de telefone ou qualquer conta de início de sessão
- Os nomes, fotografias, datas, descrições, cartas ou mensagens dos seus espaços de homenagem
- Acesso a toda a sua fototeca, à câmara, ao microfone, aos contactos ou à localização
- Os dados do seu cartão de pagamento
- Um identificador de publicidade (IDFA). A App não o segue através de apps ou sites de outras empresas e não mostra o pedido de Transparência no rastreio de apps (ATT).
- Dados analíticos ou eventos de utilização. A App não contém qualquer SDK de análise nem publicidade.

## 3. Conteúdo de homenagem guardado apenas no seu dispositivo

O seguinte é guardado no armazenamento privado da App no seu iPhone ou iPad:

- Espaços de homenagem: nome, tipo (por exemplo, um ente querido, companheiro, amigo ou animal de estimação), descrição, data de nascimento, data de lembrança, tema e definição de lembrete
- As fotografias que adiciona a um espaço de homenagem
- Registos de rituais: que vela, flor ou oferenda de papel foi usada, o número de fichas gastas, a hora e a mensagem que acrescentar
- As cartas que escreve, incluindo rascunhos
- Preferências: idioma, efeitos reduzidos, se as oferendas de papel tradicionais são mostradas, se a introdução foi concluída, uma marca de sincronização de compra pendente e um contador que limita os pedidos de avaliação
- O último saldo de fichas recebido do nosso servidor, usado apenas para apresentação sem ligação

Este conteúdo não é enviado para o nosso servidor, não é usado para publicidade e não é usado em nenhuma funcionalidade nem treino de inteligência artificial (IA). Se a cópia de segurança do iCloud estiver ativada, o iOS pode incluir estes dados na cópia de segurança do dispositivo, tratada pela Apple no âmbito do seu ID Apple. A App não tem sincronização na nuvem própria.

**Fotografias.** Escolhe as fotografias através do seletor de fotografias do sistema. A App recebe apenas as fotografias que seleciona e não acede a toda a sua fototeca. É guardada uma cópia comprimida de cada fotografia selecionada no armazenamento da App.

## 4. Fichas de homenagem e o nosso servidor

As fichas de homenagem são compras na app do tipo consumível. Para que o saldo se mantenha depois de reinstalar a App, é guardado no nosso servidor ("appapi"), alojado na Vercel, que armazena os dados no Vercel KV (Upstash Redis).

O servidor guarda apenas:

- Um ID de utilizador gerado aleatoriamente, sem ligação ao seu nome, endereço de e-mail ou ID Apple
- Um resumo (hash) do token de acesso emitido para esse ID de utilizador. O token propriamente dito não é guardado no servidor.
- O seu saldo de fichas
- Registos de compra: ID do produto, ID da transação Apple, número de fichas e hora
- Registos de gasto: ID da oferenda (por exemplo, um tipo de vela), número de fichas, a chave de pedido que evita uma cobrança duplicada, saldo resultante e hora
- Um histórico de créditos, gastos e reembolsos com os respetivos montantes e IDs de transação ou de gasto relacionados

Cada pedido ao servidor inclui também a versão da App e um identificador do dispositivo (o identifierForVendor do iOS), usados para verificar a assinatura do pedido. Como em qualquer serviço web, o nosso fornecedor de alojamento pode tratar o seu endereço IP em registos habituais de pedidos para prestar e proteger o serviço.

O servidor não guarda o seu nome, o seu endereço de e-mail nem nada sobre as pessoas ou animais que recorda: nenhum nome, fotografia, carta ou mensagem de homenagem.

O ID de utilizador e o token são guardados no Porta-chaves do iOS do seu dispositivo. Podem ser sincronizados através do Porta-chaves do iCloud, para que o saldo fique disponível depois de reinstalar a App ou noutro dispositivo com o mesmo ID Apple.

## 5. Compras

- **Apple (App Store)** processa todos os pagamentos através do seu ID Apple. Nunca recebemos os dados do seu cartão de pagamento. Política de privacidade da Apple: https://www.apple.com/legal/privacy/
- **RevenueCat** valida as transações. A RevenueCat recebe o ID de utilizador aleatório acima, informações da transação (como ID do produto, ID da transação Apple e hora da compra) e informações técnicas básicas como a versão da App, a versão do sistema operativo e o país da App Store. O nosso servidor pede à RevenueCat que confirme as compras, e a RevenueCat notifica o nosso servidor de compras e reembolsos, para que as fichas sejam creditadas apenas uma vez e retiradas após um reembolso. Política de privacidade da RevenueCat: https://www.revenuecat.com/privacy

As fichas de homenagem não têm valor monetário real. Os reembolsos são tratados pela Apple segundo as suas regras. Os termos de utilização são o contrato de licença padrão da Apple: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. Notificações (opcionais)

Se ativar um lembrete de data de lembrança para um espaço, a App pede autorização para notificações e agenda notificações locais no seu dispositivo. Os lembretes não passam pelo nosso servidor. Pode desativá-los na App ou nas Definições do iOS.

## 7. Como utilizamos as informações

Utilizamos as informações acima apenas para:

- Mostrar e guardar os seus espaços de homenagem, rituais e cartas no seu dispositivo
- Criar a sua carteira de fichas, creditar as fichas compradas uma única vez por transação, descontar fichas quando escolhe uma oferenda premium e retirar fichas após um reembolso
- Verificar pedidos e evitar fraude ou créditos duplicados
- Responder aos seus pedidos de suporte

Não vendemos nem alugamos informações pessoais, não as usamos para publicidade e não criamos perfis publicitários.

## 8. Partilha

Só partilhamos informações com os prestadores de serviços necessários ao funcionamento da App (Apple, RevenueCat e Vercel / Upstash para alojamento e armazenamento), ou quando exigido por lei ou por um processo legal válido.

## 9. Eliminar os seus dados

Nas Definições da App:

- **Eliminar todos os dados (Delete All Data)** elimina todo o conteúdo de homenagem deste dispositivo: espaços de homenagem, fotografias, registos de rituais, cartas e mensagens.
- **Eliminar dados das fichas (Delete Token Data)** elimina a sua carteira no nosso servidor: o registo do ID de utilizador, o hash do token, o saldo, os registos de compra e de gasto e o histórico. O saldo passa a zero e não pode ser recuperado. Para impedir que a mesma compra seja creditada de novo, guardamos apenas o ID da transação Apple (com o respetivo ID do produto), sem o ID de utilizador. Depois, o ID de utilizador e o token são também removidos do seu Porta-chaves.

Eliminar a App remove o seu conteúdo local do dispositivo, mas **não** elimina a sua carteira no nosso servidor. Para a eliminar, use "Eliminar dados das fichas" antes de eliminar a App ou contacte-nos. Os dados locais eliminados podem permanecer em cópias de segurança anteriores do iCloud do dispositivo até a Apple as substituir ou eliminar.

Também nos pode pedir que solicitemos à RevenueCat a eliminação do registo de compra que esta guarda.

## 10. Segurança e conservação

As ligações ao nosso servidor, à Apple e à RevenueCat usam HTTPS cifrado. Os pedidos são assinados, o servidor guarda apenas um hash do seu token e a sua identidade fica no Porta-chaves do iOS. Nenhum método de armazenamento ou transmissão é totalmente seguro.

- O conteúdo local mantém-se até o eliminar ou eliminar a App.
- Os dados da carteira no servidor mantêm-se até usar "Eliminar dados das fichas" ou nos pedir que os eliminemos.
- Os IDs de transação Apple sem ID de utilizador são conservados para evitar créditos duplicados.
- A Apple e a RevenueCat conservam os registos de compra de acordo com as suas próprias políticas e obrigações legais.

## 11. Privacidade das crianças

A Virtual Memorial Space não se destina a crianças. Não recolhemos intencionalmente informações pessoais de crianças com menos de 13 anos (ou da idade mínima exigida no seu país). Se considerar que uma criança nos forneceu informações pessoais, contacte-nos e iremos eliminá-las.

## 12. Tratamento internacional

Os nossos fornecedores de alojamento e armazenamento e a RevenueCat podem tratar dados nos Estados Unidos ou noutros países que não o seu. Para esse tratamento, baseamo-nos nas salvaguardas destes fornecedores.

## 13. Os seus direitos

Consoante o local onde vive, pode ter direito a aceder, retificar, apagar ou limitar o tratamento das suas informações pessoais. A maioria dos dados está no seu dispositivo e sob o seu controlo. Para os dados no nosso servidor, use "Eliminar dados das fichas" ou contacte-nos. Poderemos pedir-lhe informações que nos ajudem a localizar os registos em causa.

## 14. Alterações a esta política

Podemos atualizar esta Política de Privacidade. A data no topo será alterada quando o fizermos. Se a App começar a recolher novos tipos de dados, atualizaremos primeiro esta política.

## 15. Contacto

Se tiver dúvidas sobre esta Política de Privacidade, contacte-nos:

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
