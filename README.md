CREATE DATABASE perfil_willis;
USE perfil_willis;

-- TABELA: usuario

CREATE TABLE usuario (
    nome VARCHAR(100),
    curso VARCHAR(100),
    instituicao VARCHAR(150),
    area VARCHAR(100)
);

INSERT INTO usuario VALUES (
    'Willis Felipe Ch. Cardoso',
    'Análise e Desenvolvimento de Sistemas',
    'Instituto Federal do Norte de Minas Gerais - IFNMG',
    'Tecnologia da Informação'
);

-- TABELA: sobre_mim

CREATE TABLE sobre_mim (
    curiosidade TEXT
);

INSERT INTO sobre_mim VALUES
('Apaixonado por cães 🐶'),
('Fascinado por bugs (insetos 🐛)'),
('Menos bugs no código ❌🐞');


-- TABELA: interesses

CREATE TABLE interesses (
    id INT AUTO_INCREMENT PRIMARY KEY,
    descricao VARCHAR(100)
);

INSERT INTO interesses (descricao) VALUES
('Banco de Dados'),
('Programação'),
('Análise de Sistemas'),
('Aprendizado Contínuo');


-- TABELA: status

CREATE TABLE status (
    estado VARCHAR(50)
);

INSERT INTO status VALUES ('SELECT * FROM conhecimento WHERE aprendizado = TRUE;');


-- CONSULTA FINAL

SELECT 
    nome AS Desenvolvedor,
    curso,
    instituicao
FROM usuario;

-- Apaixonado por tecnologia. 🚀
