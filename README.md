# Azure


## 🔷 O que é o Azure?

O Microsoft Azure é a plataforma de computação em nuvem da Microsoft. Em outras palavras, é um ambiente online onde você pode criar e gerenciar diversos tipos de serviços de TI, sem precisar ter servidores físicos em casa ou na empresa.

No Azure, você encontra soluções para praticamente tudo:
- Criar máquinas virtuais
- Armazenar arquivos e dados
- Configurar bancos de dados
- Criar redes seguras
- Usar inteligência artificial
- Rodar contêineres com Docker e Kubernetes
- Gerenciar segurança e identidade com o **Azure Active Directory (AD)**

Tudo isso é feito diretamente pela internet, de forma flexível e escalável, conforme suas necessidades crescem ou mudam.

## 🖥️ O que é uma Máquina Virtual no Azure?

Uma máquina virtual (VM) é como um computador normal — só que rodando na nuvem. Com ela, você pode instalar um sistema operacional, rodar aplicativos, hospedar sites, desenvolver sistemas e muito mais.

Você pode personalizar tudo:
- Escolher o sistema operacional (como Windows ou Linux)
- Definir a quantidade de memória RAM e núcleos de CPU
- Optar por SSD ou HD comum para armazenamento
- Configurar a rede virtual e segurança

Ela funciona 24h por dia (se você quiser), e pode ser acessada de qualquer lugar do mundo.


## 📋 O que você precisa para começar

Antes de criar sua primeira VM no Azure, você precisa ter:

1. Uma conta no **Microsoft Azure** com uma assinatura ativa (eles oferecem crédito gratuito para novos usuários!)
2. Permissões para criar recursos na conta (como administrador ou colaborador)


## 🛠️ Criando uma Máquina Virtual no Azure (passo a passo)

### 🔹 Passo 1: Acesse o portal do Azure
Vá para [https://portal.azure.com](https://portal.azure.com) e faça login com sua conta.

### 🔹 Passo 2: Comece a criar a VM
Clique em **“Máquinas virtuais”** no menu à esquerda, ou vá em **“Criar um recurso” > “Máquina virtual”**.

### 🔹 Passo 3: Configure o básico
Na primeira aba (chamada **“Básico”**), você vai preencher algumas informações:

- **Assinatura**: escolha sua conta ativa do Azure
- **Grupo de recursos**: selecione um grupo existente ou crie um novo (serve para organizar seus recursos)
- **Nome da VM**: escolha um nome que identifique bem essa máquina
- **Região**: selecione a região mais próxima (ex: *Brazil South*, para datacenters no Brasil)
- **Imagem**: escolha o sistema operacional (ex: Ubuntu 22.04, Windows Server 2022)
- **Tamanho da VM**: defina quantos núcleos e quanta memória a máquina terá (ex: B1s, D2s)
- **Autenticação**: escolha entre senha ou chave SSH para acessar
- **Portas abertas**: abra as portas necessárias (22 para Linux via SSH, 3389 para Windows via RDP)

### 🔹 Passo 4: Configure o disco
Escolha o tipo de disco onde o sistema será instalado:
- **SSD padrão** (bom desempenho)
- **HDD padrão** (mais barato)
- **SSD premium** (melhor performance)

### 🔹 Passo 5: Ajuste a rede
Aqui o Azure cria uma rede virtual automaticamente para você (caso ainda não tenha uma).

- Você pode configurar IP público (para acessar de fora)
- E ajustar o grupo de segurança de rede (NSG), que controla o tráfego de entrada e saída

### 🔹 Passo 6: Outras opções
Você também pode:
- Ativar monitoramento (para acompanhar o uso da VM)
- Rodar scripts automaticamente assim que a VM for criada
- Ativar backups (opcional, mas recomendado)

### 🔹 Passo 7: Revisar e criar
Depois de tudo preenchido, o Azure faz uma verificação.  
Se estiver tudo certo, clique em **“Criar”** e pronto! Em alguns minutos, sua VM estará no ar.

---

## 💻 Como acessar sua VM

### ✅ Se for Linux
Use SSH no terminal:

```bash
ssh usuario@IP_PUBLICO
```

(use a chave ou senha que você definiu)

### ✅ Se for Windows
Abra o programa **Área de Trabalho Remota (RDP)** no seu PC e conecte com:

- O IP da VM
- Usuário e senha que você criou

---

## ⚠️ Dica importante: Cuidado com os custos

As VMs são cobradas por tempo de uso — então se não for usá-la por um tempo, **pare** ou **exclua** a máquina para evitar cobranças desnecessárias.

