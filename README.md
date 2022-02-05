# 1040V2.py
Questão 1040 BeeCrowd


provas = input().split(' ')

nota1 = float(provas [0])
nota2 = float(provas [1])
nota3 = float(provas [2])
nota4 = float(provas [3])

media = ((nota1 * 2) + (nota2 * 3) + (nota3 * 4) + (nota4 * 1)) / 10
print(f"Media: {media:.1f}")

if media >= 7:
    print("Aluno aprovado.")
else:
    if (media > 5) and (media <= 6.99):
        print("Aluno em exame.")
        recuperacao = float(input())
        print(f"Nota do exame: {recuperacao:.1f}")
        media_final = (media + recuperacao) / 2
        print(f"Media: {media_final:.1f}")
        if media_final >= 5:
            print("Aluno aprovado.")
        else:
            print("Aluno reprovado.")
    else:
        if media < 5:
            print("Aluno reprovado.")
