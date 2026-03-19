# Exercício 6: Verificar Lista Vazia
A forma mais simples e rápida de verificar o estado da estrutura.

### Objetivo
Implementar uma função que retorne verdadeiro (1) se a lista não contiver elementos.

### Código em C
```c
int estaVazia(Tarefa *cabeca) {
    return (cabeca == NULL);
}
