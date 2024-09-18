package introducaoLogicaProgramacao.aula1

fun main() {
    val notas = listOf(0.0, 7.0, 8.0, 7.0) // Contém as notas 2.0, 7.0, 8.0, 7.0

    val quantidadeDeNotas = notas.size // Armazena a quantidade de notas. No exemplo, 4 notas
    val somaDasNotas = notas.sum() // Armazena o somatório das notas. No exemplo, 2.0 + 7.0 + 8.0 + 7.0 = 24.0
    val media = somaDasNotas / quantidadeDeNotas // Calcula a média 24.0 / 4 = 6.0

    println("A média das notas é $media")

    if (media >= 7) {
        println("Aluno aprovado")
    } else {
        println("Aluno vai para recuperação")

        // Nota da recuperação
        val notaRecuperacao = media
        

        // Nota do exame de recuperação
        val notaExameRecuperacao = 4

        // Cálculo da nova média
        val mediaRecuperacao = (notaRecuperacao + notaExameRecuperacao) / 2
        println("Média após recuperação é: $mediaRecuperacao")

        // Verificação se o aluno foi aprovado ou reprovado após recuperação
        // Considera a nota de recuperação igual a 5 como aprovação
        if (mediaRecuperacao >= 5) {
            println("Aluno aprovado após recuperação")
        } else {
            println("Aluno reprovado após recuperação")
        }
    }
}
