# Design Pattern - Builder
O código desse repositório mostra o aplicação do Design Pattern "Template Method" através de um exemplo na linguagem PHP no contexto do tratamento de diferentes tipos de dados.

## Classe Abstrata ProcessadorDeDados:
Essa é uma classe abstrata que serve como template para o processamento dos dados. Ela cria um método template chamado 'processarDados', que fica resposável por coordenar as etapas do processamento de dados, os métodos a serem implementados pelas subclasses são marcados como abstratos (abstract), indicando que devem ser implementados pelas classes derivadas.

## Classe ProcessadorDeTexto:
Essa pode ser defina como uma subclasse de ProcesadorDeDados que implementa etapas especificas para processar dados de texto. Cada um dos métodos abstratos na classe base é implementado de acordo com o processamento necessário para dados de texto. Por exemplo, o método carregarDados exibe uma mensagem indicando que os dados de texto estão sendo carregados, em uma implementação de contexto real, o tratamento propriamente tido seria implementado.

## Classe ProcessadorDeNumeros:
A mesma implementação do ProcessadorDeTexto mas para o contexto do processamento númerico.

## Função main():
A função main é ponto incial de execução do código. Ela cria instâncias das classes ProcessadorDeTexto e ProcessadorDeNumeros e demonstra como essas classes podem ser usadas para processar diferentes tipos de dados, nesse caso textos e números. Os dados de exemplo são passados para o método processarDados, e cada etapa do processo é exibida na saída.

## Chamada da função main()
Essa linha realiza a chamada para a função principal, conforme o programa é executado as mensagens são exibidas a cada etapa.
