# Alembic :: Tema para Meduza Static Site Generator

Tema baseado no tema [Alembic](https://alembic.darn.es/) de [David Darnes](https://darn.es/).


## Instalação
O método de instalação recomendado é utilizando o [Composer](https://getcomposer.org):

```sh
composer require meduza-static-site-generator/meduza-theme-alembic
```

## Configuração
A configuração do plugin é bastante simples:

```yaml
## Configurações do tema Alembic
---
theme:
  # Caminho para os diretórios do tema. Sem / no final.
  # Diretório dos templates para uso de Twig\Loader\FilesystemLoader
  layouts: "./vendor/meduza-static-site-generator/meduza-theme-alembic/layouts"
  # Diretório para conteúdo estático que será copiado no build (arquivos e subdiretórios)
  static: "./vendor/meduza-static-site-generator/meduza-theme-alembic/static"
  # Diretório de conteúdo adicional (frontmatter + markdown) e que será processado durante o build.
  content: "./vendor/meduza-static-site-generator/meduza-theme-alembic/content"
  # Logotipo do site.
  logo: "assets/logo.svg"
  # Imagem padrão de background (para o caso de não haver "image" no frontmatter)
  image: "assets/image.jpg"
  # Menu principal do site.
  mainMenu:
    - 
      label: "Home"
      url: "index.html"
    - 
      label: "About"
      url: "pages/about.html"
    - 
      label: "Posts"
      url: "posts.html"

```

Fornecemos um arquivo de configuração *alembic.yml* com todas as opções documentadas na raiz do projeto. Inclua as configurações ou importe com ```import``` no seu arquivo de configurações.

## Plugins suportados

**Alembic** suporta os seguintes plugins:

- [Resumizer](https://github.com/meduza-static-site-generator/meduza-plugin-resumizer)
- [Time Read](https://github.com/meduza-static-site-generator/meduza-plugin-time-read)
- [Catloger](https://github.com/meduza-static-site-generator/meduza-plugin-catloger)

Os plugins são instalados automaticamente como dependências do tema via [Composer](https://getcomposer.org)

## Como contribuir
Para contribuir com o projeto, faça o seguinte:

- Crie um *fork*;
- Clone o *fork* e crie um novo *branch* para a sua contribuição;
- Envie suas alterações para o *fork*;
- Crie um *pull request*.

Será interessante você criar um *issue* no repositório oficial para a sua alteração e referenciá-la no nome do seu *branch* e nos *commits*. Também referencie seu *pull request* nas *issue*. Isso agilizará a análise da sua contribuição.

## Licença

**Alembic** é licenciado sob a [MIT Licence](https://github.com/meduza-static-site-generator/meduza-theme-alembic/blob/main/LICENSE)