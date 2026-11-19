>> [Versão em Inglês do Projeto](https://github.com/ldov/BlindCheck/blob/main/README.md)

---

# BlindCheck — Blind AI Evaluator Game

Um jogo casual de avaliação às cegas onde jogadores comuns testam, inspecionam e identificam falhas em respostas geradas por modelos de Inteligência Artificial.

## O que é o Jogo?

O **BlindCheck** (Caça ao Erro) transforma o controle de qualidade de Inteligência Artificial em uma experiência rápida, acessível e gamificada.

Em vez das tradicionais comparações lado a lado (Modelos A vs. B), o jogador recebe uma **única resposta** gerada por uma IA misteriosa para uma tarefa ou pergunta sorteada aleatoriamente. O papel do jogador é atuar como um inspetor de qualidade: ler a interação e decidir se a resposta passou no teste ou se contém alguma falha (como informações inventadas, fuga do tema, excesso de enrolação ou tom artificial).

A cada missão concluída, o jogador acumula pontos, sobe de nível, mantém sequências de acertos e descobre qual modelo de IA estava por trás daquela resposta.

## Como Funciona o Programa

O fluxo do sistema é dividido em quatro etapas simples e contínuas:

1. **Sorteio Aleatório (Teste às Cegas):** Ao iniciar uma missão, o sistema seleciona aleatoriamente uma pergunta/tarefa de um banco de desafios e sorteia um modelo de IA disponível para gerar a resposta. A identidade do modelo permanece oculta durante toda a avaliação para eliminar qualquer viés de marca.

2. **Inspeção pelo Jogador:** A pergunta e a resposta são exibidas na tela. O jogador avalia a utilidade e a qualidade do conteúdo, indicando se a resposta está correta ou apontando os erros encontrados por meio de categorias rápidas e intuitivas (com opção de comentário curto).

3. **Gamificação e Revelação:** Após enviar o veredito, o jogador recebe pontos pela missão (com bônus para feedbacks detalhados e consistência), visualiza seu progresso e descobre qual modelo de IA acabou de avaliar.

4. **Estruturação dos Dados:** Cada rodada concluída gera um registro completo contendo o identificador do avaliador, a tarefa sorteada, o modelo utilizado, a resposta gerada e os feedbacks detalhados — armazenados de forma estruturada (em JSON ou banco de dados) e prontos para análise.

## Objetivo do Projeto

O objetivo principal do **BlindCheck** é capturar **feedbacks humanos reais, granulares e livres de viés** sobre o desempenho de modelos de Inteligência Artificial em situações cotidianas.

Enquanto métricas tradicionais apenas indicam qual modelo foi preferido em uma disputa, este projeto foca em **diagnosticar o motivo exato das falhas** sob a ótica de usuários comuns (não apenas especialistas técnicos). Os dados coletados servem como insumo estratégico para empresas e pesquisadores de IA que buscam:

* Identificar padrões de alucinação, falhas de raciocínio e falta de naturalidade no idioma;

* Avaliar modelos em cenários imprevisíveis e variados;

* Alimentar pipelines de melhoria contínua, ajuste fino (Fine-Tuning) e alinhamento com preferências humanas (RLHF / DPO);

* Escalar futuramente a mesma mecânica de inspeção para avaliações multimodais (áudio e imagem).
