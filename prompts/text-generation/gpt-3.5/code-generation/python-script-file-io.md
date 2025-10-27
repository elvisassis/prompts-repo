# python-script-file-io.md

# 📝 Script Python (Entrada/Saída de Arquivo)

## Descrição
Este prompt é usado para gerar scripts Python focados em operações de arquivo (Input/Output - I/O), como leitura, escrita, manipulação de dados em arquivos CSV, TXT ou JSON.

## Estrutura do Prompt
**Exemplo:**
- Escreva um script Python que leia um arquivo chamado `dados.txt`. O script deve contar quantas linhas o arquivo possui e imprimir o resultado no console. Certifique-se de fechar o arquivo corretamente.

## Resultado Esperado
```python
def contar_linhas(nome_arquivo):
    try:
        with open(nome_arquivo, 'r') as arquivo:
            contador = 0
            for linha in arquivo:
                contador += 1
            print(f"O arquivo {nome_arquivo} possui {contador} linhas.")
    except FileNotFoundError:
        print(f"Erro: O arquivo {nome_arquivo} não foi encontrado.")

contar_linhas("dados.txt")