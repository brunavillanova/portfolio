# portfolio
----------------------------------------HTML--------------------------------------------------------------------------------------------------
Metadados e Configurações: Definição de codificação, folha de estilos, script JavaScript e uso da fonte Awesome para ícones.

Cabeçalho e Navegação: Barra de navegação com links para seções como "Inicio", "Avaliações" e "Contato". Ícone de menu para dispositivos móveis.

Seção de Destaque: Título e slogan para apresentar as melhores estampas de rock do Brasil.

Seção de Tipos de Estampas: Exibição de diferentes tipos de camisetas de bandas de rock com imagens, nomes e links de compra.

Seção de Avaliações: Depoimentos de clientes com imagens e classificações de estrelas, compartilhando opiniões positivas sobre as camisetas.

Seção de Contato: Formulário para os visitantes entrarem em contato, com campos para nome, e-mail e mensagem.

Rodapé: Declaração de direitos autorais.

Recursos Externos: Uso de jQuery e script "main.js" para funcionalidades extras.

Responsividade: Considerações para dispositivos móveis, com um ícone de menu para navegabilidade.

Melhorias Possíveis: Sugestões incluem verificar tags de fechamento, adicionar mais informações sobre as camisetas, como descrições e preços, e possivelmente incluir uma seção de busca.

-----------------------------------------------------CSS---------------------------------------------------------------------------------------------------------------------------

Configuração Geral:

Definição do tamanho da fonte em porcentagem para facilitar a responsividade.
Estilo de reset para elementos HTML padrão.
Fontes:

Importação da fonte "Poppins" do Google Fonts para uso no site.
Definição da fonte padrão para o corpo do site como "Poppins" e fonte de fallback "sans-serif".
Estilos de Botão:

Estilização para botões, incluindo cor de fundo, tamanho, borda e transições para efeito de destaque.
Barra de Navegação:

Estilos para a barra de navegação, incluindo sombra, cores de fundo e texto.
Estilização do ícone de menu para dispositivos móveis.
Seção de Destaque:

Estilos para a seção de destaque com imagem de fundo, tamanho, posição e repetição.
Estilização para o título da seção.
Seção de Tipos de Estampas:

Estilos para a seção que exibe diferentes tipos de camisetas.
Estilização para imagens, container e botões de compra.
Seção de Avaliações:

Estilização para a seção de depoimentos, incluindo cor de fundo e tamanho de fonte.
Seção de Contato:

--------------------------------------------------JS-----------------------------------------------------------------------------------------------
$(document).ready(function () { ... });:

Isso envolve todo o código em uma função que será executada assim que o documento HTML estiver totalmente carregado e pronto.
$("a").on("click", function (event) { ... });:

Isso seleciona todos os elementos de âncora (<a>) na página e define um evento de clique para eles.
if (this.hash !== "") { ... }:

Verifica se o atributo hash do link clicado não está vazio. O hash é a parte da URL que segue o símbolo "#", comumente usado para referenciar seções específicas na página.
event.preventDefault();:

Impede o comportamento padrão do link, que é navegar para outra página ou seção.
var hash = this.hash;:

Armazena o valor do atributo hash do link clicado na variável hash.
$("html, body").animate({ ... }, 800, function () { ... });:

Usa a função animate() do jQuery para criar uma animação de rolagem suave.
$("html, body") seleciona tanto o elemento <html> quanto o <body> para garantir que a animação funcione em diferentes navegadores.
.animate(...) configura a animação.
{ scrollTop: $(hash).offset().top } define a posição final da rolagem, usando o valor da posição superior (offset().top) do elemento referenciado pelo hash.
800 é a duração da animação em milissegundos (nesse caso, 800ms).
A função dentro da animação { ... } é chamada quando a animação é concluída. Nesse caso, ela atualiza a URL com o hash usando window.location.hash = hash;.

Estilos para a seção de contato, incluindo fundo, layout e tamanhos de fonte.
Rodapé:

Estilos para o rodapé, incluindo cor de fundo, tamanho de fonte e cor do texto.
Media Queries:

Adaptação de estilos com base na largura da tela, orientação e altura.
