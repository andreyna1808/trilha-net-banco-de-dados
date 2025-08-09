--CREATE TABLE Enderecos (
--	Id int PRIMARY KEY IDENTITY(1,1) NOT NULL, -- Implementado de um a um e que seja unico
--	IdClient int NULL,
--	Rua varchar(255) NULL,
--	Bairro varchar(255) NULL,
--	Cidade varchar(255) NULL,
--	Estado char(2) NULL,

--	CONSTRAINT FK_Enderecos_Clientes FOREIGN KEY(IdClient) -- Tem uma restrição que é uma chave estrangeira
--	REFERENCES Clientes(Id)
--)

--INSERT INTO Enderecos VALUES(4,'Rua teste','Bairro teste','Cidade Teste','SP')

SELECT * FROM Enderecos

SELECT * FROM Clientes
INNER JOIN Enderecos ON Clientes.Id = Enderecos.IdClient -- Juntar os endereços e clientes se o client.ID = ao endereço do IdClient
WHERE Clientes.Id = 4