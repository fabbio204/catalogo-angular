# Catalogo

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13.0.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

# Configurando ambiente com angular

## Ferramentas

1. Instalando o angular de forma global
	
	> npm install -g @angular/cli
	
1. Criando um projeto angular

	> ng new catalogo
	
1. Navegue até a pasta criada e execute o comando para executar o projeto

	> ng serve --open
	
	
# Publicando no github pages

1. Branch para publicação

	Por padrão o github pages publica o conteúdo na branch gh-pages, então crie uma branch com esse nome
	
	> git checkout -b gh-pages
	
1. Ferramenta de publicação
	
	Instale o pacote que envia somente o código compilado para o servidor
	
	> npm i angular-cli-ghpages --save-dev

1. Compilando o projeto para pubicar no github pages

	> ng build --base-href "https://fabbio204.github.io/catalogo-angular/"
	
	O parâmetro --base-href é usado para definir a raiz de onde o projeto está instalado
	
1. Para publicar use o comando:

	> ngh --dir=dist/catalogo
	
	O parâmetro `dist/catalogo` é o local onde estão todos os arquivos compilados