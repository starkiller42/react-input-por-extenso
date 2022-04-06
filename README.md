# React Input por extnso

Componente React que retorna por extenso. - Feito para estudo

## Como instalar

Abaixo as formas de como instalar essa biblioteca utilizando o npm ou yarn:
...
npm install react-meu-input-por-extenso
# ou
yarn add react-meu-input-por-extenso
...


## Como usar

Uma forma básica de como utilizar o componente:


```jsx

import ReactInputPorExtenso from 'react-meu-input-por-extenso';
import { useState } from 'react';

function App() {
  const [ numero, setNumero ] = useState("");

  return (
    <>
        <ReactInputPorExtenso 
          tipoExtenso="monetario"
          onChange={numeroExtenso => setNumero(numeroExtenso)} 
        />
        <p>
          <strong>Número por extenso</strong>: {numero}
        </p>
    </>
  );
}

```

## Propriedades

Esse componente é uma abstração de um componente input do tipo númerico,
todas as propriedades de um input estão disponiveis.

| Propriedade   | Valor inicial | Tipo | Descrição                   |
|---------------|---------------|------|-----------------------------|
| tipoExtenso   | normal        |string|Formato de extensão do número|