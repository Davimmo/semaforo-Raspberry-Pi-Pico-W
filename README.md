# Projeto Semáforo - EmbarcaTech

## Sobre o Projeto
Este projeto implementa a lógica de um semáforo utilizando a Raspberry Pi Pico. O código controla LEDs para representar os sinais vermelho, amarelo e verde, alternando entre eles a cada ciclo de tempo definido. Foi desenvolvido no âmbito do **EmbarcaTech** por **Davi Bezerra Cavalcanti**.

## Requisitos
Para compilar e executar este projeto, são necessárias as seguintes ferramentas:

## Extenções para o VS Code
- **Wokwi**
- **CMake**
- **Raspberry Pi Pico Project**

## Estrutura do Código
O código está dividido em duas pastas principais:

- **BitDogLab:** Contém o código adaptado para a placa BitDogLab.
- **Simulacao:** Contém os arquivos necessários para simulação no Wokwi.

O código está organizado da seguinte forma:

- **Bibliotecas:**
  - `led.h`: Manipulação de LEDs.
  - `button.h`: Manipulação de botões.
  - `interrupt.h`: Manipulação de eventos de interrupção.
- **Macros e Variáveis Globais:**
  - `volatile uint8_t cycle`: Controla o estado atual do semáforo.
- **Função de Timer:**
  - `repeating_timer_callback()`: Alterna o estado do semáforo a cada 3 segundos.
- **Função `main()`:**
  - Inicializa os LEDs e o botão.
  - Configura a interrupção do botão.
  - Configura e inicia um temporizador para alternar os estados do semáforo.
  - Entra em um loop infinito exibindo mensagens no console a cada segundo.

## Como Compilar e Executar
1. Certifique-se de ter o ambiente de desenvolvimento do Raspberry Pi Pico configurado.
2. Clone este repositório:
   ```sh
   git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/Davimmo/semaforo-Raspberry-Pi-Pico-W.git)
   ```
3. Importe o projeto utilizando as pastas BitDogLab ou Simulacao
   
4. Compile o projeto utilizando a extensão para Raspberry Pi Pico

5. Transfira o binário gerado para a Raspberry Pi Pico e realize seus testes.


---
**Nota:** Este projeto faz parte do programa EmbarcaTech e foi desenvolvido para fins educacionais e experimentação com a Raspberry Pi Pico.

