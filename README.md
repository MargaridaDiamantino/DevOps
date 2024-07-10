# DevOps

Material complementar utilizado no evento NLW Journey, para a tecnologia DevOps

##
# Instalando Go

A forma mais recomendada de obter o executável `go` utilizado para criar, executar e gerenciar projetos na linguagem é através do instalador oficial da linguagem ou do binário pré-compilado para seu sistema operacional

Caso Você ja tenha a ferramenta `go` disponível no seu terminal, confira se a versão é >=1.21.
Isso pode ser feito rodando o comando `go version`.
Baixe o binário mais recente para seu sistema operacional e arquitetura no site: https://go.dev/dl/

# Instalando Docker e Docker Compose

**Instalação do Docker e Docker Compose**

# Instalação

A forma mais fácil e recomendada de obter o Docker é instalar o Docker Desktop. O Docker Desktop inclui o Docker Compose juntamente com o Docker Engine e Docker CLI, que são pré-requisitos do Compose.
O Docker Desktop está disponível em:

- [Linux](https://docs.docker.com/desktop/install/linux-install/)
- [Mac](https://docs.docker.com/desktop/install/mac-install/)
- [Windows](https://docs.docker.com/desktop/install/windows-install/)

Se você já instalou o Docker Desktop, pode verificar qual versão do Compose possui selecionando "Sobre o Docker Desktop" no menu do Docker, o menu do ícone da baleia.

Se você já tiver o Docker Engine e o Docker CLI instalados, pode instalar o plugin Compose a partir da linha de comando, de duas maneiras:

- [Usando o repositório do Docker](https://docs.docker.com/compose/install/linux/#install-using-the-repository)
- [Fazendo o download e instalação manualmente](https://docs.docker.com/compose/install/linux/#install-the-plugin-manually)


# Instalando K3D

**Instalação do K3D**

# Instalação

O **K3D** está disponível em:

### Linux

1. Instale com o comando:
    
    ```bash
    wget -q -O - https://raw.githubusercontent.com/k3d-io/k3d/main/install.sh | bash
    ```
    
2. Teste se o K3D foi instalado corretamente:
    
    ```bash
    k3d --version
    ```
    

### Mac

1. Instale o Homebrew:
    
    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```
    
2. Instale o `k3d` usando o Homebrew.
    
    ```bash
    brew install k3d
    ```
    
3. Verifique a instalação.
    
    ```bash
    k3d --version
    ```
    

### Windows

<aside>
⚠️ Nesse passo precisa ter o Chocolatey instalado

</aside>

1. Certifique-se de estar usando o powershell como administrador
    
    ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/08f749ff-d06d-49a8-a488-9846e081b224/10eef077-331f-4bc8-8a8f-d63f783a9795/Untitled.png)
    
2. Rode o comando para instalar o Chocolatey.
    
    ```powershell
    Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
    ```
    
3. Rode o comando para instalar o k3d.
    
    ```powershell
    choco install k3d
    ```
    

Instalar utilizando a documentação oficial:

https://k3d.io/

# Instalando Kubectl

*Instalação do kubectl*

# Instalação

O **Kubectl** está disponível em:

### Linux

1. Faça download da versão mais recente com o comando:
    
    ```bash
    curl -LO "https://dl.k8s.io/release/**$(**curl -L -s https://dl.k8s.io/release/stable.txt**)**/bin/linux/amd64/kubectl"
    ```
    
2. Instale o kubectl
    
    ```bash
    sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
    ```
    
3. Teste para garantir que o kubectl foi instalado:
    
    ```bash
    kubectl version --client
    ```
    

### Mac

1. Instale o Homebrew:
    
    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```
    
2. Instale o `kubectl` usando o Homebrew.
    
    ```bash
    brew install kubectl
    ```
    
3. Verifique a instalação.
    
    ```bash
    kubectl version --client
    ```
    

### Windows

1. Baixe e instale a versão mais recente do kubectl com o comando:
    
    ```powershell
    winget install -e --id Kubernetes.kubectl
    ```
    
2. Verifique a instalação.
    
    ```powershell
    kubectl version --client
    ```
    

Instalar utilizando a documentação oficial:

https://kubernetes.io/pt-br/docs/tasks/tools/

# Instalando Helm

*Instalação do Helm*

# Instalação

O **Helm** está disponível em:

### Linux

1. Instale o Helm com o comando:
    
    ```bash
    curl https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3 | bash
    ```
    
2. Teste com o comando:
    
    ```bash
    helm version
    ```
    

### Mac

1. Instale o Homebrew:
    
    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```
    
2. Instale o `helm` usando o Homebrew.
    
    ```bash
    brew install helm
    ```
    
3. Teste com o comando:
    
    ```bash
    helm version
    ```
    

### Windows

<aside>
⚠️ Nesse passo precisa ter o Chocolatey instalado

</aside>

1. Certifique-se de estar usando o powershell como administrador
    
    ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/08f749ff-d06d-49a8-a488-9846e081b224/10eef077-331f-4bc8-8a8f-d63f783a9795/Untitled.png)
    
2. Rode o comando para instalar o Chocolatey.
    
    ```powershell
    Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
    ```
    
3. Rode o comando para instalar o k3d.
    
    ```powershell
    choco install kubernetes-helm
    ```
    

Instalar utilizando a documentação oficial:

https://helm.sh/pt/docs/intro/install/

# Instalando AWS CLI

*Instalação do AWS CLI*

# Instalação

O AWS CLI está disponível em:

### Linux

**1** - **Para instalar** a AWS CLI, execute os comandos a seguir.

```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

- **Para atualizar a instalação atual** da AWS CLI, adicione as informações do symlink e instalador existentes para criar o comando `install` com os parâmetros `--bin-dir`, `--install-dir` e `--update`. O bloco de comando a seguir usa um exemplo de symlink de `*/usr/local/bin*` e um exemplo de localização do instalador de `*/usr/local/aws-cli*`.

```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install --bin-dir /usr/local/bin --install-dir /usr/local/aws-cli --update
```

### Mac

1 - Baixe o arquivo usando o comando `curl`. A opção `-o` especifica o nome do arquivo no qual o pacote obtido por download foi gravado. O arquivo é gravado como `AWSCLIV2.pkg` na pasta atual.

```bash
curl "https://awscli.amazonaws.com/AWSCLIV2.pkg" -o "AWSCLIV2.pkg"
```

2 - Execute o programa `installer` padrão do macOS, especificando o arquivo `.pkg` baixado como a origem. Use o parâmetro `-pkg` para especificar o nome do pacote a ser instalado e o parâmetro `-target /` para especificar em qual unidade instalar o pacote. Os arquivos são instalados no `/usr/local/aws-cli`, e um symlink é criado automaticamente em `/usr/local/bin`. Você deve incluir `sudo` no comando para conceder permissões de gravação para essas pastas.

```bash
sudo installer -pkg ./AWSCLIV2.pkg -target /
```

Após a conclusão da instalação, os logs de depuração são gravados em `/var/log/install.log`.

3 - Para verificar se o shell pode encontrar e executar o comando `aws` no `$PATH`, use os comandos a seguir.

```bash
**which aws**
*/usr/local/bin/aws* 
**aws --version**
*aws-cli/2.10.0 Python/3.11.2 Darwin/18.7.0 botocore/2.4.5*
```

Se não for possível encontrar o comando `aws`, talvez seja necessário reiniciar o terminal ou seguir a solução de problemas em [Solucionar erros da AWS CLI](https://docs.aws.amazon.com/pt_br/cli/latest/userguide/cli-chap-troubleshooting.html).

### Windows

- Baixar e executar o instalador MSI da AWS CLI para Windows (64 bits)
    
    > https://awscli.amazonaws.com/AWSCLIV2.msi
    > 
    
- Você também pode executar o comando `msiexec` para executar o instalador MSI.

```powershell
msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi
```

- Para confirmar a instalação, abra o menu **Início**, procure `cmd` para abrir uma janela do prompt de comando e, no prompt de comando, use o comando `aws --version`.

```powershell
**aws --version**
*aws-cli/2.10.0 Python/3.11.2 Windows/10 exe/AMD64 prompt/off*
```

Instalar utilizando a documentação oficial:

# Instalando Lens

**Instalação do Lens**

# Instalação

O **Lens** está disponível em:

### Linux

1. Obtenha a chave de segurança pública do Lens:
    
    ```bash
    curl -fsSL https://downloads.k8slens.dev/keys/gpg | gpg --dearmor | sudo tee /usr/share/keyrings/lens-archive-keyring.gpg > /dev/null
    ```
    
2. Especifique o canal `stable`
    
    ```bash
    echo "deb [arch=amd64 signed-by=/usr/share/keyrings/lens-archive-keyring.gpg] https://downloads.k8slens.dev/apt/debian stable main" | sudo tee /etc/apt/sources.list.d/lens.list > /dev/null
    ```
    
3. Instale o Lens Desktop:
    
    ```bash
    sudo apt update
    sudo apt install lens
    ```
    

### Mac

1. Instale o Homebrew:
    
    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```
    
2. Instale o `k3d` usando o Homebrew.
    
    ```bash
    brew install --cask lens
    ```
    

### Windows

1. Instale o Lens com o comando:
    
    ```powershell
    wget "https://api.k8slens.dev/binaries/Lens%20Setup%202024.3.191333-latest.exe" -O Lens_Setup.exe
    ```
    

Instalar utilizando a documentação oficial:

https://docs.k8slens.dev/getting-started/install-lens/
