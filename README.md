# ProWayComputer

# manual de codigo do projeto:


Desenvolvimento do projeto ProwayComputer:

criar o projeto
ng new ProwayComputer

criar component header
ng g component header

implementação do componente de cabeçalho das paginas do projeto, esse cabeçalho se repetira em todas as paginas:


incluir icones na aplicação:

no site fontawesome.com , faça um cadastro, procure pela opção Kits, e compie a seguinte tago <script>
![image](https://user-images.githubusercontent.com/106206316/225788267-55afdc42-7ca7-4aaa-b0e8-b7f2906bbbb0.png)





<script src="https://kit.fontawesome.com/e06ef8676d.js" crossorigin="anonymous"></script>

após copiar a tág script cole a mesma no arquivo index.html 
![image](https://user-images.githubusercontent.com/106206316/225788303-80c2a62f-65fc-4b4f-9990-a9fbf34a81e8.png)




feito essa configurarção basta ir na pagina na barra de pesquisa digitar o nome da categoria do icone, como cart para carrinho de compra,  box para caixa etc, alguns icon para facilirtar o encontro, deve escrever o nome esplicito.
Exemplo:
barra de pesquisa;
![image](https://user-images.githubusercontent.com/106206316/225788363-c7b2b99a-6fc7-4b3f-826b-72093bb82a4b.png)
																				
digite cart para buscar por carrinhos, tecla enter, e selecione no resultado da busca o carrinho desejado, e na tela que abrir, copie o conteudo com a tag <i>		
		![image](https://user-images.githubusercontent.com/106206316/225788386-a4550d13-a52b-4203-addf-6891b488089d.png)
  ![image](https://user-images.githubusercontent.com/106206316/225788426-f7971627-a51c-4e11-8172-25434a1a9778.png)

											
copiado a tag <i> cole no componente onde deseja que o icone apareça:
![image](https://user-images.githubusercontent.com/106206316/225788441-c8ab09e6-bd4e-4201-a993-c0bf6e3d8670.png)

e pro nosso componente header aparecer na tela, apague todo codigo da tela inicial, no arquivo header.component.html e chame o componente header como  , <app-header> e feche a tegue do mesmo, crtl + s para salvar verifique a pagina que deve estar assim:
  
  
  ![image](https://user-images.githubusercontent.com/106206316/225788479-792aaf70-b42d-4a55-aa4e-e3be90d90bcd.png)


																										
ainda   falta estilizar o header. E paraa isso basta copiar o codigo que o professor disponibilizou no material de apoio

## seguindo em frente criaremos o compnente Footer:

ng g component footer

assim como o component header: o footer vai ter as tags os icones e os estilos, para a interface visual, 
<footer class="footer">

    <div class="footer__container">
        <section>
            <h2 class="footer__title">Sobre</h2>
            <p class="footer__about-text">What is Lorem Ipsum?
                Lorem Ipsum is simply dummy 
                Lorem Ipsum is simply dummy 
                Lorem Ipsum is simply dummy 
                
            </p>
        </section>
        <address>
        <h2 class="footer__title">Contato</h2>
        <ul>
            <li><i class="fa-solid fa-phone"></i>(00) 00000-0000</li>  
            <li><i class="fa-brands fa-square-whatsapp">(00) 00000-0000</i></li>       
            <li><i class="fa-solid fa-envelope"></i> email@email.com.br</li>  

           
            
        </ul>
    </address>
    </div>
    <section class="footer__copyright">
        &copy;Todos os direitos reservados

    </section>
</footer>



## Criando a navegação do projeto :

ainda implementaremos os devidas funcionalidade de cada componente


criar um novo modulo para a navegação: caso o mesmo não tenha sido criado junto com o projeto

ng g module app-routing --flat  --module app.module

caso crie o arquivo de roteamento, o mesmo deve ser iniciado com oseguinte codigo:

![image](https://user-images.githubusercontent.com/106206316/225788593-a5dbaba8-9632-4133-b416-b28892bcfa56.png)



após concluir essas implementações, va ate o arquivo app.component.html, e chame o seguinte componet para exibit os elementos da navegação

![image](https://user-images.githubusercontent.com/106206316/225788614-a5fb0d2e-61a3-493a-b1f4-4db95815d16e.png)









## Criar pagina de produtos:

para implementar a pagina de produtos , criaremos um modulo, chamado produtos, para trabalhar com lazy loading “carregamento preguiçoso” 

ng generate module produtos --route produtos --module app.module

ng generate module produtos // cria o modulo produtos
--route produtos // atribuit um modulo de rotiamento a produtos com o nome de produto-routing
--module app module // atribui o mudulo que esta sendo criado ao  modulo pricipal app-module

dessa forma o codigo acima cria meu modulo, adiciona no arquivo app-routing.module um path “rota de navegação” de forma automatica, e basta apenas nos fazermos o redirecionamento para que  a nossa pagina de produtos fique definida como nossa pagina inicial
  
  ![image](https://user-images.githubusercontent.com/106206316/225788697-dec92ab5-a0c2-46a1-a9fe-022307323c92.png)

















				
