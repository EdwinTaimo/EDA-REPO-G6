# Exercício 2: Filtrar Tarefas Pendentes
Aplica lógica condicional durante a iteração de uma lista.

### Objetivo
Imprimir no ecrã apenas as tarefas cujo campo `concluida` seja igual a 0.

### Código em C
```c
void listarPendentes(Tarefa *cabeca) {
    Tarefa *atual = cabeca;
    printf("Tarefas Pendentes:\n");
    
    while (atual != NULL) {
        if (atual->concluida == 0) {
            printf("- %s\n", atual->descricao);
        }
        atual = atual->proximo;
    }
}
