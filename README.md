# Análise-de-dados-Pessoas-em-situção-de-Rua
Esse estudo faz parte de uma iniciativa para detectar pessoas em situação de rua em diferentes regiões, entender suas circunstâncias e as razões que as levaram a essa situação. O objetivo é identificar os locais com maior concentração de pessoas em situação de rua para que possam receber a devida ajuda.

Para isso crie uma base de dados Fictícia com as seguintes colunas :

CREATE DATABASE Ronda;
USE Ronda ;

CREATE TABLE PessoasEmSituacaoDeRua (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(50),
    idade INT,
    genero VARCHAR(10),
    tempo_na_rua VARCHAR(20),
    motivo_situacao_rua VARCHAR(255),
    saude_mental VARCHAR(50),
    saude_fisica VARCHAR(50),
    dependentes VARCHAR(50),
    educacao VARCHAR(50),
    habilidades_profissionais VARCHAR(100),
    localizacao_atual VARCHAR(100),
    zona VARCHAR(50) 
    );
    
    INSERT INTO PessoasEmSituacaoDeRua (nome, idade, genero, tempo_na_rua, motivo_situacao_rua, saude_mental, saude_fisica, dependentes, educacao, habilidades_profissionais, localizacao_atual, zona) VALUES
('João Silva', 45, 'M', '2 anos', 'Perda de emprego e dificuldades econômicas', 'Estável', 'Hipertensão', 'Nenhum', 'Ensino Médio', 'Carpinteiro', 'São Paulo, SP', 'Zona Sul'),
('Maria Souza', 32, 'F', '1 ano', 'Problemas de saúde mental', 'Depressão', 'Boa', '1 filho', 'Ensino Superior', 'Administradora', 'Rio de Janeiro, RJ', 'Zona Norte'),
('Carlos Lima', 27, 'M', '3 meses', 'Rompimento de relacionamentos familiares', 'Ansiedade', 'Boa', 'Nenhum', 'Ensino Médio', 'Vendedor', 'Belo Horizonte, MG', 'Zona Norte'),
('Ana Pereira', 50, 'F', '4 anos', 'Despejo devido a dívidas', 'Estável', 'Diabetes', '2 filhos', 'Ensino Fundamental', 'Dona de casa', 'Salvador, BA', 'Zona Sul'),
('José Santos', 40, 'M', '5 anos', 'Dependência química', 'Esquizofrenia', 'Boa', 'Nenhum', 'Ensino Fundamental', 'Eletricista', 'Fortaleza, CE', 'Zona Norte'),
('Beatriz Costa', 22, 'F', '6 meses', 'Fugiu de violência doméstica', 'PTSD', 'Boa', 'Nenhum', 'Ensino Médio', 'Estudante', 'Curitiba, PR', 'Zona Sul'),
('Pedro Alves', 36, 'M', '2 anos', 'Falência e perda de bens', 'Estável', 'Obesidade', '1 filho', 'Ensino Médio', 'Comerciante', 'Porto Alegre, RS', 'Zona Sul'),
('Carolina Dias', 28, 'F', '1 ano', 'Desemprego e falta de suporte social', 'Ansiedade', 'Boa', 'Nenhum', 'Ensino Superior', 'Enfermeira', 'Recife, PE', 'Zona Norte'),
('Marcos Ferreira', 38, 'M', '1 ano', 'Despejo devido a violência', 'Estável', 'Boa', 'Nenhum', 'Ensino Médio', 'Motorista', 'Brasília, DF', 'Zona Norte'),
('Tatiana Rodrigues', 26, 'F', '8 meses', 'Rompimento de relacionamento abusivo', 'Depressão', 'Boa', 'Nenhum', 'Ensino Médio', 'Assistente administrativa', 'São Luís, MA', 'Zona Sul'),
('Luiz Fernando Melo', 49, 'M', '3 anos', 'Perda de emprego e saúde precária', 'Ansiedade', 'Diabetes', '1 filho', 'Ensino Fundamental', 'Pedreiro', 'Manaus, AM', 'Zona Sul'),
('Daniela Oliveira', 33, 'F', '2 anos', 'Problemas financeiros e familiares', 'Estável', 'Boa', '2 filhos', 'Ensino Superior', 'Professora', 'Florianópolis, SC', 'Zona Norte'),
('Felipe Almeida', 29, 'M', '6 meses', 'Dependência química e falta de suporte', 'Estável', 'Boa', 'Nenhum', 'Ensino Médio', 'Técnico em informática', 'Goiânia, GO', 'Zona Norte'),
('Gustavo Martins', 41, 'M', '1 ano', 'Perda de emprego e saúde mental', 'Depressão', 'Boa', 'Nenhum', 'Ensino Superior', 'Contador', 'Campinas, SP', 'Zona Norte'),
('Fernanda Alves', 35, 'F', '3 anos', 'Violência doméstica', 'PTSD', 'Boa', '1 filha', 'Ensino Médio', 'Cabeleireira', 'Natal, RN', 'Zona Sul'),
('Roberto Nascimento', 52, 'M', '6 meses', 'Despejo devido a dívidas', 'Estável', 'Hipertensão', 'Nenhum', 'Ensino Fundamental', 'Segurança', 'Belém, PA', 'Zona Norte'),
('Patrícia Costa', 29, 'F', '8 meses', 'Rompeu com família', 'Ansiedade', 'Boa', 'Nenhum', 'Ensino Médio', 'Garçonete', 'Vitória, ES', 'Zona Sul'),
('Ricardo Mendes', 44, 'M', '4 anos', 'Dependência química', 'Esquizofrenia', 'Boa', 'Nenhum', 'Ensino Fundamental', 'Pintor', 'Maceió, AL', 'Zona Norte'),
('Larissa Fonseca', 23, 'F', '1 ano', 'Fuga de violência doméstica', 'Ansiedade', 'Boa', 'Nenhum', 'Ensino Médio', 'Estudante', 'Teresina, PI', 'Zona Sul'),
('Eduardo Ramos', 37, 'M', '2 anos', 'Falência empresarial', 'Estável', 'Boa', '2 filhos', 'Ensino Superior', 'Advogado', 'Aracaju, SE', 'Zona Norte'),
('Renata Machado', 31, 'F', '5 anos', 'Dependência química', 'Ansiedade', 'Boa', 'Nenhum', 'Ensino Médio', 'Recepcionista', 'João Pessoa, PB', 'Zona Sul');
![Screenshot 2025-02-27 080226](https://github.com/user-attachments/assets/bad2ac99-d0ed-408b-980a-dfa7942a527c)
