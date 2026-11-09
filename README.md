🌽 Raízes do Nordeste – Protótipo Front-end

Interface web responsiva para uma rede de lanchonetes de comida nordestina, criada como atividade da disciplina de Projeto Multidisciplinar (trilha Front-End). O trabalho parte do estudo de caso "Rede Raízes do Nordeste – Tecnologia, Tradição e Escala".

🔗 Demonstração online: https://matheus-maioqui.github.io/Raizes-Do-Nordeste-Uninter-Matheus/

📌 Sobre o projeto

A rede precisa vender bem em vários canais (App, Totem e Web) e manter a mesma experiência em cada unidade. Este protótipo mostra como seria essa experiência do lado do cliente: escolher onde comprar, montar o pedido, pagar, acompanhar o preparo e juntar pontos de fidelidade.

⚠️ Projeto acadêmico. Login, pedidos e pagamento são simulados no navegador. Não existe back-end, banco de dados nem cobrança real.

✨ O que dá para fazer
Área	Recursos
Unidade e cardápio	Escolher a unidade, ver o cardápio dela, buscar e filtrar produtos, ver promoções locais
Compra	Carrinho com ajuste de quantidade e remoção, checkout e escolha da forma de pagamento
Pagamento (simulado)	Retorno de aprovado, recusado ou erro, com proteção contra pagamento duplicado
Pedido	Acompanhamento: Pedido recebido → Em preparação → Pronto para retirada
Conta	Cadastro, login e perfil do cliente
Fidelidade	Pontos por compra aprovada e troca por recompensas
Privacidade	Consentimento LGPD no cadastro e preferências de marketing separadas

Caminho principal do usuário

Unidade → Cardápio → Carrinho → Checkout → Pagamento → Confirmação → Acompanhamento
⭐ Como funciona a fidelidade
Cada R$ 1,00 gasto vale 1 ponto (só a parte inteira conta).
Os pontos entram apenas em compras com pagamento aprovado e para clientes logados.
O saldo pode ser trocado por recompensas; sem saldo suficiente, o resgate é bloqueado.
🔐 Privacidade (LGPD)
O cadastro só é concluído com o consentimento para tratamento de dados.
O aceite de marketing é uma opção à parte, e o cliente pode mudá-la depois.
Os dados ficam no localStorage do navegador, apenas para fins de teste. Em um sistema real, tudo isso passaria por um servidor seguro.
📱 Responsividade

Foi usada a abordagem Mobile-first: o layout nasce para celular e se expande para telas maiores. No celular, o menu fica recolhido e abre ao toque.

🛠️ Tecnologias
HTML5 e CSS3
JavaScript (puro)
localStorage para guardar dados simulados
Git, GitHub e GitHub Pages
🗂️ Estrutura de pastas
Raizes-Do-Nordeste/
├── index.html      # página inicial
├── css/            # estilos
├── js/             # lógica da aplicação
└── pages/          # demais páginas
🧪 Cenários testados
Cardápio e promoções por unidade
Busca e filtros
Carrinho (adicionar, alterar, remover)
Cadastro, login e consentimento LGPD
Pagamento aprovado, recusado e com erro
Bloqueio de pagamento duplicado
Acúmulo e resgate de pontos
Layout em celular e em desktop
▶️ Como rodar localmente
# abra o index.html no navegador

Não é preciso instalar nada.

🚀 Próximos passos
Conectar a uma API real (cardápio, pedidos e login)
Integrar um gateway de pagamento
Criar telas para atendente, cozinha e gerente
Adaptar a interface para o totem de autoatendimento
Automatizar os testes
👤 Autor

Desenvolvido por [Matheus Leite Maioqui] · RU [4906124] · [Uninter]
