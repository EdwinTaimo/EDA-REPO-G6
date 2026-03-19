# Exercício 1: Contador de Nós
Este exercício foca-se na travessia básica de uma estrutura linear.

### Objetivo
Criar uma função que percorra toda a lista ligada e retorne o número total de elementos (nós) existentes.

### Código em C
```c
int contarTarefas(Tarefa *cabeca) {
    int contador = 0;
    Tarefa *atual = cabeca;

    while (atual != NULL) {
        contador++;
        atual = atual->proximo;
    }
    return contador;
}
