# Projeto
Nesse projeto, apliquei os conhecimentos aprendidos em aula para a criacao de script em JS de um arquivo de reembolso

## Alteracao do input
- remocao dos caracteres numericos com Regex
- Transformar o valor para centavos
- chamar a funcao que vai formatar o dinheio do input conforme a localidade, usando formatCurrencyBRL

### configuracao do input que transforma o dinheiro para PT-BR
Criacao de uma funcao que vai formatar o input para transformar o valor do input pra pt-BR
- utilizacao do toLocaleString("pt-BR")
- uso de style: "Currency" e Currency: "BRL"
- return do valor formatado para chamar a funcao e o resultado vir

## Captura do evento de submit do formulario
objetivo é capturar os valores que vao ser utilizados para outras funcoes e alteracoes
- Prevencao do comportamento padrao de recarregar a pagina com event.preventDefault()
- criacao de um objeto com os detalhes da despesa
-chamar a funcao que adiciona o item na lista

## Adicionar um novo item na lista com a funcao expenseAdd(newExpense)
- criacao de elemento para adicionar item (li) na lista (ul) com createElement
- Criacao do icone da categoria com createElement e depois uso do setAttribute para usar o arquivo de imagem e nome da categoria conforme a selecao
- Cria a info da despesa com o createElement para criar o div
- Criacao do nome da despesa com createElement pra colocar o strong
- Criacao da categoria de despesa com createElement para o span
- Adicao do nome e da categoria na div das informacoes da despesa com expenseInfro.append(expenseName, expenseCategory)
-criacao do valor da despesa com a criacao de elementos que a despesa esta inserida, com createElement, adicao de class e adicao de HTML co innerHTML
-Criacao do icode de remover com createElement, adicao de classe com classList e colocar atributos para remover com setAttribute
- adicao de informacoes no item 
- Adicao do iten na lista
- Limpeza de formulario para um novo item
- Atualiza os totais

## Funcao que atualiza os totais
- Recuperacao dos itens de li e da lista ul
- atualizacao da quantidade de itens da lista para deixar no singular ou plural com text.content
- uso do for para cada item da lista transformar os caracteres nao numericos e substituir a , pelo .
- incrimento do valor tottal
- criacao do span para formatar o R$, remocao do R$ exibido automatico, limpa o conteudo do elemento e adicionar o elemento de valor formatado

## evento que captura o clique nos itens da lista 
- uso do addEventListener com click para identificar onde o usuario clicar
- se o elemento clicar for o icone de remover, ira emover, obtencao da li pai do elemento clicado e remocao do item. Por fim faz o update do total

## Funcao clear para quando o usuario enviar, deixar os campos gratis
