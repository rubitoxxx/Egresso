# 🎓 EGRESSO

[![Badge - Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white)](https://www.java.com/)
[![Badge - Ant](https://img.shields.io/badge/Ant-02303A?style=for-the-badge)]()
[![Badge - NetBeans](https://img.shields.io/badge/NetBeans-0082C9?style=for-the-badge&logo=netbeans&logoColor=white)]()

> Projeto desenvolvido para a gestão de egressos com integração de ferramentas de build utilizando **Ant** e **NetBeans**.

---

## 📌 Visão Geral

Este projeto tem como objetivo o gerenciamento de egressos, incluindo a automação de processos e a integração com sistemas externos. O **EGRESSO** utiliza **Java** para a lógica de negócios e **Ant** como ferramenta de automação de build. O sistema foi desenvolvido utilizando o **NetBeans** como ambiente de desenvolvimento integrado (IDE).

Inclui:
- Sistema de gestão de egressos
- Automação de build com **Ant**
- Estrutura modular para fácil expansão
- Testes e integração contínua

---

## 🤖 Funcionalidades do Sistema

- 🎯 **Gerenciamento de Egressos**: Cadastro, consulta e controle de egressos no sistema
- 💬 **Automação de Build**: Processo automatizado de construção e distribuição do sistema
- 🎨 **Interface Adaptável**: Sistema modular com flexibilidade para modificações e ajustes
- 🔄 **Testes Automatizados**: Execução de testes unitários para garantir a qualidade do código

---

## 📂 Estrutura do Projeto

EGRESSO/
├── build/                  # Arquivos gerados após o processo de build
├── build.xml               # Arquivo de configuração do Ant
├── dist/                   # Diretório de distribuição com arquivos compilados
├── manifest.mf             # Arquivo de manifesto
├── nbproject/              # Configurações do NetBeans
├── src/                    # Código fonte do projeto
└── test/                   # Diretório de testes

---

## 💡 Tecnologias Utilizadas

- **Java** para a lógica do sistema e implementação da integração
- **Ant** para automação de build
- **NetBeans** como IDE para desenvolvimento
- **JUnit** para execução de testes unitários
- **MySQL** para persistência de dados (caso o banco de dados esteja implementado)

---

## 🚀 Como Executar

1. Clone este repositório para sua máquina local:

   ```bash
   git clone https://github.com/SEU-USUARIO/EGRESSO.git
   cd EGRESSO
Para construir o projeto, utilize o Ant. No terminal, dentro da pasta do projeto, execute:

ant build


Isso irá gerar os arquivos necessários dentro do diretório build/.

Para executar o projeto:

ant run

🧠 Análise do Código
Como Funciona o Sistema de Egressos:

1. Cadastro de Egressos:

public class Egresso {
    private String nome;
    private String cpf;
    private String curso;
    
    public void cadastrarEgresso() {
        // Lógica para cadastro de egresso no sistema
    }
}


2. Processo de Build Automatizado:

O arquivo build.xml contém a configuração necessária para a automação do processo de build, incluindo a compilação do código, a execução de testes e a distribuição do sistema:

<project name="EGRESSO" default="build">
    <target name="build">
        <javac srcdir="src" destdir="build/classes" />
    </target>
    <target name="run" depends="build">
        <java classname="com.egresso.Main" classpath="build/classes" />
    </target>
</project>


3. Testes e Validação:

O sistema utiliza JUnit para testes unitários, garantindo que a lógica do sistema esteja funcionando corretamente:

@Test
public void testCadastroEgresso() {
    Egresso egresso = new Egresso("João", "123456789", "Engenharia");
    assertNotNull(egresso);
}

📚 Conceitos Aplicados

Características Demonstradas:

Automação de Build: Como usar o Ant para criar processos automáticos no ciclo de vida do projeto

Testes Automatizados: Garantia de qualidade por meio de testes unitários contínuos

Gerenciamento de Dados: Integração simples e eficaz com o sistema de gestão de egressos

🙋‍♂️ Autor
[Rubens Gabriel]
📫 [Rubensgabrielesilvasantos@gmail.com]
🔗 https://www.linkedin.com/in/rubens-gabriel-221679263
💻 https://github.com/rubitoxxx
