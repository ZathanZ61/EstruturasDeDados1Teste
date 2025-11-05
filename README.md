Este código implementa um contador de "b"s consecutivos no final de uma cadeia, usando um Autômato Finito Determinístico (AFD).
A Memória (Estados): O AFD usa quatro estados (q0 a q3) para "lembrar" quantos 'b's consecutivos foram lidos por último. Por exemplo, q2 significa que a cadeia terminou em 'bb'.
Regra principal Sempre que o autômato lê um 'b', ele avança para o próximo estado (aumenta o contador).
Sempre que lê um 'a' ou 'c', ele reseta o contador, voltando imediatamente ao estado inicial (q0).

Resultado: Após processar a cadeia inteira, se o autômato estiver no estado final q3 (ou seja, o contador atingiu 3 e não foi resetado), a cadeia é aceita. Caso contrário, é rejeitada. Esse não tem inserção interativa de dados. Ele é executado diretamente, passando as cadeias de teste como argumentos fixos para a função
