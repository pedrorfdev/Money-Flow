# Money Flow

Aplicação web em React e TypeScript para controle de transações financeiras pessoais (entradas, saídas, busca e resumo de saldo).

> **Origem do projeto:** baseado no **dt-money** da trilha React da [Rocketseat](https://www.rocketseat.com.br/), com adaptações para rodar de forma autônoma no navegador:
> - **Modo demo com `localStorage`:** remoção da dependência de `json-server`, com persistência local (`@finance-app:transactions-1.0.0`) e dados iniciais pré-carregados.
> - **Feedback dinâmico de saldo:** o card de total alterna automaticamente entre verde (saldo positivo ou zerado) e vermelho (saldo negativo).
> - **Reset de estado:** botão no rodapé (**Resetar App**) para restaurar os dados iniciais de demonstração.

## Funcionalidades

- Cadastro de transações (entrada ou saída) via modal com validação
- Resumo automático de entradas, saídas e saldo total
- Busca em tempo real por descrição ou categoria
- Persistência local no navegador (`localStorage`) e reset dos dados de demonstração

## Stack

- **Core:** React 18, TypeScript, Vite
- **UI e estilos:** Styled Components, Radix UI (Dialog e Radio Group), Phosphor Icons
- **Formulários e validação:** React Hook Form, Zod
- **Estado:** Context API com `use-context-selector`

## Como rodar

Pré-requisitos: Node.js 18+.

```bash
git clone https://github.com/pedrorfdev/Money-Flow.git
cd Money-Flow
npm install
npm run dev
```

Acesse `http://localhost:5173` no navegador.

### Outros scripts

- `npm run build` — gera o build de produção (`tsc && vite build`)
- `npm run preview` — visualização local do build
- `npm run lint` — verificação com ESLint

## Licença

Distribuído sob a licença MIT. Veja [LICENSE](LICENSE) para mais detalhes.
