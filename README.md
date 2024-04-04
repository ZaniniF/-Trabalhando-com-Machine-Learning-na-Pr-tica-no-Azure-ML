# Explorando os recursos de Machine Learning

Atividade proposta pelo bootcamp Microsoft Azure AI Fundamentals.

# Primeiro Passo

Acessar o portal do [Azure](https://portal.azure.com/#home) usando as credenciais previamente cadastradas conforme orientado em aulas anteriores.

Sequencialmente vamos criar um novo recurso disponível no canto superior esquerdo, a seguir pesquise por Azure Machine Learning e crie o novo recurso.

Utilizando os parâmetros sugeridos na documentação disponível [aqui](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html), após alguns instantes temos o nossa implantação realizada com sucesso.


# Segundo Passo

Após a inicialização do estúdio podemos explorar os recursos disponíveis na ferramenta e agora vamos treinar um modelo.

O objetivo desse exercício é prever o número de aluguel de bicicletas usando como base os dados de histórico.

Isso será feito usando o recurso de "ML Automatizado" disponível na barra lateral esquerda.

Os dados utilizados nesse exercício estão disponíveis nesse [link](https://aka.ms/bike-rentals).

Assim como no passo anterior, todas as configurações foram feitas utilizando as orientações do laboratório disponível no primeiro passo.

Após aplicação dos parâmetros aguardamos o resultado para poder avaliar o melhor modelo disponível.

# Avaliando o melhor modelo

Através da guia de visão geral do nosso trabalho, é possível observarmos e interagirmos com o melhor modelo 

No canto inferior direito será exibido o melhor modelo, nesse caso foi o "MaxAbsScaler, LightGBM", ao clicar no seu nome os detalhes são exibidos. 

Ao analisar os gráficos de resultados, vemos que há uma diferença entre os valores previstos e os resultados reais.

Para implantar e testar o nosso modelo, na guia "Modelo" vamos utilizar "Implantar" com a opção de serviço web, mais uma vez utilizando os parâmetros descritos no lab, link no primeiro passo.

Após o status de concluído é possível testar os serviços através de "Pontos de Extremidade" na barra lateral esquerda.

Após selecionar o nome do modelo e a opção testar

Obs: uma possível mensagem de erro de dados não integros pode ser exibida porque o estado da implantação ainda não foi concluído, ele pode ficar inacessível por alguns minutos.

Após a execução dos testes e aplicação do JSON solicitado, o resultado foi:

{
  "Results": [
    444.277099014669
  ]
}

Obs: os resultados antes da alteração do JSON foram:

{
  "Results": [
    434.37126365725817
  ]
}

Disponível nesse projeto conforme solicitado o arquivo JSON dos "Pontos de Extremidade".
