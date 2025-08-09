--INSERT INTO Clientes (Nome, Sobrenome, Email, AceitaComunicados, DataCadastro)
--VALUES ('Andreyna', 'Carvalho', 'drica@gmail.com', 1, GETDATE())

--SELECT * FROM Clientes
---- Where AceitaComunicados = 1
---- WHERE Nome LIKE '%T%' -- Nome começa com T e qualquer coisa no final 
--ORDER BY Nome, Sobrenome

--SELECT * FROM Clientes

--BEGIN TRAN -- Roda ele primeiro que pode desfazer se tiver feito caca
--ROLLBACK -- Volta para o que era antes da sua alteração

--UPDATE Clientes
--SET Email = 'terri@gmail.com', AceitaComunicados = 1
--WHERE Id = 2

--SELECT * FROM Clientes

DELETE Clientes
WHERE Id = 10