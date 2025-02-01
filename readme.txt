# README.md

## Descrição do Projeto
Este projeto utiliza o Vagrant para gerenciar e configurar máquinas virtuais de maneira simples e eficiente. Ele facilita o desenvolvimento local ao criar um ambiente consistente e controlado, garantindo que todos os integrantes da equipe de desenvolvimento utilizem as mesmas configurações de ambiente.

## Instruções para Iniciar a Máquina Virtual
Para iniciar a máquina virtual, siga os passos abaixo:

1. Certifique-se de que o Vagrant e o VirtualBox estão instalados em sua máquina.
2. Navegue até o diretório onde o arquivo `Vagrantfile` está localizado.
3. Execute o seguinte comando no terminal:

   ```bash
   vagrant up
   ```

   Este comando irá iniciar a máquina virtual definida no arquivo `Vagrantfile`. Caso a máquina ainda não tenha sido provisionada, ela será configurada automaticamente durante o processo.

## Como Acessar a Máquina Virtual via SSH
Após iniciar a máquina virtual, você pode acessá-la via SSH com o seguinte comando:

```bash
vagrant ssh
```

Este comando conecta você à máquina virtual diretamente, permitindo que você execute comandos no ambiente provisionado.

## Explicação sobre a Pasta Sincronizada
O Vagrant configura uma pasta sincronizada entre sua máquina anfitriã e a máquina virtual. Isso permite que você edite arquivos localmente e veja as alterações refletidas na máquina virtual sem a necessidade de transferências manuais de arquivos.

### Utilizando a Pasta Sincronizada

1. Por padrão, o diretório onde o arquivo `Vagrantfile` está localizado é sincronizado com o diretório `/vagrant` na máquina virtual.
2. Você pode acessar essa pasta dentro da máquina virtual navegando para o caminho `/vagrant`:

   ```bash
   cd /vagrant
   ```

3. Qualquer arquivo ou pasta que você adicionar no diretório local será automaticamente acessível dentro da máquina virtual no diretório sincronizado.

Essa funcionalidade facilita a colaboração e o desenvolvimento, pois você pode usar suas ferramentas locais para editar o código e testar diretamente na máquina virtual.
