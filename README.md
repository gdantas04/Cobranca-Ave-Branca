# Cobranca-Ave-Branca
Bot de Telegram que gerencia e realiza os pagamentos da mensalidade do Capítulo.


## Do que esse bot é capaz?
### Esse bot vai te lembrar de fazer seu pagamento 🕓
- Você receberá um aviso no dia 5 de cada mês falando que a mensalidade já pode ser paga;
- Caso você ainda não tenha pago, você receberá um aviso no dia 15 de cada mês alertando sobre o pagamento.

### Esse bot vai receber seus pagamentos 💶
- Através da API do Mercado Pago, o bot emitirá um código pix (válido por 5 minutos) que deve ser pago pelo usuário;
- Através da mesma API, será possível receber em tempo real a confirmação de pagamento;
- Caso você tenha mensalidades atrasadas, o bot irá cobrar a soma de todas as pendências. Não deixe acumular suas mensalidades.

### Esse bot se preocupa com seus dados 📊
- Para fins de segurança, o bot realiza backups do banco de dados todos os dias, às 18:00;
- Você não precisa compartilhar dados de cartões, o pagamento é feito via PIX;
- As informações armazenadas no banco de dados são as seguintes:
  - Nome completo;
  - Id de usuário do Telegram;
  - Detalhamento de cada mensalidade (pago ou não pago).
  
## Como usar? 🚀

### Comandos
#### Usuário comum 👤
- `/start`: faz seu cadastro, caso você não esteja no banco de dados;
- `/pendencias`: mostra quantas e quais mensalidades estão pendentes;
- `/pagar`: emite o código PIX válido por 5 minutos para que o usuário efetue o pagamento.

#### Conta da tesouraria 💰
- `/gestao`: mostra quantos membros estão cadastrados e quais membros estão com mensalidades pendentes;
- `/remove`: remove um usuário do banco de dados pelo ID do Telegram.
