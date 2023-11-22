# Hero Level Classifier

## Description

This JavaScript code implements a hero level classifier based on the specified conditions. It prompts the user to enter the hero's name and the amount of experience (XP). Using a decision-making structure, it determines the hero's level and displays a final message indicating the hero's name and achieved level.

## Usage

1. Open the HTML file containing this script in a web browser.

2. When prompted, enter the hero's name and the amount of experience (XP).

3. The code will calculate and display the hero's level based on the entered XP.

## Code

```javascript
// Solicita ao usuário que insira o nome do herói e a quantidade de experiência (XP)
const nomeHeroi = prompt("Digite o nome do herói:");
const xpHeroi = parseInt(prompt("Digite a quantidade de experiência (XP) do herói:"));

// Variável para armazenar o nível do herói
let nivelHeroi;

// Utiliza estrutura de decisão para determinar o nível do herói
if (xpHeroi < 1000) {
  nivelHeroi = "Ferro";
} else if (xpHeroi >= 1001 && xpHeroi <= 2000) {
  nivelHeroi = "Bronze";
} else if (xpHeroi >= 2001 && xpHeroi <= 5000) {
  nivelHeroi = "Prata";
} else if (xpHeroi >= 6001 && xpHeroi <= 7000) {
  nivelHeroi = "Ouro";
} else if (xpHeroi >= 7001 && xpHeroi <= 8000) {
  nivelHeroi = "Platina";
} else if (xpHeroi >= 8001 && xpHeroi <= 9000) {
  nivelHeroi = "Ascendente";
} else if (xpHeroi >= 9001 && xpHeroi <= 10000) {
  nivelHeroi = "Imortal";
} else {
  nivelHeroi = "Radiante";
}

// Exibe a mensagem final
console.log(`O Herói de nome ${nomeHeroi} está no nível de ${nivelHeroi}`);

