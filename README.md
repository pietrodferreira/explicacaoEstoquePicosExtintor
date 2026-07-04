```
# Módulo de Estoque

## 1. Escopo do Módulo

O módulo de Estoque foi feito para controlar os produtos e a disponibilidade de itens em cada filial da empresa. Ele ajuda a acompanhar o que tem em estoque de forma mais prática, identificar produtos que estão acabando, registrar todas as movimentações e gerar relatórios quando necessário.

As principais seções são:

- **Visualização**: Mostra um resumo geral do estoque por filial, com totais, quantidade disponível, itens cheios, itens vazios, produtos em alerta e itens zerados. É útil para ver rapidamente o que precisa de atenção.
- **Cadastro/Edição**: Aqui dá para cadastrar novos produtos, definir preço, peso, filial de destino e quantidade inicial. Também permite editar as informações e ajustar o estoque manualmente em cada filial.
- **Movimentação de Entradas/Saídas**: Registra todo o histórico de mudanças no estoque — entradas, saídas e transferências entre filiais. Dá uma boa visão do fluxo ao longo do tempo.
- **Relatório em PDF**: Gera um relatório consolidado do estoque, destacando os itens que estão acabando ou zerados, e permite exportar para imprimir ou compartilhar.

## 2. Instalação Rápida

1. Entre na pasta do projeto.
2. Crie o ambiente virtual:
   ```bash
   python -m venv .venv
   ```
3. Ative o ambiente:
   - No Linux ou macOS: `source .venv/bin/activate`
   - No Windows: `.venv\Scripts\activate`
4. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
5. Rode as migrações:
   ```bash
   python manage.py migrate
   ```
6. Inicie o servidor:
   ```bash
   python manage.py runserver
   ```

## 3. Como Usar o Módulo

Para trabalhar com o estoque, basta acessar a seção de Estoque no painel do sistema.

Na tela principal (Visualização) você consegue ver as quantidades por filial, identificar os itens em alerta e os que já estão zerados. Na aba de **Cadastro/Edição** é possível adicionar novos produtos (nome, preço, peso, quantidade inicial etc.) e ajustar o estoque de cada filial. Já na aba de **Movimentação** dá para acompanhar todas as entradas, saídas e transferências realizadas. Por fim, na aba de **Relatório** é só clicar para gerar e baixar o PDF com o resumo consolidado.

---
```
