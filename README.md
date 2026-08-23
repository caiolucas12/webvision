# Web Vision

Dashboard web estático para visualização do estado de máquinas em uma rede interna.

O projeto apresenta uma interface de monitoramento com dispositivos, endereços IP, uso de CPU e RAM, status de conexão e informações sobre a arquitetura sugerida para uma implementação real.

> Atualmente, os dados exibidos são estáticos e servem como protótipo visual.

## Funcionalidades

- Dashboard responsivo para desktop e dispositivos móveis
- Lista de máquinas monitoradas
- Indicadores visuais de CPU e RAM
- Status online dos dispositivos
- Detalhes da máquina selecionada
- Seção explicativa sobre a arquitetura do projeto
- Execução sem dependências externas ou banco de dados

## Tecnologias

- HTML5
- CSS3
- JavaScript não é necessário nesta versão estática

## Estrutura do projeto

```text
.
├── .vscode/
│   └── launch.json
├── index.html
├── style.css
└── README.md

## Como executar

### Opção 1: abrir diretamente

Abra o arquivo `DWEB/index.html` em qualquer navegador moderno.

### Opção 2: usar o VS Code

Abra a pasta do projeto no VS Code e execute a configuração **Iniciar o Navegador Integrado no localhost** disponível em `.vscode/launch.json`.

### Opção 3: usar um servidor local

Na raiz do projeto, execute um servidor HTTP de sua preferência. Por exemplo, com Python:

```bash
python -m http.server 8080
```

Depois acesse:

```text
http://localhost:8080/DWEB/index.html
```

## Publicação no GitHub

1. Crie um novo repositório no GitHub.
2. Na pasta do projeto, inicialize o Git:

```bash
git init
git add .
git commit -m "Adiciona projeto Web Vision"
```

3. Vincule o repositório remoto e envie os arquivos:

```bash
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git
git push -u origin main
```

Substitua `SEU_USUARIO/SEU_REPOSITORIO` pelos dados do seu repositório.

## GitHub Pages

Como o projeto é estático, ele pode ser publicado pelo GitHub Pages:

1. Abra **Settings > Pages** no repositório.
2. Em **Build and deployment**, selecione **Deploy from a branch**.
3. Escolha a branch `main` e a pasta `/root`.
4. Salve e aguarde a geração do endereço público.

## Próximos passos

Para transformar o protótipo em um monitoramento real, será necessário adicionar:

- Um agente para coletar métricas das máquinas
- Uma API para receber os dados
- Armazenamento para histórico
- Atualização dos indicadores em tempo real

## Licença

Este projeto foi desenvolvido para fins acadêmicos e de prototipação.
