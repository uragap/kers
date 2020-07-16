Primeiro cabeçalho | Segundo cabeçalho
--- | ---
Célula de Conteúdo | Célula de Conteúdo
Célula de Conteúdo | Célula de Conteúdo

Primeiro cabeçalho | Segundo cabeçalho
--- | ---
Célula de Conteúdo | Célula de Conteúdo
Célula de Conteúdo | Célula de Conteúdo

![Cidadela](https://vignette.wikia.nocookie.net/masseffect/images/d/d7/MassEffect2Citadel.jpg/revision/latest?cb=20100721191415)

Esquerda alinhada | Alinhado ao centro | Alinhado à direita
:-- | :-: | --:
col 3 é | algum texto prolixo | **$ 1600**
col 2 é | centrado | $ 12
listras de zebra | são legais | ~~ $ 1 ~~

O Dillinger é um editor de HTML5 Markdown HTML5 habilitado para nuvem, pronto para celular e com armazenamento móvel, AngularJS.

- Digite algum Markdown à esquerda
- Veja HTML à direita
- Magia

# verdade

- Importe um arquivo HTML e observe-o converter magicamente em Markdown
- Arraste e solte imagens (requer que sua conta do Dropbox esteja vinculada)

Você também pode:

- Importe e salve arquivos do GitHub, Dropbox, Google Drive e One Drive
- Arraste e solte arquivos de marcação e HTML no Dillinger
- Exportar documentos como Markdown, HTML e PDF

O Markdown é uma linguagem de marcação leve, baseada nas convenções de formatação que as pessoas usam naturalmente no email. Como [John Gruber] escreve no [site Markdown] [df1]

> O objetivo principal do design da sintaxe de formatação do Markdown é torná-lo o mais legível possível. A idéia é que um documento no formato Markdown seja publicável como está, como texto sem formatação, sem parecer que foi marcado com tags ou instruções de formatação.

Este texto que você vê aqui está *realmente* escrito em Markdown! Para ter uma idéia da sintaxe do Markdown, digite algum texto na janela esquerda e observe os resultados à direita.

### falso

Dillinger usa vários projetos de código aberto para funcionar corretamente:

- [AngularJS] - HTML aprimorado para aplicativos da web!
- [Ace Editor] - editor de texto incrível baseado na Web
- [markdown-it] - Analisador de Markdown feito corretamente. Rápido e fácil de estender.
- [Twitter Bootstrap] - ótimo modelo de interface do usuário para aplicativos da web modernos
- [node.js] - E / S registrada para o back-end
- [Express] - estrutura rápida de aplicativos de rede node.js. [@tjholowaychuk]
- [Gulp] - o sistema de criação de streaming
- [Breakdance](https://breakdance.github.io/breakdance/) - conversor de HTML para Markdown
- [jQuery] - duh

E, claro, o próprio Dillinger é de código aberto com um [repositório público] [dill] no GitHub.

### Instalação

![Ilos](https://lh3.googleusercontent.com/proxy/DDV8a7sLIWurhJtW8Ego9bq-JlwpfFFoR0tkLJQKKYXEXoWHB6ZUP5jGKD2VcYt3z1QVsgcn6L3GoU1ns8m9fvi3U51GzddA70ZUMHgzHvjl4-i7YOJY9cShBPrfjUhMQhxaJ97WFBp612XmjMXVGypfGkiBarN4PWxhiHkiYYNW7HGbtTpOcyt9GQ4Q23C2noxLTWFXZMcQZhRpQA_qzu2n6_H6CPViBnhSHpEl4JZAPaGCSJqgZg)

O Dillinger exige que o [Node.js](https://nodejs.org/) v4 + seja executado.

Instale as dependências e devDependencies e inicie o servidor.

```sh
$ cd dillinger
$ npm install -d
$ node app
```

Para ambientes de produção ...

```sh
$ npm install --production
$ NODE_ENV=production node app
```

### Plugins

Atualmente, o Dillinger está estendido com os seguintes plugins. Instruções sobre como usá-los em seu próprio aplicativo estão relacionadas abaixo.

Plugar | Leia-me
--- | ---
Dropbox | [plugins / dropbox / README.md] [PlDb]
GitHub | [plugins / github / README.md] [PlGh]
Google Drive | [plugins / googledrive / README.md] [PLGd]
OneDrive | [plugins / onedrive / README.md] [PLOd]
Médio | [plugins / medium / README.md] [PlMe]
Google Analytics | [plugins / googleanalytics / README.md] [PlGa]

### Desenvolvimento

Deseja contribuir? Ótimo!

Dillinger usa Gulp + Webpack para desenvolvimento rápido. Faça uma alteração no seu arquivo e veja instantaneamente suas atualizações!

Abra seu terminal favorito e execute esses comandos.

Primeira guia:

```sh
$ node app
```

Segunda guia:

```sh
$ gulp watch
```

(opcional) Terceiro:

```sh
$ karma test
```

#### Construindo para fonte

Para liberação de produção:

```sh
$ gulp build --prod
```

Gerando arquivos zip pré-criados para distribuição:

```sh
$ gulp build dist --prod
```

### Docker

O Dillinger é muito fácil de instalar e implantar em um contêiner Docker.

Por padrão, o Docker irá expor a porta 8080, portanto, altere isso no Dockerfile, se necessário. Quando estiver pronto, basta usar o Dockerfile para criar a imagem.

```sh
cd dillinger
docker build -t joemccann/dillinger:${package.json.version} .
```

Isso criará a imagem do dillinger e extrairá as dependências necessárias. Certifique-se de trocar `${package.json.version}` pela versão atual do Dillinger.

Depois de concluído, execute a imagem do Docker e mapeie a porta para o que você desejar no seu host. Neste exemplo, simplesmente mapeamos a porta 8000 do host para a porta 8080 do Docker (ou qualquer porta que foi exposta no Dockerfile):

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

Verifique a implantação navegando até o endereço do servidor no seu navegador preferido.

```sh
127.0.0.1:8000
```

#### Kubernetes + Google Cloud

Veja [KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)

### Todos
