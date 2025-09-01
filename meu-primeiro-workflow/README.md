# Meu Primeiro Workflow de CI

Este projeto tem como objetivo demonstrar a criação de um workflow de Integração Contínua (CI) utilizando GitHub Actions. O workflow é acionado automaticamente sempre que há um push para a branch `main`, exceto quando o commit altera apenas o arquivo `README.md`.

## Estrutura do Projeto

O projeto possui a seguinte estrutura de arquivos:

```
meu-primeiro-workflow
├── .github
│   └── workflows
│       └── primeiro-workflow.yml
└── README.md
```

### Arquivo de Workflow

- **.github/workflows/primeiro-workflow.yml**: Este arquivo define o workflow de CI. Ele contém um job chamado `meu-primeiro-job`, que é executado em uma máquina virtual Linux (ubuntu-latest). O job possui três passos:
  1. Exibe uma mensagem com o nome e RA.
  2. Mostra o diretório de trabalho utilizando o comando `pwd`.
  3. Imprime o nome do repositório utilizando uma variável específica do GitHub.

## Instruções para Configuração e Execução

1. **Clone o repositório**: Use o comando `git clone <URL do repositório>` para clonar o repositório em sua máquina local.
2. **Faça alterações**: Realize as alterações desejadas no código.
3. **Adicione e faça commit**: Use os comandos `git add .` e `git commit -m "sua mensagem"` para adicionar e fazer commit das suas alterações.
4. **Envie para o GitHub**: Use o comando `git push origin main` para enviar suas alterações para a branch `main`.
5. **Verifique o Workflow**: Acesse a aba "Actions" no GitHub para visualizar a execução do seu workflow.

Parabéns! Você agora tem um workflow de CI configurado e em funcionamento.