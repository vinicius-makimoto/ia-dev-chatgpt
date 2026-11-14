# Service Desk Acadêmico

Aplicação web simples para registrar e acompanhar chamados de suporte. O projeto foi criado para demonstrar um fluxo básico de Service Desk e boas práticas de versionamento.

## Descrição para o GitHub (350 caracteres)

> Aplicação web de Service Desk para abrir e acompanhar chamados. Permite pesquisar por ID, título ou solicitante, atualizar status e prioridade, registrar correções e consultar o histórico. Desenvolvida com HTML, CSS e JavaScript, funciona diretamente no navegador e salva os dados no localStorage. Uma demonstração prática de suporte e versionamento.

## Funcionalidades

- Abrir chamados com solicitante, e-mail, categoria, prioridade, título e descrição.
- Pesquisar chamados por ID, título ou nome do solicitante.
- Consultar a fila e selecionar um chamado no painel do analista.
- Atualizar status e prioridade e registrar a correção aplicada.
- Acompanhar os eventos do chamado e consultar a tabela de auditoria.
- Armazenar os dados no navegador usando `localStorage`.

### Status disponíveis

- **Aberto** — azul
- **Em atendimento** — laranja
- **Aguardando usuário** — roxo
- **Resolvido** — verde

## Como executar

Não há dependências para instalar nem servidor obrigatório.

1. Abra `service-desk/abrir-service-desk.bat`, ou
2. abra `service-desk/index.html` diretamente no navegador.

## Tecnologias

- HTML
- CSS
- JavaScript (sem bibliotecas externas)
- `localStorage` para persistência local

## Estrutura

```text
.
├── DETALHAMENTO.md       # histórico das correções, commits e validações
├── README.md             # apresentação e instruções do projeto
└── service-desk/
    ├── app.js            # regras de negócio e persistência
    ├── index.html        # estrutura da aplicação
    ├── styles.css        # estilos e layout
    └── abrir-service-desk.bat
```

## Observações

Os chamados ficam apenas no armazenamento local do navegador usado para abrir a aplicação; não há servidor ou banco de dados compartilhado. O botão **Limpar base local** restaura os chamados de exemplo no navegador atual.

Consulte [DETALHAMENTO.md](DETALHAMENTO.md) para ver os bugs corrigidos, as melhorias, o fluxo de versionamento e os resultados da validação ponta a ponta.
