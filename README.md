# Curso Interativo de IoT: Da Teoria à Prática

![Licença](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-ativo-brightgreen)
![GitHub issues](https://img.shields.io/github/issues/caiosmascarenhas/curso-iot)
![GitHub forks](https://img.shields.io/github/forks/caiosmascarenhas/curso-iot?style=social)
![GitHub stars](https://img.shields.io/github/stars/caiosmascarenhas/curso-iot?style=social)

Material de aula interativo em formato de página web única (SPA) para o curso de **Internet das Coisas** da **Fatec Sorocaba**, ministrado pelo **Prof. Caio S. Mascarenhas**. O projeto aborda desde os conceitos fundamentais de IoT até a implementação de um sistema prático de monitoramento de compressores, utilizando hardware acessível e software de código aberto.

### [➡️ Acesse a Demonstração Ao Vivo Aqui](https://caiosmascarenhas.github.io/curso-iot/)

*(Nota: Este é um link de exemplo. Substitua `<SEU-USUARIO-GITHUB>` pelo seu nome de usuário após publicar no GitHub Pages.)*

---

### 📸 Screenshot da Aplicação

![Imagem do Curso de IoT](https://placehold.co/800x450/d1fae5/047857?text=Screenshot+da+Página+do+Curso)

---

## 🎯 Sobre o Projeto

Este repositório contém o material de apoio para um curso introdutório de IoT, projetado para alunos de diversas áreas. O objetivo é fornecer uma base sólida sobre o que é a Internet das Coisas, suas aplicações e capacitar os alunos a desenvolverem um protótipo funcional do início ao fim.

O projeto prático consiste em um sistema de monitoramento de vibração e temperatura para um compressor de ar, cobrindo todo o ciclo de vida dos dados:

1.  **Coleta:** Um sensor **MPU6050** captura dados de movimento e temperatura.
2.  **Processamento na Ponta (Edge):** Um microcontrolador **ESP32** lê o sensor, calibra os dados e os publica em uma rede local.
3.  **Comunicação:** O protocolo **MQTT** é usado para transportar os dados de forma leve e eficiente.
4.  **Backend e Armazenamento:** Um **Raspberry Pi** atua como servidor, rodando um broker MQTT (**Mosquitto**) para receber os dados, que são então processados pelo **Node-RED** e armazenados em um banco de dados de série temporal (**InfluxDB**).
5.  **Visualização:** Os dados são apresentados em tempo real em dashboards interativos criados com **Grafana**.

---

## 🚀 Funcionalidades

* **Conteúdo Estruturado:** Módulos separados para Fundamentos, Casos de Uso, Projeto Prático, Documentação e Impressão 3D.
* **Navegação Fixa:** Sidebar lateral para fácil acesso a todas as seções do curso.
* **Conteúdo Expansível:** Seções do projeto prático são colapsáveis para uma leitura focada.
* **Diagramas Visuais:** Arquitetura e fluxos de dados explicados com diagramas em HTML/CSS.
* **Blocos de Código:** Exemplos de código para o ESP32 e Docker Compose com funcionalidade de "Copiar para a Área de Transferência".
* **Responsividade:** Layout adaptável para visualização em desktops, tablets e dispositivos móveis.
* **Documentação Integrada:** Seção dedicada com explicações detalhadas sobre as tecnologias utilizadas e links para recursos oficiais.

---

## 🛠️ Tecnologias Utilizadas

Este projeto foi construído utilizando as seguintes tecnologias:

* **Frontend:** HTML5, Tailwind CSS, JavaScript.
* **Visualização de Dados:** Chart.js.
* **Backend (Projeto Prático):**
    * **Hardware:** ESP32, Raspberry Pi (3B+, 4 ou 5), Sensor MPU6050.
    * **Software e Plataformas:** Raspberry Pi OS, Docker, Docker Compose, Mosquitto (Broker MQTT), Node-RED, InfluxDB, Grafana.

---

## ⚙️ Configuração Local com Git

Para executar este projeto localmente utilizando Git, siga os passos abaixo. É necessário ter o [Git](https://git-scm.com/) instalado em sua máquina.

1.  **Clone o repositório:**
    Abra seu terminal ou Git Bash e execute o comando abaixo, substituindo `<SEU-USUARIO-GITHUB>` pelo seu nome de usuário.

    ```bash
    git clone [https://github.com/](https://github.com/)<SEU-USUARIO-GITHUB>/curso-iot.git
    ```

2.  **Navegue até a pasta do projeto:**

    ```bash
    cd curso-iot
    ```

3.  **Abra o arquivo principal:**
    Agora que você está na pasta do projeto, basta abrir o arquivo `index.html` no seu navegador de preferência.

---

## 🤝 Como Contribuir

Contribuições são sempre bem-vindas! Se você encontrar algum erro, tiver sugestões de melhoria ou quiser adicionar novo conteúdo, sinta-se à vontade para:

1.  **Abrir uma Issue:** Descreva o problema ou a sua sugestão na aba "Issues" do repositório.
2.  **Enviar um Pull Request:**
    * Faça um **Fork** deste repositório.
    * Crie uma nova **Branch** para sua modificação (`git checkout -b minha-feature`).
    * Faça o **Commit** de suas alterações (`git commit -m 'Adicionando minha incrível feature'`).
    * Envie para a sua Branch (`git push origin minha-feature`).
    * Abra um **Pull Request**.

---

## 📜 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 🎓 Agradecimentos

* Agradecimento especial à **Fatec Sorocaba** por proporcionar o ambiente para a disseminação do conhecimento.
* A todos os alunos dedicados deste curso.

