<div align="center">

<a href="https://davi.metup.com.br">
  <img src="banner.svg" width="100%" alt="Terminal: GET /davi HTTP/2, resposta 200 OK. Davi Maximo Quoos, desenvolvedor fullstack com foco em C# e .NET" />
</a>

# Davi Maximo Quoos

**Desenvolvedor Fullstack · Backend C# / .NET**

*Eu escrevo a parte do software que ninguém vê. E é ela que não pode cair.*

<a href="https://davi.metup.com.br"><img src="https://img.shields.io/badge/Portfólio-davi.metup.com.br-9D8CFF?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfólio" /></a>
<a href="https://www.linkedin.com/in/davimaximoquoos"><img src="https://img.shields.io/badge/LinkedIn-davimaximoquoos-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:devdavimaximo@gmail.com"><img src="https://img.shields.io/badge/Email-devdavimaximo@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<a href="https://wa.me/5551995204679"><img src="https://img.shields.io/badge/WhatsApp-Conversar-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp" /></a>

</div>

---

## `> whoami`

Sou desenvolvedor fullstack com o coração no backend. Construo **APIs em ASP.NET Core** com **Clean Architecture**, regras de negócio protegidas no domínio e dados que não se perdem, e subo até o pixel com **React** e **Three.js** quando a interface precisa estar à altura.

Hoje tenho **sistemas em produção** rodando com dados reais de clientes: SaaS multi-tenant de ERP + PDV, CRM comercial, gestão de creche e financeiro multiunidade. Trabalho na [Metup](https://metup.com.br).

```csharp
public sealed class Davi : IDeveloper
{
    public string Nome => "Davi Maximo Quoos";
    public Foco Foco => Foco.Backend | Foco.Arquitetura;

    public async Task<Software> ConstruirAsync(Ideia ideia, CancellationToken ct)
    {
        var dominio = await EntenderAsync(ideia, ct);  // primeiro o problema
        var nucleo  = Modelar(dominio);                 // regras sem framework
        return await EntregarAsync(nucleo, testes: true, ct);
    }
}
```

---

## `> anatomia de uma requisição`

Meu portfólio é uma viagem 3D por dentro de uma requisição HTTP, do Kestrel até o `200 OK`. Esse é o trace dela:

<img src="trace.svg" width="100%" alt="Trace estilo OpenTelemetry com sete spans: Request, Middleware, Endpoint, Application, Domain, Infrastructure e Response, totalizando 38 ms" />

<img src="architecture.svg" width="100%" alt="Clean Architecture em anéis: Infrastructure envolve Application, que envolve Domain. Dependências apontam para dentro." />

---

## `> tail -f /cases`

<img src="cases.svg" width="100%" alt="Log de rotas dos 9 cases, 5 em produção com dados reais e 4 abertos para visitar" />

| Projeto | O que é | Stack |
|---|---|---|
| **Beemov** | SaaS de ERP + PDV multi-tenant para o mercado de bebidas. RBAC, auditoria e CI com 680+ testes | `.NET 10` `EF Core` `PostgreSQL` `React` |
| **Metup CRM** | Sistema operacional comercial: funil, atividades e API de ingestão idempotente | `ASP.NET Core` `SignalR` `Hangfire` |
| **Confraria** | ERP + PDV sob medida: caixa, estoque, PIX e cartão | `CQRS + MediatR` `PostgreSQL` `React` |
| **Sementinhas** | Gestão de creche com LGPD: permissão no servidor e auditoria de acesso sensível | `ASP.NET Core` `Identity` `React` |
| **Gestão Financeira** | Financeiro multiunidade com permissões por unidade e trilha de auditoria | `.NET 10` `Identity` `JWT` |
| [**Wedding Planner**](https://weddingplannerdn.vercel.app) | API que distribui o orçamento de casamento entre fornecedores | `ASP.NET Core` `Swagger` `React` |
| [**Xadrez Console**](https://github.com/devdavimaximo/Xadrez-Console) | Motor de xadrez do zero em C#: roque, en passant, xeque-mate | `C#` `.NET` |
| [**Caulim**](https://porcelana.metup.com.br) | Vaso em WebGL que atravessa torno, esmalte e forno conforme o scroll | `Three.js` `GLSL` `GSAP` |
| [**Fôlego**](https://apneia.metup.com.br) | Rolar a página é descer no mar: luz e pressão mapeadas à profundidade | `Three.js` `GLSL` `Lenis` |

> Os sistemas em produção não têm link público porque guardam dados reais de clientes. Mostro tudo funcionando numa call.

<div align="center">
  <a href="https://davi.metup.com.br">
    <img src="hero.png" width="100%" alt="Hero do portfólio: o nome DAVI MAXIMO QUOOS em tipografia gigante e o retrato desenhado com caracteres de código" />
  </a>
  <sub><b>↑ clique para abrir o portfólio, uma experiência WebGL em <a href="https://davi.metup.com.br">davi.metup.com.br</a></b></sub>
</div>

---

## `> dotnet list package`

**Backend**
<br />
<img src="https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white" alt="C#" />
<img src="https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt=".NET" />
<img src="https://img.shields.io/badge/ASP.NET_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="ASP.NET Core" />
<img src="https://img.shields.io/badge/EF_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="EF Core" />
<img src="https://img.shields.io/badge/xUnit-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="xUnit" />
<img src="https://img.shields.io/badge/SignalR-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="SignalR" />
<img src="https://img.shields.io/badge/Hangfire-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="Hangfire" />

**Arquitetura**
<br />
<img src="https://img.shields.io/badge/Clean_Architecture-27272A?style=flat-square" alt="Clean Architecture" />
<img src="https://img.shields.io/badge/DDD-27272A?style=flat-square" alt="DDD" />
<img src="https://img.shields.io/badge/CQRS_+_MediatR-27272A?style=flat-square" alt="CQRS + MediatR" />
<img src="https://img.shields.io/badge/Multi--tenant-27272A?style=flat-square" alt="Multi-tenant" />

**Dados & Infra**
<br />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions" />
<img src="https://img.shields.io/badge/Cloudflare_R2-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare R2" />

**Frontend**
<br />
<img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white" alt="Three.js" />
<img src="https://img.shields.io/badge/GLSL-5586A4?style=flat-square&logo=opengl&logoColor=white" alt="GLSL" />
<img src="https://img.shields.io/badge/GSAP-0AE448?style=flat-square&logo=greensock&logoColor=black" alt="GSAP" />
<img src="https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind" />

---

## `> git log --graph`

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/devdavimaximo/devdavimaximo/output/snake.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/devdavimaximo/devdavimaximo/output/snake-light.svg" />
  <img alt="Gráfico de contribuições sendo percorrido por uma cobra" src="https://raw.githubusercontent.com/devdavimaximo/devdavimaximo/output/snake.svg" width="100%" />
</picture>

---

<div align="center">

**Tem um sistema que não pode cair?**

<a href="https://davi.metup.com.br"><img src="https://img.shields.io/badge/›_GET_/contato-davi.metup.com.br-9D8CFF?style=for-the-badge" alt="Contato pelo portfólio" /></a>

<sub>HTTP/2 200 OK · connection: keep-alive</sub>

</div>
