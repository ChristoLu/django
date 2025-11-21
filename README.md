🚗 Projeto Carros – Aplicação Django para Gestão de Veículos

Este projeto é uma aplicação web desenvolvida com Django, focada no cadastro, listagem, filtragem e exibição de carros, incluindo suporte a imagens, categorias (marcas) e formulários completos com validações.

Ele foi estruturado para servir como um guia prático de aprendizado em Django, cobrindo desde a criação do projeto até recursos avançados do framework.

📁 Estrutura do Projeto
🏁 Criação e Organização do Projeto

O projeto inicia com a criação do ambiente Django, entendimento dos arquivos básicos e configuração da primeira App.
Também é abordada a estrutura em camadas do Django e o funcionamento geral do framework.

🗂️ Banco de Dados, Models e Admin

Criação de modelos para representar carros e marcas.

Uso de ForeignKey para relacionar carros a suas respectivas marcas.

Execução de migrações para criação das tabelas.

Configuração do Django Admin para gerenciar registros de forma intuitiva.

Ajustes adicionais no projeto para suportar novas funcionalidades.

🖼️ Armazenamento de Imagens

A aplicação permite o upload e armazenamento de imagens dos carros, configurando diretórios de mídia e exibindo as imagens em templates.

🔐 Admin e Usuário

Foi feita a separação entre a visão administrativa (via Django Admin) e a visão pública para os usuários do sistema.

🌐 URLs, Views e Templates

- Criação das rotas (URLs) para organização da aplicação.

- Desenvolvimento das Views responsáveis por retornar páginas e dados.

- Construção de templates utilizando Django Template Language (DTL).

- Organização de um base template reutilizável para todas as páginas.

- Melhoria progressiva dos templates com listas, filtros e buscas.

🔍 Consultas e Filtros com Django ORM

- A aplicação faz diferentes tipos de busca e filtragem, como:

- Listar todos os carros cadastrados.

- Filtrar registros com filter().

- Utilizar parâmetros vindos da requisição (request.GET).

- Pesquisas usando icontains (busca parcial).

- Ordenação dinâmica usando order_by.
  
📝 Formulários e Cadastro

O projeto implementa:

- Formulários manuais usando forms.Form.

- Cadastro de novos carros com validações.

- Migração para ModelForm, tornando o processo mais simples e padronizado.

- Criação de validações customizadas para garantir integridade dos dados.

🚀 Funcionalidades da Aplicação

- Cadastro de carros e marcas.

- Upload e exibição de imagens.

- Sistema de busca e filtragem por nome, marca e outros parâmetros.

- Ordenação de resultados.

- Área administrativa completa via Django Admin.

- Templates reaproveitáveis com herança.

- Formulários automáticos e customizados com validações.

🔧 Tecnologias Utilizadas

- Django (Framework principal)

- Python 3.x

- SQLite (banco padrão, facilmente substituível)

- HTML, CSS e Django Template Language

- Bootstrap (opcional, se usado na interface)

▶️ Como Rodar o Projeto

Clone o repositório

git clone https://github.com/seuusuario/projeto-carros.git
cd projeto-carros


*Crie um ambiente virtual

- python -m venv venv
- source venv/bin/activate      # Linux/Mac
- venv\Scripts\activate         # Windows


*Instale as dependências

- pip install -r requirements.txt


*Execute as migrações

python manage.py migrate


Execute o servidor

**python manage.py runserver**
