**CURSO DE ANÁLISE DE DADOS - SENAC/RESILIA** <br>
**Projeto individual 1 - Módulo 3;** <br>
**Sistema RESILIADATA** <br><br>
**Matheus Augusto de Souza.** <br>
e-mail para contato: <br>
mataugusto1999@gmail.com <br>


**O que devemos fazer?** <br>
Devemos construir um modelo de banco de dados (diagrama) para representar quais são as tecnologias utilizadas <br>
pelas empresas parceiras, com o objetivo de se analisar a necessidade de alteração de stacks dos cursos <br>
oferecidos pela Resilia. <br>
<br>
**Entidades exigidas no projeto:** <br>
Devemos criar uma entidade para as empresas parceiras, uma para as tecnologias utilizadas por essas e uma <br>
entidade para a tabela que é proveniente da relação dessas duas entidades (com a cardinalidade N,N , visto <br>
que uma empresa pode possuir N tecnologias e uma tecnologia pode ser utilizada por N empresas). Além dessas <br>
podemos criar tambem uma entidade para a área tecnologica, visto que o na tecnologia deve-se selecionar qual <br>
a área da tecnologia. <br>
<br>
**Preenchimento das informações do modelo:** <br>
(2 registros para a checagem de cada entidade) <br>
------------------------------------------------------------------------------------------
# Entidade ‘Empresa_parceira’, <br>
# Atributos (CNPJ, Tecnologia, Nome, Area_atuacao, Endereco): <br>
<br>
insert into Empresa_parceira VALUES <br>
(‘121.121.121/1111-01’, ‘PowerBI’, ‘Americanas’, ‘Comércio’, ‘Av. Flores n. 200’) <br>
(‘212.212.212/2222-02’, ‘Excel’, ‘Renner’, ‘Comércio’, ‘Av. Nova York n. 240’) <br>
<br>
<br>
------------------------------------------------------------------------------------------
# Entidade ‘Tecnologia’, <br>
# Atributos (Nome, Area_tec, Tipo): <br>
<br>
insert into Tecnologia VALUES <br>
(‘Excel’, ‘Dados’, ‘Software’) <br>
(‘PowerBI’, ‘Dados’, ‘Software’) <br>
<br>
<br>
------------------------------------------------------------------------------------------
# Entidade ‘Área’. <br>
# Atributo (Nome): <br>
<br>
insert into Area VALUES  <br> 
(‘Dados’) <br>
(‘Marketing’) <br>
<br>
<br>
------------------------------------------------------------------------------------------
# Entidade ‘Tecnologia_empresa’, <br>
# Atributos (ID, CNPJ, Nome_tec): <br>
<br>
insert into Tecnologia_empresa VALUES <br>
(1, ‘121.121.121/1111-01’, ‘PowerBI’) <br>
(2, ‘212.212.212/2222-02’, ‘Excel’) <br>
<br>
<br>
