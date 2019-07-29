# DotNet RabbitMQ Hello World!

This project is a basic script displaying the core functionality of integrating RabbitMQ with a DotNet application. RabbitMQ is a message broker and queuing software used by enterprise organizations and startups for message centers, among it's many other purposes.

![RabbitMQ](workflow.png)

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
