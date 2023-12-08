Projeto de programação mobile. Integrantes: Mariana Magalhães, Emanuelle dos Santos Miranda e Thais Batista da Paixão. SQL: 

-- phpMyAdmin SQL Dump
-- version 5.2.1
-- https://www.phpmyadmin.net/
--
-- Host: 127.0.0.1
-- Tempo de geração: 08-Dez-2023 às 03:47
-- Versão do servidor: 10.4.32-MariaDB
-- versão do PHP: 8.2.12

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Banco de dados: `bdatividade`
--

-- --------------------------------------------------------

--
-- Estrutura da tabela `usuario`
--

CREATE TABLE `usuario` (
  `Email` varchar(30) NOT NULL,
  `Nome` varchar(10) NOT NULL,
  `Sobrenome` varchar(80) NOT NULL,
  `Usuario` varchar(20) NOT NULL,
  `Senha` varchar(25) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Extraindo dados da tabela `usuario`
--

INSERT INTO `usuario` (`Email`, `Nome`, `Sobrenome`, `Usuario`, `Senha`) VALUES
('Admin@', 'Thais', 'Paixao', 'Admin', '0000'),
('carlosdias5@hotmail.com', 'Carlos', 'Dias', 'Carl', 'usyreq99e'),
('Exemplo@hotmail.com', 'Ex', 'Exemplo', 'Example', 'ex123'),
('matheus@hotmail.com', 'Matheus', 'Andrade', 'Theus', '24re5435'),
('PedroCarlos@gmail.com', 'Pedro', 'Carlos', 'PedrinhoCarlos', 'pedrocarlos');

--
-- Índices para tabelas despejadas
--

--
-- Índices para tabela `usuario`
--
ALTER TABLE `usuario`
  ADD PRIMARY KEY (`Email`);
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;

