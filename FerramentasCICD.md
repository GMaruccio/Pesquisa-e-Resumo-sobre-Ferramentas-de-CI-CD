# Comparação de ferramentas de CI/CD

Atividade baseada no artigo:

> MANOLOV, Vladislav; GOTSEVA, Daniela; HINOV, Nikolay. *Practical Comparison Between the CI/CD Platforms Azure DevOps and GitHub*. Future Internet, v. 17, n. 4, 2025, p. 153.

## 1. Introdução

CI (Integração Contínua) é juntar o código de todo mundo num repositório central o tempo todo, rodando build e testes automáticos. CD (Entrega/Implantação Contínua) é automatizar o envio dessa versão para os ambientes, até a produção. O artigo compara principalmente o **Azure DevOps** e o **GitHub (Actions)**, mas cita várias outras ferramentas. Onde eu completei com coisa que **não está no artigo**, marquei com (*).

## 2. Ferramentas citadas no artigo

- **Plataformas de CI/CD:** Azure DevOps (Azure Pipelines), GitHub (GitHub Actions), Jenkins, GitLab CI/CD, Bitbucket, AWS CodePipeline, TeamCity, TravisCI, CircleCI
- **Parte do Azure DevOps:** Azure Repos, Azure Boards, Azure Test Plans, Azure Artifacts, Azure DevOps Server (on-premises)
- **Parte do GitHub:** GitHub Actions, Advanced Security, Dependabot, Marketplace, Copilot
- **Controle de versão:** Git, TFVC, Mercurial
- **Infra e nuvem:** Terraform, Kubernetes (AKS, GKE), Docker, AWS, Google Cloud
- **Segurança:** Microsoft Defender for DevOps, Azure Policy, Azure AD, HashiCorp Vault
- **Testes:** NUnit, xUnit, Selenium (Azure) e Jest, Mocha, Cypress (GitHub)
- **Outras integrações:** Jira, Confluence, ServiceNow, Power BI, Teams, Visual Studio, Prometheus

**Participação de mercado segundo o artigo:** GitHub 33%, Azure DevOps 24%, Jenkins 14%, GitLab 9%, outras 20%.

## 3. Azure DevOps vs. GitHub

| Critério | Azure DevOps | GitHub |
|---|---|---|
| Ideia geral | Suíte completa, voltada a empresas | Mais flexível, focada no desenvolvedor e no open source |
| CI/CD | Azure Pipelines: multiestágio, aprovações de release, agentes hosted e self-hosted | GitHub Actions: workflows em YAML disparados por eventos (push, PR) |
| Controle de versão | Git e TFVC | Só Git |
| Gestão e testes | Boards e Test Plans já inclusos | Não tem ferramenta de testes nativa, usa Actions e terceiros |
| Integrações | Mais forte com Microsoft/Azure | Milhares de integrações no Marketplace, agnóstico de nuvem |
| Segurança | RBAC avançado, Azure AD, Defender, Azure Policy | Advanced Security, Dependabot, secret scanning, assinatura de commits |
| Conformidade | ISO 27001, SOC 2, GDPR, HIPAA, FedRAMP | Boa, mas recursos avançados pedem plano Enterprise |
| Escalabilidade | Melhor para projetos grandes, multirregião e nuvem híbrida | Ótimo para times ágeis e distribuídos |
| Desempenho | Melhor em projetos grandes | Mais rápido em projetos pequenos e médios |
| SLA | 99,9% | 99,95% (Enterprise Cloud) |
| Preço | Por usuário e por serviço; grátis até 5 usuários; 1.800 min/mês | Planos Free, Team e Enterprise; 2.000 min/mês no Free |
| Aprendizado | Interface complexa, precisa de treino | Interface simples, fácil de aprender |

### Na prática, CI e CD

- **CI:** o GitHub Actions é mais prático para uma CI leve, porque roda testes e verificações direto no pull request. O Azure Pipelines dá mais controle em projetos grandes (paralelismo, cache, dependências entre jobs).
- **CD:** o Azure Pipelines leva vantagem, por causa das aprovações de release, do controle de ambientes e da integração com AKS, Functions e App Services. O GitHub Actions também faz CD bem, principalmente com Terraform, Kubernetes e GitOps, mas com menos governança.

## 4. Outras ferramentas

O artigo fala pouco delas, então a análise é bem mais curta.

| Ferramenta | Vantagens | Limitações | Quando usar |
|---|---|---|---|
| **Jenkins** | Open source, muitos plugins, integra com quase tudo | Dá bastante trabalho de manutenção e exige conhecimento técnico | Quando a equipe quer controle total e sabe manter a infra |
| **GitLab CI/CD** | Tudo em uma plataforma (código, projeto e CI/CD) | Quase não é detalhado no artigo | Quando quer uma solução all-in-one |
| **Bitbucket** | Integra bem com Jira e Confluence | O artigo cita Mercurial, mas isso já foi descontinuado (*) | Quem já usa o ecossistema Atlassian |
| **TeamCity** | Configurações de build poderosas, interface amigável | Pouco detalhado | Builds complexos em empresas |
| **AWS CodePipeline** | Só é citado; integra com a AWS (*) | Menos flexível fora da AWS (*) | Infra toda na AWS (*) |
| **TravisCI / CircleCI** | Só citados como parte pequena do mercado; CI hospedada e simples (*) | — | Projetos pequenos (*) |

## 5. Qual escolher?

- **Azure DevOps:** empresas grandes, setores regulados (finanças, saúde, governo), uso de Azure e Microsoft, nuvem híbrida ou on-premises.
- **GitHub:** open source, startups, times pequenos e médios, GitOps e cloud-native.
- **Jenkins:** quando precisa de muita customização e tem equipe para manter.
- **GitLab:** quando quer tudo numa plataforma só.
- **Bitbucket / TeamCity:** quem já usa ferramentas da Atlassian ou da JetBrains.
- **Usar os dois:** os autores dizem que também dá para combinar Azure DevOps e GitHub.


## 6. Conclusão

Não existe uma ferramenta melhor para tudo. O Azure DevOps funciona melhor em ambientes grandes, com regras rígidas e muito uso de Microsoft. O GitHub se encaixa melhor em times ágeis, open source e projetos mais leves. A escolha depende do tamanho do time, do orçamento, da segurança exigida e da infraestrutura que já existe.
