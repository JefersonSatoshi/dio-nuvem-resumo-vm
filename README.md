
# Desafio de Projeto DIO - Criando uma Máquina Virtual no Azure

Este repositório contém um resumo básico do processo de criação de uma máquina virtual (VM) no Microsoft Azure.

## 📌 Objetivo

Aplicar os conhecimentos aprendidos sobre o Microsoft Azure na criação de uma máquina virtual e documentar esse processo para fins de estudo.

## 💻 O que é uma Máquina Virtual (VM)?

Uma Máquina Virtual (VM) é um ambiente virtual que simula um computador físico. Ela permite executar sistemas operacionais e aplicativos de forma isolada, utilizando os recursos da infraestrutura em nuvem, como o Microsoft Azure. É amplamente usada para testes, desenvolvimento, hospedagem de aplicações e muito mais.


## 🧱 Etapas Realizadas

1. Acesse o [portal do Azure](https://portal.azure.com/)
   - Login com conta Microsoft.

2. **Detalhes do Projeto**
   - **Assinatura**: Azure Subscription 1.
   - **Grupo de Recursos**: Criação de um novo grupo de recursos chamado `vm-dio-lab_group`.

3. **Detalhes da Instância**
   - **Nome da Máquina Virtual**: `vm-dio-lab`.
   - **Região**: `Brazil South`.
   - **Opções de Disponibilidade**: Nenhuma redundância de infraestrutura necessária.
   - **Zona de Disponibilidade**: Seleção de Zona 1 para a VM. (O Azure atribui automaticamente a zona de acordo com a disponibilidade da região).
   - **Imagem**: `Windows Server 2016 Datacenter - x64 Gen2`.
   - **Arquitetura da VM**: `x64`.
   - **Tamanho**: `Standard B1s` (1 vCPU, 1 GiB de memória).
   - **Habilitar Hibernação**: Não compatível com a imagem e o tamanho selecionados.

4. **Conta de Administrador**
   - **Nome de Usuário**: `nome do adm`.
   - **Senha**: A senha foi configurada de acordo com os requisitos do Azure.

5. **Regras de Portas de Entrada**
   - **Portas de Entrada Públicas**:
     - Seleção de `RDP (3389)` para permitir o acesso remoto à VM.
     - A configuração está aberta para todos os IPs, sendo recomendada apenas para testes. O tráfego pode ser mais restrito configurando regras avançadas na guia "Rede".

6. **Criação Final**
   - **Revisar + Criar**
   - Confirmação da criação da VM com as configurações padrão.

## 💡 Observações e Dicas

- Utilizei a assinatura gratuita (`Azure Subscription 1`)
- A VM está configurada para testes, com acesso remoto via RDP
- É importante **encerrar ou excluir a VM após o uso** para evitar consumo de créditos ou cobranças.
- Ficar atento com o consumo dos créditos.
- Recomendado usar um cartão virtual com validade limitada para evitar cobranças indevidas.

## 🚀 Conclusão

Com esse laboratório, foi possível aplicar na prática os conhecimentos de criação e configuração de máquinas virtuais na nuvem.

## 📚 Referências

- [Documentação oficial Microsoft Azure](https://learn.microsoft.com/pt-br/azure/virtual-machines/)
- Aulas da DIO sobre Azure
