# Sistema de Inventário de Armazém

Este projeto implementa um sistema básico de inventário para gerenciamento de produtos, fornecedores e categorias em um armazém. O banco de dados é projetado para armazenar e organizar informações sobre produtos disponíveis, fornecedores e categorias, além de fornecer consultas e operações de atualização e exclusão.

## Funcionalidades

- **Gestão de Categorias**: Registra e armazena informações sobre as categorias de produtos no armazém.
- **Gestão de Fornecedores**: Registra os fornecedores, seus dados de contato e endereço.
- **Gestão de Produtos**: Armazena dados sobre os produtos, incluindo nome, descrição, preço, quantidade em estoque, categoria e fornecedor.
- **Consultas**:
  - Listar produtos disponíveis em estoque.
  - Consultar produtos por categoria.
  - Consultar fornecedores que fornecem produtos acima de um preço específico.
- **Atualização de Dados**:
  - Atualizar preços de produtos e endereços de fornecedores.
  - Alterar descrições de categorias.
- **Exclusão de Dados**:
  - Remover produtos do inventário.
  - Excluir categorias e seus produtos relacionados.
  - Excluir fornecedores não relacionados a produtos.

## Estrutura do Banco de Dados

### Tabelas:

- **Categorias**:
  - `CategoriaID`: Identificador único da categoria.
  - `Nome`: Nome da categoria.
  - `Descricao`: Descrição opcional da categoria.

- **Fornecedores**:
  - `FornecedorID`: Identificador único do fornecedor.
  - `Nome`: Nome do fornecedor.
  - `Contato`: Detalhes de contato do fornecedor.
  - `Endereco`: Endereço do fornecedor.

- **Produtos**:
  - `ProdutoID`: Identificador único do produto.
  - `Nome`: Nome do produto.
  - `Descricao`: Descrição do produto.
  - `Preco`: Preço do produto.
  - `QuantidadeEmEstoque`: Quantidade em estoque do produto.
  - `CategoriaID`: Categoria associada ao produto.
  - `FornecedorID`: Fornecedor associado ao produto.

## Consultas Disponíveis

1. **Listar todos os produtos disponíveis em estoque**:
   - Exibe todos os produtos com estoque maior que zero.

2. **Mostrar produtos de uma categoria específica**:
   - Exibe produtos pertencentes a uma categoria específica.

3. **Consultar fornecedores de produtos acima de um preço específico**:
   - Exibe fornecedores que fornecem produtos com preços superiores a um valor determinado.

## Como Usar

1. **Criar o Banco de Dados**:
   Execute o script SQL fornecido para criar o banco de dados e as tabelas necessárias.

2. **Inserir Dados**:
   Insira os dados de categorias, fornecedores e produtos usando os scripts SQL.

3. **Consultas e Operações**:
   Use as consultas SQL para visualizar, atualizar e excluir informações do banco de dados conforme necessário.

## Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

## Requisitos

- MySQL ou outro sistema de gerenciamento de banco de dados SQL compatível.
- Editor SQL para execução de consultas e scripts.
