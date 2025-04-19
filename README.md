# 🧙‍♂️ Calculadora de Partidas Rankeadas com Heróis – Desafio DIO

Esse projeto foi desenvolvido como parte dos estudos de lógica de programação na DIO. A proposta era criar uma **calculadora de partidas ranqueadas** com foco em estruturas condicionais, funções, classes e objetos — tudo isso no contexto de um **jogo de RPG** com personagens que possuem diferentes tipos e ataques.

A ideia principal foi aplicar conceitos de **Programação Orientada a Objetos (POO)** para representar heróis com características distintas e simular seus comportamentos em combate.

## 🎯 Objetivo

Criar uma classe chamada `Heroi` com as seguintes propriedades:

- `nome`: nome do personagem
- `idade`: idade do personagem
- `tipo`: classe do herói (`guerreiro`, `mago`, `monge`, `ninja`)

Além disso, a classe possui um método `atacar()` que exibe a seguinte mensagem no console:

O {tipo} atacou usando {ataque}

csharp
Copiar
Editar

O tipo de ataque varia de acordo com a classe do herói:

| Tipo do Herói | Ataque Executado        |
|---------------|-------------------------|
| mago          | usou magia              |
| guerreiro     | usou espada             |
| monge         | usou artes marciais     |
| ninja         | usou shuriken           |

---

## 💻 Exemplo de Código

```javascript
class Heroi {
  constructor(nome, idade, tipo) {
    this.nome = nome;
    this.idade = idade;
    this.tipo = tipo.toLowerCase();
  }

  atacar() {
    let ataque;

    switch (this.tipo) {
      case "mago":
        ataque = "magia";
        break;
      case "guerreiro":
        ataque = "espada";
        break;
      case "monge":
        ataque = "artes marciais";
        break;
      case "ninja":
        ataque = "shuriken";
        break;
      default:
        ataque = "um ataque desconhecido";
    }

    console.log(`O ${this.tipo} atacou usando ${ataque}`);
  }
}

// Testando com alguns personagens
const heroi1 = new Heroi("Arthas", 30, "guerreiro");
const heroi2 = new Heroi("Merlin", 150, "mago");
const heroi3 = new Heroi("Lee", 40, "monge");
const heroi4 = new Heroi("Hanzo", 28, "ninja");

heroi1.atacar(); // O guerreiro atacou usando espada
heroi2.atacar(); // O mago atacou usando magia
heroi3.atacar(); // O monge atacou usando artes marciais
heroi4.atacar(); // O ninja atacou usando shuriken
🚀 Como Executar o Projeto
Clone o repositório:

bash
Copiar
Editar
git clone https://github.com/seu-usuario/nome-do-repositorio.git
Acesse a pasta do projeto:

bash
Copiar
Editar
cd nome-do-repositorio
Execute o arquivo:

bash
Copiar
Editar
node index.js
Você pode testar criando seus próprios heróis e observando os ataques diferentes de cada classe.

🧠 Aprendizados
Esse projeto me ajudou a fixar melhor conceitos como:

Uso de classes e construtores em JavaScript

Criação e uso de métodos personalizados

Lógica com switch case para múltiplas condições

Organização de código orientado a objetos

📌 Observações
Esse projeto pode ser expandido para incluir:

Pontuação de dano

Sistema de defesa ou resistência

Combate entre dois heróis

Tipos adicionais de personagens

👨‍🎓 Sobre mim
Sou estudante universitário de Ciência de Dados e tenho buscado desafios práticos que me ajudem a aplicar lógica de programação em contextos criativos. Esse tipo de projeto, com elementos de jogos e simulação, é uma forma divertida e eficaz de aprender.

Se quiser ver mais projetos como esse, dá uma olhada no meu GitHub. 🚀
