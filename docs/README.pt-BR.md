<br>

<div align="center">

[<img src="../resources/icon.png" width="144"/>](https://help.hydralauncher.gg)

  <h1 align="center">Hydra Launcher</h1>

  <p align="center">
    <strong>Hydra é um Launcher de Jogos com seu próprio cliente de bittorrent integrado.</strong>
  </p>

[![build](https://img.shields.io/github/actions/workflow/status/hydralauncher/hydra/build.yml)](https://github.com/hydralauncher/hydra/actions)
[![release](https://img.shields.io/github/package-json/v/hydralauncher/hydra)](https://github.com/hydralauncher/hydra/releases)

[![pt-BR](https://img.shields.io/badge/lang-pt--BR-green.svg)](README.pt-BR.md)
[![en](https://img.shields.io/badge/lang-en-red.svg)](../README.md)
[![ru](https://img.shields.io/badge/lang-ru-yellow.svg)](README.ru.md)
[![uk-UA](https://img.shields.io/badge/lang-uk--UA-blue)](README.uk-UA.md)
[![be](https://img.shields.io/badge/lang-be-orange)](README.be.md)
[![es](https://img.shields.io/badge/lang-es-red)](README.es.md)
[![fr](https://img.shields.io/badge/lang-fr-blue)](README.fr.md)
[![de](https://img.shields.io/badge/lang-de-black)](README.de.md)
[![ita](https://img.shields.io/badge/lang-it-red)](README.it.md)
[![cs](https://img.shields.io/badge/lang-cs-purple)](README.cs.md)
[![da](https://img.shields.io/badge/lang-da-red)](README.da.md)
[![nb](https://img.shields.io/badge/lang-nb-blue)](README.nb.md)
[![et](https://img.shields.io/badge/lang-et-blue.svg)](README.et.md)
[![tr](https://img.shields.io/badge/lang-tr-red.svg)](README.tr.md)

![Hydra Catalogue](./screenshot.png)

</div>

## Índice

- [Índice](#índice)
- [Sobre](#-sobre)
- [Recursos](#-recursos)
- [Instalação](#-instalação)
- [Contribuindo](#-contribuindo)
  - [Junte-se ao nosso Telegram](#-junte-se-ao-nosso-telegram)
  - [Fork e clone o seu repositório](#-fork-e-clone-o-seu-repositório)
  - [Formas de contribuir](#-formas-de-contribuir)
  - [Estrutura do Projeto](#-estrutura-do-projeto)
- [Compile a partir do código-fonte](#-compile-a-partir-do-código-fonte)
  - [Instale Node.js](#-instale-nodejs)
  - [Instale Yarn](#-instale-yarn)
  - [Instale Dependencias do Node](#-instale-dependencias-do-node)
  - [Instale Python 3.9](#-instale-python-39)
  - [Instale Python Dependencies](#-instale-python-dependencies)
- [Environment variables](#-environment-variables)
- [Running](#-running)
- [Build](#-build)
  - [ Criar o cliente bittorrent](#-build-the-bittorrent-client)
  - [Criar a aplicação Electron](#-build-the-electron-application)
- [Contribuidores](#-contributors)
- [Licença](#-licença)

## <a name="about"> Sobre

**Hydra** é um **Launcher de Jogos** com seu próprio **Cliente BitTorrent incorporado**.
<br>
O launcher é escrito em TypeScript (Electron) e Python, que lida com o sistema de torrent usando libtorrent.

## <a name="features"> Recursos

- Cliente BitTorrent incorporado próprio
- Integração com [How Long To Beat (HLTB)](https://howlongtobeat.com/) na página do jogo
- Personalização do caminho de downloads
- Suporte para Windows e Linux
- Constantemente atualizado
- E mais ...

## <a name="installation"> Instalação

Siga os passos abaixo para instalar:

1. Baixe a versão mais recente do Hydra na página de [Releases](https://github.com/hydralauncher/hydra/releases/latest).
   - Baixe apenas o .exe se quiser instalar o Hydra no Windows.
   - Baixe .deb ou .rpm ou .zip se quiser instalar o Hydra no Linux. (depende da sua distribuição Linux)
2. Execute o arquivo baixado.
3. Aproveite o Hydra!

## <a name="contributing"> Contribuindo

### <a name="join-our-telegram"></a> Junte-se ao nosso Telegram

Concentramos nossas discussões no nosso canal do [Telegram](https://t.me/hydralauncher).

### <a name="fork-and-clone-your-repository"></a> Fork e clone o seu repositório

1. Faça um fork do repositório [(clique aqui para fazer o fork agora)](https://github.com/hydralauncher/hydra/fork)
2. Clone o código do seu fork `git clone https://github.com/seu_nome_de_usuário/hydra`
3. Crie uma nova branch
4. Faça o push dos seus commits
5. Envie um novo Pull Request

### <a name="ways-you-can-contribute"></a> Formas de contribuir

- **Tradução**: Queremos que o Hydra esteja disponível para o maior número possível de pessoas. Sinta-se à vontade para ajudar a traduzir para novos idiomas ou atualizar e melhorar aqueles que já estão disponíveis no Hydra.
- **Código**: O Hydra é construído com Typescript, Electron e um pouco de Python. Se você deseja contribuir, junte-se ao nosso [Telegram](https://t.me/hydralauncher)!

### <a name="project-structure"></a> Estrutura do Projeto

- torrent-client: Utilizamos o libtorrent, uma biblioteca Python, para gerenciar downloads via torrent.
- src/renderer: A interface de usuário (UI) da aplicação.
- src/main: Toda a lógica da aplicação reside aqui.

## <a name="build-from-source"></a> Compile a partir do código-fonte

### <a name="install-nodejs"></a> Instale Node.js

Certifique-se de ter o Node.js instalado em sua máquina. Se não, faça o download e instale-o em [nodejs.org](https://nodejs.org/).

### <a name="install-yarn"></a> Instale Yarn

Yarn é um gerenciador de pacotes para Node.js. Se você ainda não o instalou, pode fazê-lo seguindo as instruções em [yarnpkg.com](https://classic.yarnpkg.com/lang/en/docs/install/).

### <a name="install-node-dependencies"></a> Instale Dependencias do Node

Navegue até o diretório do projeto e instale as dependências do Node usando o Yarn:

```bash
cd hydra
yarn
```

### <a name="install-openssl-11"></a> Instale OpenSSL 1.1

[OpenSSL 1.1](https://slproweb.com/download/Win64OpenSSL-1_1_1w.exe) é exigido pelo libtorrent em ambientes Windows.

### <a name="install-python-39"></a> Instale Python 3.9

Certifique-se de ter o Python 3.9 instalado em sua máquina. Você pode baixá-lo e instalá-lo em [python.org](https://www.python.org/downloads/release/python-3913/).

### <a name="install-python-dependencies"></a> Instale Python Dependencies

Instale as dependências Python necessárias usando o pip:

```bash
pip install -r requirements.txt
```

## <a name="environment-variables"></a> Variáveis de ambiente

Você precisará de uma chave da API SteamGridDB para buscar os ícones do jogo durante a instalação.

Depois de obtê-lo, você pode copiar ou renomear o arquivo `.env.example` para `.env` e inserir `STEAMGRIDDB_API_KEY`.

## <a name="running"></a> Executando

Uma vez que você tenha configurado tudo, você pode executar o seguinte comando para iniciar tanto o processo Electron quanto o cliente BitTorrent:

```bash
yarn dev
```

## <a name="build"></a> Build

### <a name="build-the-bittorrent-client"></a> Criar o cliente bittorrent

Compile o cliente BitTorrent usando este comando

```bash
python torrent-client/setup.py build
```

### <a name="build-the-electron-application"></a> Criar a aplicação Electron

Compile a aplicação Electron usando este comando:

No Windows:

```bash
yarn build:win
```

No Linux:

```bash
yarn build:linux
```

## <a name="contributors"></a> Contribuidores

<a href="https://github.com/hydralauncher/hydra/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=hydralauncher/hydra" />
</a>

## <a name="license"></a> Licença

O Hydra é licenciado sob a [Licença MIT](LICENSE).
