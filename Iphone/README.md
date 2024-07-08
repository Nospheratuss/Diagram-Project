# Projeto iPhone 2007

Este projeto modela as funcionalidades do iPhone 2007 conforme descritas no vídeo de lançamento. As funcionalidades incluem um reprodutor musical, um aparelho telefônico e um navegador na internet. Utilizamos UML para diagramação e Java para implementação.

## Funcionalidades

- **Reprodutor Musical**
  - `tocar()`: Inicia a reprodução de uma música.
  - `pausar()`: Pausa a reprodução da música.
  - `selecionarMusica(String musica)`: Seleciona uma música específica para reprodução.

- **Aparelho Telefônico**
  - `ligar(String numero)`: Faz uma chamada para o número especificado.
  - `atender()`: Atende uma chamada.
  - `iniciarCorreioVoz()`: Inicia o correio de voz.

- **Navegador na Internet**
  - `exibirPagina(String url)`: Exibe a página da URL especificada.
  - `adicionarNovaAba()`: Adiciona uma nova aba no navegador.
  - `atualizarPagina()`: Atualiza a página atual.

## Diagrama UML

O diagrama abaixo representa as interfaces e a classe iPhone.


@startuml
class ReprodutorMusical {
    +tocar()
    +pausar()
    +selecionarMusica(String musica)
}

class AparelhoTelefonico {
    +ligar(String numero)
    +atender()
    +iniciarCorreioVoz()
}

class NavegadorInternet {
    +exibirPagina(String url)
    +adicionarNovaAba()
    +atualizarPagina()
}

class iPhone implements ReprodutorMusical, AparelhoTelefonico, NavegadorInternet
@enduml
