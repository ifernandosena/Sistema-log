# Sistema-log
Sistema de Log . criado para apresentar resultados e informações detalhadas 

.
- Feedback visual para carregamento e erros.

## Estrutura do Projeto
```
📂 src
 ├── 📄 LogAlocacao.js  # Componente principal
 ├── 📄 LogAlocacao.css # Estilos personalizados
 ├── 📂 assets          # Pasta para assets (se necessário)
 ├── 📂 components      # Componentes auxiliares (se houver)
 └── 📂 services        # Serviços de API (caso queira separar a lógica de requisição)
```

## Instalação e Execução
### Pré-requisitos
Certifique-se de ter o Node.js e o gerenciador de pacotes npm ou yarn instalados.


## Uso
1. Acesse a aplicação no navegador (geralmente em `http://localhost:3000`).
2. Selecione uma data de início e uma data de fim.
3. Clique no botão "Buscar" para carregar os registros.
4. Os dados serão exibidos em uma tabela responsiva.

## API Endpoint
O componente faz requisições para:
```
GET http://192.168.1.214:3333/lista_Logaloc?inicio=YYYY-MM-DD&fim=YYYY-MM-DD
```

## Personalização
Caso precise alterar a URL da API, edite o arquivo `LogAlocacao.js` e modifique a linha:
```js
const response = await axios.get(`http://192.168.1.214:3333/lista_Logaloc?inicio=${dataInicio}&fim=${dataFim}`);
```

## Estilos
Os estilos personalizados estão no arquivo `LogAlocacao.css`, que pode ser modificado para adaptar a interface conforme necessário.

## Melhorias Futuras
- Adicionar paginação para grandes conjuntos de dados.
- Implementar cache local para melhorar a performance.
- Criar um serviço separado para a API para melhor modularidade.



