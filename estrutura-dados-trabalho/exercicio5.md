# Exercício 5: Inserir no Início (Push)
Diferença entre inserir no início vs. inserir no fim da lista.

### Objetivo
Criar uma função que adicione uma nova tarefa como o primeiro elemento da lista, o que é mais eficiente ($O(1)$) do que percorrer tudo até ao fim.

### Código em C
```c
void inserirNoInicio(Tarefa **cabecaRef, char *desc) {
    Tarefa *nova = (Tarefa*)malloc(sizeof(Tarefa));
    strcpy(nova->descricao, desc);
    
    nova->proximo = (*cabecaRef); // A nova aponta para a antiga cabeça
    (*cabecaRef) = nova;         // A cabeça agora é a nova tarefa
}
