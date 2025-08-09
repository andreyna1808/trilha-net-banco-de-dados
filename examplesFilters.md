SELECT COUNT(*) FROM Produtos -- CONTA E RETORNA APENAS O NÚMERO/QUANTIDADE DE DADOS EXISTENTES

SELECT COUNT(*) FROM Produtos WHERE Tamanho = 'M' -- Filtro para saber a quantidade de algo, QUANDO

SELECT SUM(Preco) PrecoTotal FROM Produtos -- Soma tudo de alguma coluna

SELECT MAX(Preco) FROM Produtos -- Pega o valor máximo

SELECT MIN(Preco) FROM Produtos --Pega o valor mínimo

SELECT AVG(Preco) FROM Produtos -- Média do produto / average

SELECT Nome + ' ' + Cor FROM Produtos -- Também dá para concatenar o retorno

SELECT UPPER(Nome) NomeUpper, LOWER(Cor) LowerCor FROM Produtos -- Maiusc/Minusc

SELECT * FROM Produtos

ALTER TABLE Produtos ADD DataCadastro DATETIME2 -- ADICIONA A COLUNA

UPDATE Produtos SET DataCadastro = GETDATE() -- Atualiza a coluna

ALTER TABLE Produtos DROP COLUMN DataCadastro -- APAGAR A COLUNA

SELECT FORMAT(DataCadastro, 'dd-MM-yyyy HH:mm') Data FROM Produtos

SELECT
Tamanho, COUNT(*) Quantidade
FROM Produtos
WHERE Tamanho <> '' -- Se tamanho for diferente de vazio
GROUP BY Tamanho
ORDER BY Quantidade DESC