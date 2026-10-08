# Cafeteria

## Objetivos
1-Nome do caso de uso		FAZER O PEDIDO
identificador		AM-01
Ator   principal 		cliente
Ator   secundário 		vendedor
Resumo 		FAZER UM PEDIDO PELO APP
Pré-condição		"Fazer o login, identificar a comanda/mesa"
Pôs-condição		N.A.
Ação do Ator		Resposta do Sistema
1	Abrir o cardápio	
2	Seleciona o item no carrinho	
3	Escolhe o método de pagamento	
4		Compra finalizada
5		Envia o pedido para cozinha
2-Nome do caso de uso		CADASTRAR PRODUTO
identificador		AM-02
Ator   principal 		vendedor
Ator   secundário 		N.A.
Resumo 		Cadastrar o produto no cardápio
Pré-condição		Fazer o login
Pôs-condição		N.A.
Ação do Ator		Resposta do Sistema
1	Clicar no botão cadastrar	
2		"Nome do produto, categoria, preço"
3	Clicar em finalizar	
4		Salvando produto
3-Nome do caso de uso		REALIZAR O PAGAMENTO
identificador		AM-03
Ator   principal 		cliente
Ator   secundário 		N.A.
Resumo 		Cadastrar o produto no cardápio
Pré-condição		Fazer o login
Pôs-condição		N.A.
Ação do Ator		Resposta do Sistema
1	Clicar no botão cadastrar	
2		"Nome do produto, categoria, preço"
3	Clicar em finalizar	
4		Salvando produto

### Stack Tecnlógico
- Backend: PHP estruturado com sessões nativas
- Banco de dados: MySQL (PDO para segurança)
- Frontend: HTML5, PHP, CSS, Tailwind CSS

#### Regras de negócio (CORE)

<img width="958" height="551" alt="image" src="https://github.com/user-attachments/assets/e4d14719-306c-4c84-9e3f-624b9a458890" /> 


##### Regras Globais
- Use sempre PDO para conexão e queries no MySQL para evitar SQL Injections
- Mantenha o código limpo e comente apenas logicas complexas.
- Separe os arquivos de forma lógica: um arquivo para conexão com a base (bd.php) e scripts de backend isolados e views em HTML5/PHP, nunca faça o sistema como um monolito, deixe sempre separados todas as regras para facilitar os futuros upgrades.
 - Estilize as telas em Tailwind de forma responsiva priorizando o MobileFrist.
 - Retorne sempre as mensagens de erros de forma claras na interface para o usuário (TOAST)
 - sempre trate as mensagens de caixa de mensagens nativas do navegador em um MODAL
