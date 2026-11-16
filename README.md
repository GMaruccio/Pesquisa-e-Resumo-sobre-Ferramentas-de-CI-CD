# Pesquisa: Comparação de ferramentas de CI/CD

Este repositório reúne uma pesquisa acadêmica sobre ferramentas
utilizadas em processos de **Integração Contínua (CI)** e
**Entrega/Implantação Contínua (CD)**, desenvolvida com base no artigo
*Practical Comparison Between the CI/CD Platforms Azure DevOps and
GitHub*.

## Sobre a pesquisa

O objetivo do trabalho é identificar e analisar ferramentas relacionadas
a CI/CD, comparando suas características, funcionalidades, vantagens,
limitações e cenários de utilização.

A pesquisa tem como foco principal a comparação entre **Azure DevOps** e
**GitHub Actions**, além de apresentar uma análise mais breve de outras
plataformas e tecnologias citadas pelos autores.

## Referência principal

MANOLOV, Vladislav; GOTSEVA, Daniela; HINOV, Nikolay. **Practical
Comparison Between the CI/CD Platforms Azure DevOps and GitHub**.
*Future Internet*, v. 17, n. 4, 2025, artigo 153.

-   [Acessar o artigo original](https://www.mdpi.com/1999-5903/17/4/153)

## Conteúdo do repositório

O arquivo [`FerramentasCICD.md`](FerramentasCICD.md) contém o material
completo da pesquisa, organizado nos seguintes tópicos:

1.  **Introdução a CI e CD** --- apresenta os conceitos de Integração
    Contínua e Entrega/Implantação Contínua.
2.  **Ferramentas citadas no artigo** --- reúne as plataformas,
    serviços, tecnologias e ferramentas mencionadas pelos autores.
3.  **Azure DevOps vs. GitHub** --- compara as duas plataformas
    considerando CI/CD, controle de versão, gestão de projetos, testes,
    integrações, segurança, conformidade, escalabilidade, desempenho,
    custos e facilidade de aprendizado.
4.  **Outras ferramentas** --- apresenta observações sobre Jenkins,
    GitLab CI/CD, Bitbucket, TeamCity, AWS CodePipeline, Travis CI e
    CircleCI.
5.  **Critérios de escolha** --- resume os contextos em que cada solução
    pode ser mais adequada.
6.  **Conclusão** --- reúne os principais pontos identificados na
    comparação.

## Principais ferramentas e tecnologias abordadas

A pesquisa menciona, entre outras, as seguintes ferramentas e
tecnologias:

  -----------------------------------------------------------------------
  Categoria                           Ferramentas e tecnologias
  ----------------------------------- -----------------------------------
  Plataformas de CI/CD                Azure DevOps, Azure Pipelines,
                                      GitHub Actions, Jenkins, GitLab
                                      CI/CD, Bitbucket, AWS CodePipeline,
                                      TeamCity, Travis CI e CircleCI

  Gestão e colaboração                Azure Boards, Azure Test Plans,
                                      Azure Repos, Azure Artifacts, Jira,
                                      Confluence, ServiceNow, Power BI e
                                      Microsoft Teams

  Controle de versão                  Git, TFVC e Mercurial

  Infraestrutura e nuvem              Terraform, Kubernetes, AKS, GKE,
                                      Docker, AWS e Google Cloud

  Segurança                           Microsoft Defender for DevOps,
                                      Azure Policy, Azure AD, HashiCorp
                                      Vault, GitHub Advanced Security e
                                      Dependabot

  Testes                              NUnit, xUnit, Selenium, Jest, Mocha
                                      e Cypress
  -----------------------------------------------------------------------

A análise detalhada e as observações sobre cada ferramenta estão no
arquivo da pesquisa.

## Síntese da comparação

De acordo com a análise apresentada no material:

-   **Azure DevOps** é apresentado como uma solução abrangente,
    especialmente adequada a organizações que precisam de governança,
    controle de ambientes, recursos integrados de gestão e testes, ou
    que já utilizam tecnologias Microsoft e Azure.
-   **GitHub Actions** se destaca pela integração com o GitHub, pela
    execução de workflows acionados por eventos do repositório e pela
    flexibilidade de integração com diferentes ferramentas e provedores
    de nuvem.
-   **Jenkins** é uma alternativa que oferece ampla personalização e
    ecossistema de plugins, mas exige maior responsabilidade de
    configuração e manutenção.
-   **GitLab CI/CD** reúne recursos de desenvolvimento e automação em
    uma mesma plataforma.
-   **Bitbucket, TeamCity, AWS CodePipeline, Travis CI e CircleCI**
    também são considerados, com comentários mais breves no material, de
    acordo com o nível de detalhamento disponível na pesquisa.

A conclusão geral é que **não existe uma ferramenta ideal para todos os
cenários**. A escolha depende de fatores como infraestrutura existente,
porte da equipe, orçamento, requisitos de segurança e conformidade,
necessidade de personalização e nível de governança desejado.

## Observação sobre o escopo

O arquivo da pesquisa diferencia informações apresentadas no artigo de
complementações feitas durante a elaboração do trabalho. Essas
complementações estão identificadas com `(*)` no próprio documento. As
observações sobre ferramentas que recebem pouco detalhamento no artigo
devem ser entendidas como análises complementares, e não como conclusões
atribuídas diretamente aos autores.

## Arquivo principal

-   [`FerramentasCICD.md`](FerramentasCICD.md) --- pesquisa completa.

------------------------------------------------------------------------

Pesquisa elaborada para fins acadêmicos, com base no artigo referenciado
acima.
