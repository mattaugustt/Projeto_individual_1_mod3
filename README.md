**CURSO DE ANÁLISE DE DADOS - SENAC/RESILIA** <br>
**Projeto individual 1 - Módulo 3;** <br>
**Sistema RESILIADATA** <br><br>
**Matheus Augusto de Souza.** <br>
e-mail para contato: <br>
mataugusto1999@gmail.com <br>


*** O que devemos fazer? ** <br>
Devemos construir um modelo de banco de dados (diagrama) para representar quais são as tecnologias utilizadas <br>
pelas empresas parceiras, com o objetivo de se analisar a necessidade de alteração de stacks dos cursos <br>
oferecidos pela Resilia.

*** Entidades exigidas no projeto: **
Devemos criar uma entidade para as empresas parceiras, uma para as tecnologias utilizadas por essas e uma <br>
entidade para a tabela que é proveniente da relação dessas duas entidades (com a cardinalidade N,N , visto <br>
que uma empresa pode possuir N tecnologias e uma tecnologia pode ser utilizada por N empresas). Além dessas <br>
podemos criar tambem uma entidade para a área tecnologica, visto que o na tecnologia deve-se selecionar qual <br>
a área da tecnologia. 

** Preenchimento das informações do modelo: **
(2 registros para a checagem de cada entidade)
------------------------------------------------------------------------------------------
# Entidade ‘Empresa_parceira’,
# Atributos (CNPJ, Tecnologia, Nome, Area_atuacao, Endereco):

insert into Empresa_parceira VALUES
(‘121.121.121/1111-01’, ‘PowerBI’, ‘Americanas’, ‘Comércio’, ‘Av. Flores n. 200’)
(‘212.212.212/2222-02’, ‘Excel’, ‘Renner’, ‘Comércio’, ‘Av. Nova York n. 240’)


------------------------------------------------------------------------------------------
# Entidade ‘Tecnologia’,
# Atributos (Nome, Area_tec, Tipo):

insert into Tecnologia VALUES
(‘Excel’, ‘Dados’, ‘Software’)
(‘PowerBI’, ‘Dados’, ‘Software’)


------------------------------------------------------------------------------------------
# Entidade ‘Área’.
# Atributo (Nome):

insert into Area VALUES 
(‘Dados’)
(‘Marketing’)


------------------------------------------------------------------------------------------
# Entidade ‘Tecnologia_empresa’,
# Atributos (ID, CNPJ, Nome_tec):

insert into Tecnologia_empresa VALUES
(1, ‘121.121.121/1111-01’, ‘PowerBI’)
(2, ‘212.212.212/2222-02’, ‘Excel’)

