# Sistema de Estacionamento em C#

Este projeto é uma solução para um desafio de programação proposto pela [DIO](https://www.dio.me/), implementado como uma **Console Application** em C# .NET. O sistema simula as operações básicas de um estacionamento, como registrar a entrada e saída de veículos e calcular o valor a ser pago pela permanência.

## 🚀 Funcionalidades

O sistema oferece um menu interativo com as seguintes opções:

1.  **Cadastrar Veículo**: Adiciona um veículo ao estacionamento, registrando sua placa.
2.  **Remover Veículo**: Registra a saída de um veículo. O usuário informa a placa e a quantidade de horas que o veículo permaneceu no local. O sistema então calcula e exibe o valor total a ser pago.
3.  **Listar Veículos**: Exibe uma lista com as placas de todos os veículos que estão atualmente no estacionamento.
4.  **Encerrar**: Finaliza a execução do programa.

## ⚙️ Lógica de Negócio

-   O estacionamento possui um **preço inicial** fixo.
-   É cobrado um **preço por hora** adicional, que é multiplicado pela quantidade de horas que o veículo ficou estacionado.
-   O valor total para o cliente é a soma do `preço inicial` com o (`preço por hora` * `horas estacionado`).

## 🛠️ Tecnologias Utilizadas

-   **C#**: Linguagem de programação principal.
-   **.NET**: Plataforma de desenvolvimento.

## 📂 Estrutura do Código

O projeto está organizado em duas classes principais:

-   `Program.cs`: Contém a lógica da interface com o usuário (o menu de opções) e a instanciação dos objetos. É o ponto de entrada da aplicação.
-   `Estacionamento.cs`: Classe que encapsula toda a lógica de negócio do estacionamento. Contém os preços, a lista de veículos e os métodos para `AdicionarVeiculo()`, `RemoverVeiculo()` e `ListarVeiculos()`.

## 🏃 Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/jdecdomingues/DesafioEstacionamentoDotNet.git](https://github.com/jdecdomingues/DesafioEstacionamentoDotNet.git)
    ```

2.  **Navegue até o diretório do projeto:**
    ```bash
    cd DesafioEstacionamentoDotNet
    ```

3.  **Execute a aplicação usando o .NET CLI:**
    ```bash
    dotnet run
    ```

4.  Após a execução, o menu interativo será exibido no seu terminal.
