# Mercadinho Central

Aplicativo web instalável (PWA) para controle de clientes, compras fiado e pagamentos.

## Funcionalidades
- Cadastro e edição de clientes.
- Registro de compras fiado com vários produtos, quantidade, preço unitário, total automático e vencimento opcional.
- Controle de saldo por cliente e registro de pagamentos parciais ou totais.
- Comprovante de compra, recibo de pagamento, extrato individual e relatório geral por impressão/salvamento como PDF.
- Pesquisa de clientes e movimentações.
- Backup e restauração manual em JSON.
- Interface responsiva para celular e cache básico para uso offline após primeira abertura.

## Publicar
O repositório usa a branch `main`. Para GitHub Pages: Settings → Pages → Build and deployment → Deploy from a branch → `main` → `/ (root)` → Save. Aguarde a publicação e abra a URL apresentada pelo GitHub Pages.

## Dados e privacidade
A primeira versão salva os dados no `localStorage` do navegador neste aparelho. Os dados **não** são sincronizados automaticamente entre aparelhos ou navegadores. Exporte backups regularmente e mantenha-os em local seguro. Não é uma solução multiusuário nem um banco de dados centralizado. Para uso em vários celulares ou funcionários, será necessário adicionar autenticação e banco de dados remoto com regras de acesso.

## PDF
Os comprovantes abrem a janela de impressão do navegador. No Android, escolha a opção “Salvar como PDF” no diálogo de impressão, quando disponível.

## Testes recomendados
1. Cadastrar cliente.
2. Registrar compra com dois produtos e conferir o total.
3. Registrar pagamento parcial e conferir o saldo.
4. Gerar comprovante e extrato PDF.
5. Exportar um backup e testar a restauração em um ambiente de teste.
