# 🐧 Linux Training Lab

Ambiente de treinamento Linux.

Este projeto foi criado para que a equipe possa praticar comandos Linux em um ambiente seguro e isolado, sem alterar a máquina local.

O objetivo é desenvolver familiaridade com terminal, arquivos, permissões, processos, logs etc.

---

# 📋 Pré-requisitos

Antes de iniciar, é necessário ter instalado:

* Docker
* Git

Para validar:

```bash
docker --version
```

```bash
docker compose version
```

---
# Instalando o docker
Instalando o docker:
```bash
Acesse o site https://docs.docker.com/desktop/setup/install/windows-install/ e escolha a maneira para instalar o docker
```
---

# 🚀 Iniciando o ambiente

Clone o repositório:

```bash
git clone <URL_DO_REPOSITORIO>
```

Entre no diretório:

```bash
cd linux-training
```

Construa e inicie o container:

```bash
docker compose up -d
```

Verifique se o container está rodando:

```bash
docker ps
```

---

# 💻 Acessando o Linux

Entre no terminal do container:

```bash
docker exec -it linux-lab bash
```

Você estará dentro de um ambiente Ubuntu:

```bash
aluno@container:~$
```

Agora você pode executar comandos Linux normalmente.

---

# Senha do Linux
```bash
linux123
```

---

# 🛑 Parando o ambiente

Sair do container:

```bash
exit
```

Parar o ambiente:

```bash
docker compose down
```

---

# 🔄 Resetar o laboratório

Caso queira recriar o ambiente do zero:

```bash
docker compose down
```

```bash
docker compose build --no-cache
```

```bash
docker compose up -d
```

## Objetivo do laboratório

Ao finalizar este treinamento, a pessoa deverá estar confortável com:

✅ Terminal Linux

Bom treinamento! 🚀
