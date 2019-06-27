# DotNet RabbitMQ Hello World!

This project is a basic script displaying the cord functionality of integrating RabbitMQ with a DotNet application.

## Installation

RabbitMQ installation instructions can be found [here](https://www.rabbitmq.com/install-windows.html). This application requires an [installation of Erlang](https://www.erlang.org/downloads) to the host machiene.

## Usage

```shell
git clone [this repo]
cd [this repo]/Receive
dotnet restore
dotnet run

# open a new terminal
cd [this repo]/Send
dotnet restore
dotnet run
```

You should see the each terminal display a send or receive message. Leaving the "Receive" terminal open and running, quit the "Send" terminal by pressing `Enter`, then re-run `dotnet run` again. Another message should appear in the "Receive" terminal in real time.
