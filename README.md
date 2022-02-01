 1. Qual será o HTML gerado do elemento com id 'container'?

No caso em si, a variavel let container está recebendo
via getelementbyid o que esta sendo referenciado no html pelo
conteiner.

2. Tiraria o this dentro do onClick

3. Nos props são passados para o componente parâmtros de funções,
enquanto o state é gerenciado de dentro do componente 
como variaveis declaradas dentro da função.

4.ReactDOM.render{React.createElement{'div', {styler: {'fontSize': '30px'} }, 
'Hello Word!'), container);


const name = 'Hello Word';

ReactDOM.render(
	name,
	document.getElementById('root')
	);

ou

class Hello extends React.Component {
  render() {
    return <div>Hello {this.props.toWhat}</div>;
  }
}

ReactDOM.render(
  <Hello toWhat=" Hello World" />,
  document.getElementById('root')
);