# Sistema de Compartilhamento de Responsabilidades no Azure  

No **Microsoft Azure**, a segurança e a gestão da infraestrutura seguem o **modelo de responsabilidade compartilhada**. Isso significa que tanto a **Microsoft** quanto o **cliente** têm papéis distintos para garantir a proteção e o funcionamento adequado dos serviços.  

A divisão das responsabilidades varia de acordo com o modelo de serviço: **IaaS, PaaS ou SaaS**.  

---

## 1. IaaS (Infrastructure as a Service)  
No **IaaS**, o cliente tem maior controle, mas também mais responsabilidades.  

- **Responsabilidade da Microsoft (Azure):**  
  - Segurança física dos datacenters.  
  - Disponibilidade da rede e da infraestrutura física.  
  - Virtualização, servidores físicos e armazenamento básico.  

- **Responsabilidade do Cliente:**  
  - Sistema operacional das VMs.  
  - Configuração de rede (firewalls, NSGs, VPNs).  
  - Aplicações instaladas.  
  - Dados armazenados e gerenciados.  
  - Contas, identidades e acessos.  

---

## 2. PaaS (Platform as a Service)  
No **PaaS**, a Microsoft assume mais responsabilidades, permitindo que o cliente foque apenas no desenvolvimento e gestão das aplicações.  

- **Responsabilidade da Microsoft (Azure):**  
  - Toda a infraestrutura física e virtual.  
  - Sistema operacional e middleware (banco de dados, serviços de mensageria, runtime).  
  - Patch e atualizações automáticas da plataforma.  

- **Responsabilidade do Cliente:**  
  - Código da aplicação.  
  - Configurações específicas da aplicação.  
  - Dados inseridos e manipulados.  
  - Controle de identidades e permissões de acesso.  

---

## 3. SaaS (Software as a Service)  
No **SaaS**, quase tudo é gerenciado pela Microsoft, cabendo ao cliente apenas a utilização correta do serviço.  

- **Responsabilidade da Microsoft (Azure):**  
  - Infraestrutura física e virtual.  
  - Sistema operacional, middleware e aplicação.  
  - Atualizações de software e patches de segurança.  
  - Alta disponibilidade e escalabilidade do serviço.  

- **Responsabilidade do Cliente:**  
  - Gestão de usuários e permissões.  
  - Dados fornecidos ou manipulados.  
  - Uso adequado e seguro da aplicação.  

---

## 📌 Resumo Visual das Responsabilidades  

| Modelo | Infraestrutura | SO | Aplicações | Dados | Acessos |
|--------|----------------|----|------------|-------|---------|
| **IaaS** | Azure | Cliente | Cliente | Cliente | Cliente |
| **PaaS** | Azure | Azure | Cliente | Cliente | Cliente |
| **SaaS** | Azure | Azure | Azure | Cliente | Cliente |
