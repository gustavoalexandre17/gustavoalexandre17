<h1 align="center">Olá, eu sou Gustavo Alexandre! 👋</h1>
<h3 align="center">Ciência da Computação | Cibersegurança</h3>

<p align="center">
  <a href="mailto:alexandrega333@gmail.com" target="_blank">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>
  <a href="https://www.linkedin.com/in/gustavo-alexandre-4485b1353/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="https://leetcode.com/u/alexanderthebig0/" target="_blank">
    <img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="Leetcode">
  </a>
  <a href="https://judge.beecrowd.com/en/profile/1117817" target="_blank">
    <img src="https://img.shields.io/badge/Beecrowd-F9A825?style=for-the-badge&logo=beecrowd&logoColor=black" alt="Beecrowd">
  </a>
</p>

---

## Sobre Mim

<p>
  Sou estudante de <strong>Ciência da Computação</strong>, interessado em entender como as tecnologias funcionam por baixo dos panos. Atualmente, meu foco principal é me especializar em <strong>Cibersegurança</strong> e infraestrutura.
</p>

<p>
  Possuo interesse em <strong>sistemas de baixo nível</strong>, arquitetura de <strong>sistemas Linux</strong>, <strong>redes de computadores</strong> e <strong>computação distribuída</strong>. Tenho uma base sólida em <strong>C</strong>, <strong>C++<strong> e <strong>Python</strong>, linguagens que utilizo na programação competitiva e que agora são fundamentais para explorar o funcionamento interno dos sistemas operacionais e criar scripts de automação.
</p>

<p>
  Meu objetivo atual é aprofundar meus estudos em protocolos de rede, segurança da informação, manipulação de memória e administração de sistemas UNIX-like.
</p>

---

## Experiência Prática & Projetos em Destaque

### Edge AI: Desenvolvimento de Kernel Driver para NPU (RISC-V)
Atualmente, sou responsável pelo desenvolvimento de um **Kernel Driver** para comunicação com um acelerador de hardware (NPU *multiplierless*) focado em inferência de **Edge AI**, rodando em arquitetura **RISC-V**. 

O projeto engloba todo o ciclo de vida do driver no espaço de kernel (Kernel Space), desde a emulação até o deploy físico em FPGA, com as seguintes responsabilidades:
* **Desenvolvimento de LKM (Loadable Kernel Module):** Criação, compilação via *cross-compiler toolchain* e validação de módulos do kernel Linux, inicialmente utilizando QEMU para emulação RISC-V.
* **Dispositivo de Caractere & File Operations:** Exposição da NPU para o *User Space* através de um nó de dispositivo (`/dev/npu_ternaria`), mapeando chamadas de sistema (syscalls) para rotinas internas via `struct file_operations` (`read`, `write`, `ioctl`).
* **Memory-Mapped I/O (MMIO):** Conversão de endereços físicos para virtuais utilizando a API do kernel (`ioremap`) com base nas especificações do *Device Tree Source (DTS)*, permitindo a comunicação direta com os registradores de hardware.
* **Sincronização e Transferência Segura:** Uso de `copy_from_user` e `copy_to_user` para tráfego seguro de matrizes de pesos/dados, controle de fluxo no hardware manipulando registradores de status/controle, e implementação de *Polling/IRQ* para gerenciar a execução da NPU.
* **Otimização de Contexto:** Redução do overhead de *context-switching* no tráfego Aplicação ↔ Driver ↔ Hardware para garantir precisão máxima no benchmarking de performance durante o deploy no SoC físico (FPGA).

---

### Engenharia de Software & Automação: Bot Cardápio UFCA
Desenvolvimento de um bot no Telegram em **Python** para automação de consultas e notificações.
* **Test-Driven Development (TDD):** Desenvolvimento guiado por testes com 80-90% de cobertura utilizando `pytest`, garantindo resiliência e facilitando refatorações seguras.
* **Extração de Dados e Automação:** Implementação de rotinas de *parsing* automático de PDFs para extração de dados não estruturados e sistema de agendamento (*scheduling*) de notificações.
* **Arquitetura Modular:** Separação clara de responsabilidades no design do software (Handlers, Scraper, Cache management), com documentação arquitetural e integração com CI/CD e testes unitários.

---

## Tecnologias e Ferramentas

### Base Técnica
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05033?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

### Em Estudo
![Kali Linux](https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kali-linux&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Computer Networks](https://img.shields.io/badge/Redes_de_Computadores-02569B?style=for-the-badge)

### Conhecimentos Prévios
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-02569B?style=for-the-badge)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

---
