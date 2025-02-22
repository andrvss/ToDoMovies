<h1 align="center">🎬 To Do Movies 📽️</h1>

<div align="center">

Aplicativo desenvolvido como parte de um teste técnico, com o objetivo de recriar funcionalidades do aplicativo [TodoMovies](https://apps.apple.com/br/app/todomovies-4id792499896), utilizando a [API do The Movies Database](https://www.themoviedb.org).

</div>

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-3.0.2-blue?logo=flutter" alt="Flutter Version">
  <img src="https://img.shields.io/badge/BLoC-Provider-blue?logo=dart" alt="BLoC and Provider">
  <img src="https://img.shields.io/badge/Clean%20Architecture-%F0%9F%93%96%20Clean%20Code-blue" alt="Clean Architecture">
</p>

## 🎨 Arquitetura

Aplicativo desenvolvido com [Flutter](https://flutter.dev) versão 3.0.2, utilizando [BLoC](https://pub.dev/packages/flutter_bloc) e [Provider](https://pub.dev/packages/provider) para gerência de estados e injeção de dependências. As requisições à API são feitas com o pacote [Dio](https://pub.dev/packages/dio). A arquitetura do software segue o padrão de [Clean Architecture](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html), garantindo um código organizado e de fácil manutenção.
## 🚀 Como Usar o Repositório

Após clonar o repositório, siga os passos abaixo para configurar e executar o aplicativo:

1. **Instalar Dependências** 📦

   - Abra o terminal na raiz do projeto.
   - Execute o comando abaixo para instalar todas as dependências listadas no arquivo [pubspec.yaml](./pubspec.yaml):
     ```sh
     flutter pub get
     ```
   - Isso irá baixar e instalar todos os pacotes necessários para o projeto.

2. **Adicionar Chave da API** 🔑

   - Obtenha uma chave de API do [The Movies Database (TMDB)](https://www.themoviedb.org) criando uma conta e acessando as [Configurações de API](https://www.themoviedb.org/settings/api).
   - No projeto, navegue até o arquivo [app_secrets.dart](./lib/src/shared/app_secrets.dart), localizado em `lib/src/shared/`.
   - Abra o arquivo e adicione a sua chave de API ao valor da constante `_apiKeyMovieDB_`. O arquivo deve ficar parecido com o exemplo abaixo:
     ```dart
     const String _apiKeyMovieDB = 'SUA_CHAVE_DE_API_AQUI';
     ```
   - Salve as alterações.

3. **Rodar o Aplicativo** ▶️

   - Você pode rodar o aplicativo a partir da sua IDE preferida (como Visual Studio Code, Android Studio ou IntelliJ IDEA) ou pelo terminal.
   - Para rodar a partir da IDE:
     - Abra o projeto na sua IDE.
     - Selecione um dispositivo emulado ou físico conectado.
     - Clique no botão de execução (geralmente um ícone de "play").
   - Para rodar a partir do terminal:
     - Certifique-se de estar na raiz do projeto.
     - Execute o comando abaixo:
       ```sh
       flutter run
       ```
   - O aplicativo será iniciado e estará pronto para uso.

## 🔖 Layout

Visualizem a documentação desse projeto [NESSE LINK](https://www.figma.com/design/BOkYtcABGfDuS2PAHBg5N3/Proposta-de-Prot%C3%B3tipo---Dimensa?node-id=0-1&t=vhDo2m0BLBsQ34d3-1). É necessário ter conta no [Figma](https://figma.com) para acessá-lo e é muito importante que o faça, pois ele contém informações complementares sobre meu processo de desenvolvimento, mostrando os esboços primários. ferramentas utilizadas e comentários importantes.

## 📝 Considerações Finais

Este projeto ainda não possui uma release oficial e está disponível apenas como código-fonte neste repositório. Ele foi testado exclusivamente no modelo Android, portanto, a eficácia no iOS ainda não foi verificada. 

Há uma possibilidade de a chave API apresentar inconsistências, porém, durante os testes locais, o código funcionou corretamente. 

Novas features estão sendo desenvolvidas e em breve haverão mais interações no app.
