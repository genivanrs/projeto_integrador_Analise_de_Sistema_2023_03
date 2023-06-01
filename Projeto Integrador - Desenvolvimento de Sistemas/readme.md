# PROJETO INTEGRADOR DESENVOLVIMENTO DE SISTEMAS – QUAIS 
# PRÓS E CONTRAS DE SE TER UM SISTEMA DA INFORMAÇÃO DE GESTÃO 
# DE DADOS E INTERNET VISANDO O LADO FRONT ENT (CLIENTE) 
# TRABALHO NO RAMO VAREJISTA (LOJAS SIMONETTI LTDA) DO ESPIRITO SANTO
# Instruido pelo professor Edilson Rodrigues
# Atraves da Universidade Santo Amaro - UNISA
O Código foi desenvolvido para ser rodado dentro de uma mikrotik ou equipamento que gerencie um hotspot, 
Assim que o cliente clica na rede Conexão Simonetti, o mesmo e redirecionado para uma pagina de login
onde o mesmo deverá entrar com seus dados... após clicar em enviar o mesmo ja esta navegando... Caso este
cliente volte a loja / filial o mesmo não precisará utilizar / refazer o cadastro, pois o sistema utiliza cookies 
que grava e vincula o MAC do aparelho ao Nome / CPF e refaz o logim automaticamente...
Em paralelo,as informações deste cliente sobe para a nossa base de dados que e possivel acessar via navegador web
e através dele temos a quantidade de clientes cadastrados, feedbacks, controle de banda para cada perfil 9 no nosso sistema criamos dois: 1º Padrão, este todos que fazem o cadastro inicialmente recebe este perfil... O mesmo tem um limite de 2 horas diarias e 2 mb/s para utilizar, o 2º Funcionario, que não tem limite de horas, e a banda e de 5 mb/s;
# Do funcionamento do codigo dentro da Routerbiard Mikrotik
O codigo e adicionado em files e e interligado com o hotspot, assim que o cliente clica na rede o hotspot redireciona para as paginas do codigo que esta em files, após isso os dados são salvos na base de dados assim que o cliente clica em salvar / entar;
# Da configuração da Unifi
Utilizamos a Unifi para entregar o sinal de wifi para nossa matriz e filial, onde me media cada loja tem uma unifi por piso, a mesma e vinculada no nosso DHCP server da routerboard mikrotik onde a unifi recebe uma velan criada na routerboar ( que por padrão recebe o numero da loja Ex.: 2+Nº da loja - ficando assim 226 onde 26 e a filial 26 de Porto Seguro);
# Facilidade de acesso pelo cliente
Nas fliais foram distribuidos placas com um QR code, assim que o cliente lê o mesmo ele e redirecionado para a pagina de login;