# Rafael Parise Passos

Professor do curso técnico de Desenvolvimento de Sistemas, no ensino médio da
rede estadual de São Paulo (SEDUC-SP). Crio aplicativos pedagógicos para a
sala de aula.

## O que ensino

- Lógica e Linguagem de Programação
- Redes e Segurança da Informação na Nuvem
- Processos de Desenvolvimento de Software e Metodologias Ágeis
- Programação Back-End e Front-End
- Modelagem e Desenvolvimento de Banco de Dados

## Projeto em destaque: ARENA — o console da turma

<a href="https://github.com/RafaParise/arena-console">
  <img src="https://raw.githubusercontent.com/RafaParise/arena-console/main/docs/imagens/arena-capa.png"
       width="640"
       alt="ARENA, o console da turma: o nome em letras douradas sobre um céu de galáxia em pixel art, com a frase jogos retrô na sala de aula, roda de pen drive, sem instalar nada">
</a>

Central de jogos retrô portátil para a sala de aula. Reúne numa tela só, em
português, os emuladores de mais de 50 consoles, do Atari 2600 ao PlayStation 3 e ao
Xbox 360, e cuida do que costuma dar trabalho: achar o jogo, ajustar a imagem
ao computador, configurar o controle, guardar o progresso e juntar os
recordes da turma.

- Roda de pen drive, sem instalar nada e sem senha de administrador.
- Funciona sem internet: os computadores da sala jogam juntos pela rede local
  e trocam recordes até sem rede, levando um arquivo no pen drive.
- Feito para o notebook mais fraco da escola: a régua de desempenho é um
  Celeron N5100 (4 núcleos, sem AVX), e cada mudança é julgada por ele.
- Sem gravação de vídeo e sem transmissão ao vivo, de propósito: é usado por
  alunos menores de idade.
- Mais de 300 testes automatizados, testes de ponta a ponta com os emuladores
  de verdade e auditorias completas de qualidade, com os relatórios públicos
  em [`docs/`](https://github.com/RafaParise/arena-console/tree/main/docs).

O ARENA tem dois papéis: é um produto que a turma usa e é material de aula. O
código, em Python puro e comentado em português, é estudado em Redes, Banco
de Dados, Back-End, Front-End e Metodologias Ágeis:

| Componente | O que estudar no ARENA |
|---|---|
| Redes | A partida a dois por TCP, a descoberta dos colegas por UDP broadcast, a rede local sem roteador |
| Banco de Dados | O placar da turma em SQLite, com funções de janela (`RANK() OVER (PARTITION BY ...)`) |
| Back-End | As rotas da API HTTP, a gravação atômica, as travas de concorrência |
| Front-End | A tela em JavaScript sem framework, a acessibilidade, os estados de carregamento |
| Metodologias Ágeis | Os defeitos reais do projeto num quadro Kanban e os casos de teste que nasceram deles |

**[Ver o repositório](https://github.com/RafaParise/arena-console)** ·
**[Baixar a versão pronta](https://github.com/RafaParise/arena-console/releases/latest)**

Software livre, sob a licença GPL-3.0. O pacote traz o programa e os
emuladores; jogos, BIOS e firmware não vêm junto: são de quem tem o console.

## Tecnologias do ARENA

- **Python 3.13**, só a biblioteca padrão: servidor HTTP (`http.server`),
  banco de dados (`sqlite3`), rede (`socket`) e testes (`unittest`)
- **SQLite** para o placar, as sessões de jogo e a sincronização da turma
- **HTML, CSS e JavaScript** sem framework, com Canvas nos fundos em pixel
  art; a tela abre como janela de aplicativo no Microsoft Edge
- **RetroArch** (núcleos libretro), **PCSX2**, **Dolphin**, **RPCS3** e
  **Xenia**, configurados para rodar de dentro da pasta
- Scripts **.bat** do Windows; versionamento com **Git** e **GitHub**

## Contato e contribuições

O contato é pelo GitHub. Dúvidas, problemas e sugestões vão nas
[issues do ARENA](https://github.com/RafaParise/arena-console/issues).
Correções e melhorias são bem-vindas por pull request, seguindo as regras da
seção [Para quem programa](https://github.com/RafaParise/arena-console#para-quem-programa):
sem `pip install`, sem senha de administrador, caminhos relativos e tudo
funcionando sem internet.

As issues são públicas: não escreva nome completo, nome da escola, telefone
nem outros dados pessoais.
