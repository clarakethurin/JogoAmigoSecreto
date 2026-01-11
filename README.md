# JogoAmigoSecreto
🎁 Sorteio de Amigos – Algoritmo de Amigo Secreto

Este projeto implementa um sistema simples de sorteio de amigo secreto, onde o usuário adiciona nomes a uma lista e o algoritmo sorteia pares automaticamente sem repetições.

🚀 Funcionalidades

Adicionar amigos à lista

Impedir nomes vazios ou repetidos

Embaralhar a lista aleatoriamente

Gerar pares no formato:
Fulano → Sicrano

Garantir que o último nome aponte para o primeiro

Reiniciar todo o sorteio e limpar as listas

🧠 Como funciona

🔹 adicionar()

Lê o nome digitado pelo usuário

Valida se está vazio

Verifica se o nome já foi adicionado

Adiciona o nome ao array amigos

Atualiza a exibição da lista em tela

🔹 sortear()

Exige mínimo de 4 amigos

Embaralha a lista com a função embaralha()

Exibe os resultados no formato:

Ana → João  
João → Maria  
Maria → Pedro  
Pedro → Ana  


Garante que não há pares repetidos

🔹 embaralha(lista)

Algoritmo de embaralhamento estilo Fisher-Yates, garantindo aleatoriedade justa:

for (let indice = lista.length; indice; indice--) {
    const indiceAleatorio = Math.floor(Math.random() * indice);
    [lista[indice - 1], lista[indiceAleatorio]] = [lista[indiceAleatorio], lista[indice - 1]];
}

🔹 reiniciar()

Limpa o array amigos

Reseta o conteúdo exibido na tela

📌 Tecnologias utilizadas

JavaScript (Vanilla JS)

Manipulação do DOM

Arrays e validações

Algoritmo Fisher-Yates (embaralhamento)

▶️ Como executar

Clone o repositório:

git clone https://github.com/SEU-USUARIO/sorteio-amigos


Abra o arquivo index.html no navegador.

Adicione amigos, clique em Sortear e veja os pares gerados automaticamente.

👩‍💻 Autora

Clara Kethurin
Desenvolvedora Front-end
Estudante de Análise e Desenvolvimento de Sistemas
