# embarcatech_2025_u4c5_-atividade_1

#  O projeto de um semáforo com temporização periódica utilizando o microcontrolador Raspberry Pi Pico W e a função add_repeating_timer_ms() do Pico SDK. O objetivo deste trabalho é demonstrar como controlar LEDs para alternar entre os sinais vermelho, azul e verde a cada 3 segundos, garantindo uma simulação realista de um semáforo utilizando o simulador Wokwi e a ferramenta educacional BitDogLab.Esta tarefa envolve um sinal luminoso conectado às interfaces GPIO 11, 12 e 13, que altera seu estado a cada 3 segundos. Garantindo uma simulação realista de um semáforo utilizando o simulador wokwi e a ferramenta educacional BitDogLab.
# Ao realizar testes na placa BitDogLab, os LEDs acenderam na sequência esperada, porém, devido à ausência de um LED na cor amarela,conforme orientado pelo professor para torcar pelo Led de cor azul, não foi exatamente igual ao da simulação, no entanto, a tarefa realizada foi um sucesso!

# Explicação do Funcionamento O projeto foi configurado para alternar automaticamente entre os estados do semáforo com base em um temporizador periódico. Cada estado é representado por um LED diferente:
1) LED VERMELHO: Indica parada e é o estado inicial.
2) LED AZUL: Indica atenção e prepara para a troca de estado.
3) LED VERDE: Indica permissão para avançar.
4) A transição ocorre a cada 3 segundos utilizando a função repeating_timer_callback(), que altera o estado dos LEDs de forma sequencial.

# Configuração e Implementação
1) O código foi desenvolvido no VS Code utilizando o Pico SDK.
2) A simulação foi realizada no Wokwi, permitindo validar a lógica do semáforo antes da implementação no hardware real.
3) No BitDogLab, o projeto foi testado utilizando um LED RGB, onde os GPIOs 11, 12 e 13 representam os estados do semáforo.

# Objetivos
1) Entender e aplicar a função add_repeating_timer_ms() do Pico SDK para criar temporizações periódicas em microcontroladores.
2) Desenvolver um semáforo funcional, alternando entre os sinais vermelho, amarelo e verde com um intervalo fixo de 3 segundos.
3) Implementar a lógica de controle dos LEDs utilizando uma função de call-back para gerenciar as transições de estado.
4) Configurar o sistema para enviar mensagens pela porta serial a cada segundo, permitindo o monitoramento em tempo real do funcionamento do semáforo.
5) Validar a implementação por meio da simulação no Wokwi e da experimentação prática no BitDogLab, utilizando um LED RGB nos GPIOs 11, 12 e 13 para representar os sinais do semáforo.

# Resultados Obtidos
1) A função add_repeating_timer_ms() foi aplicada com sucesso para criar a temporização periódica, garantindo a troca automática dos sinais do semáforo a cada 3 segundos.
2) O semáforo foi implementado corretamente, iniciando na cor vermelha e alternando sequencialmente para amarelo e verde, respeitando o intervalo definido.
3) A função de call-back foi utilizada para gerenciar a mudança de estado dos LEDs, garantindo uma transição precisa e previsível entre as cores.
4) A estrutura de repetição while foi configurada para enviar mensagens à porta serial a cada 1 segundo, permitindo a monitorização em tempo real do funcionamento do sistema.
5) A simulação no Wokwi confirmou a operação correta do sistema, e os testes práticos no BitDogLab com o LED RGB nos GPIOs 11, 12 e 13 demonstraram que a abordagem também funciona em hardware real.

# Segue o link da atividade 1 : https://drive.google.com/file/d/1QzHGfhVbpD3OK5WTtMeYackQ0JT87B1U/view?usp=sharing

# Conclusão
A implementação do temporizador periódico utilizando a função add_repeating_timer_ms() no Raspberry Pi Pico W permitiu a simulação eficaz de um semáforo funcional, garantindo a alternância precisa entre os sinais vermelho, amarelo e verde a cada 3 segundos. A utilização da função de call-back assegurou uma transição automatizada e eficiente dos LEDs, enquanto a exibição de mensagens na porta serial possibilitou o monitoramento em tempo real do funcionamento do sistema.

Além disso, a simulação no Wokwi e os testes no BitDogLab comprovaram a validade da abordagem, demonstrando que o código desenvolvido pode ser facilmente aplicado tanto em ambientes simulados quanto em hardware real. Dessa forma, a atividade permitiu fixar conceitos fundamentais sobre temporização, manipulação de LEDs e integração de software com hardware, consolidando o aprendizado sobre sistemas embarcados e programação para microcontroladores.

