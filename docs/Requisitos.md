# Requisitos para o Desenvolvimento do Aplicativo de Quiz

Este documento descreve os requisitos funcionais e técnicos para o desenvolvimento de um aplicativo de quiz sobre linguagens de programação. 
Os requisitos estão organizados em formato de cards para facilitar a gestão e a alocação de tarefas para a equipe de desenvolvimento.

## Visão Geral do Projeto

*   **Nome:** Tech-Quiz
*   **Descrição:** Um aplicativo interativo nativo para Android que testa os conhecimentos do usuário em linguagens de programação.
*   **Objetivo:** Proporcionar uma experiência de quiz simples, intuitiva e otimizada para dispositivos móveis.

## Tecnologias

*   **Linguagem de Programação:** Kotlin
*   **Ambiente de Desenvolvimento:** Android Studio
*   **Ferramentas de Layout:** XML para design da interface do usuário
*   **Gerenciamento de Estado:** ViewModel (Android Architecture Components)

## Cards de Funcionalidades (User Stories)

### Card: Exibir a Pergunta e Opções

*   **Título do Card:** Exibição da Pergunta Atual
*   **Descrição:** O sistema deve exibir uma pergunta do conjunto de dados, juntamente com quatro opções de resposta. A pergunta e as opções devem ser claras e fáceis de ler.
*   **Critérios de Aceitação:**
    *   A tela deve mostrar a pergunta atual de forma destacada.
    *   Quatro botões ou cards de opções devem ser exibidos para o usuário clicar.
    *   Deve haver uma indicação visual de qual pergunta é a atual (ex: "Pergunta 1 de 5").

---

### Card: Lógica de Resposta e Feedback

*   **Título do Card:** Processamento de Resposta do Usuário
*   **Descrição:** O sistema deve capturar a seleção do usuário e verificar se a resposta está correta ou incorreta. O feedback visual deve ser imediato.
*   **Critérios de Aceitação:**
    *   Ao clicar em uma opção, os botões de resposta devem ficar desabilitados para novos cliques.
    *   A opção correta deve ser destacada visualmente (ex: cor verde com um ícone de "certo").
    *   A opção incorreta selecionada pelo usuário deve ser destacada visualmente (ex: cor vermelha com um ícone de "errado").
    *   A pontuação do usuário deve ser atualizada se a resposta for correta.

---

### Card: Navegação entre Perguntas

*   **Título do Card:** Navegação para a Próxima Pergunta
*   **Descrição:** O usuário deve ser capaz de avançar para a próxima pergunta somente após responder à pergunta atual.
*   **Critérios de Aceitação:**
    *   Um botão "Próxima Pergunta" deve aparecer após o usuário selecionar uma resposta.
    *   Ao clicar no botão, a próxima pergunta e suas opções devem ser carregadas.
    *   O botão "Próxima Pergunta" deve ser substituído por "Ver Resultado" na última pergunta.

---

### Card: Exibição da Pontuação Final

*   **Título do Card:** Tela de Pontuação Final
*   **Descrição:** Após responder a todas as perguntas, o sistema deve exibir a pontuação total do usuário e um botão para reiniciar o quiz.
*   **Critérios de Aceitação:**
    *   O quiz deve terminar após a última pergunta ser respondida.
    *   Uma nova tela deve ser exibida mostrando a pontuação final (ex: "Sua pontuação foi de X de Y").
    *   Um botão "Reiniciar Quiz" deve estar visível para o usuário começar novamente.

---

### Card: Funcionalidade de Reinício

*   **Título do Card:** Reiniciar o Quiz
*   **Descrição:** O usuário deve ser capaz de reiniciar o quiz a qualquer momento a partir da tela de pontuação final.
*   **Critérios de Aceitação:**
    *   O botão "Reiniciar Quiz" deve estar visível na tela de pontuação.
    *   Ao clicar no botão, o quiz deve ser redefinido para a primeira pergunta, a pontuação deve ser zerada e o estado do quiz deve ser resetado.

## Requisitos de Design e UX

*   O layout deve ser otimizado para dispositivos móveis, garantindo boa usabilidade em smartphones e tablets.
*   A interface deve ser limpa e visualmente agradável, com cores claras e tipografia legível.
*   Os botões e elementos interativos devem ter feedback visual ao serem pressionados.