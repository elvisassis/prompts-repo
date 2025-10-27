# javascript-react-component.md

# 📝 Componente React em JavaScript

## Descrição
Este prompt é usado para gerar a estrutura de código e a lógica de um componente React (JSX ou TSX), focando em funcionalidade específica, como tratamento de estado, props e eventos.

## Estrutura do Prompt
**Exemplo:**
- Gere um componente funcional simples em React (JavaScript) chamado `Contador`. Ele deve exibir um número e ter dois botões: um para incrementar e outro para decrementar o valor. Use o hook `useState`.

## Resultado Esperado
```javascript
import React, { useState } from 'react';

function Contador() {
  const [contagem, setContagem] = useState(0);

  const incrementar = () => {
    setContagem(contagem + 1);
  };

  const decrementar = () => {
    setContagem(contagem(prevContagem) => prevContagem - 1);
  };

  return (
    <div>
      <h1>Contagem: {contagem}</h1>
      <button onClick={incrementar}>Incrementar</button>
      <button onClick={decrementar}>Decrementar</button>
    </div>
  );
}

export default Contador;