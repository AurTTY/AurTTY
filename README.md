<div align="center">

# **Backend Engineer**
### Java • Spring Boot • TypeScript • Node.js • NestJS

![Banner](https://raw.githubusercontent.com/gist/vininjr/d29bb09bd8cff42e7c1d7c2c483c6117/raw/3392f178ddfbf714217dbb3ec65ed648db3c3eb0/header.png)

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)

**Construindo APIs robustas e escaláveis com boas práticas de engenharia de software**

</div>

---

## 🎯 Sobre Mim

Engenheiro de Software com sólida formação no **SENAC** (Desenvolvimento de Sistemas) e atualmente cursando **Engenharia de Software na Estácio**. Especializado no desenvolvimento **backend** com foco em:

- **Java/Spring Boot**: APIs REST empresariais, segurança, JPA/Hibernate
- **TypeScript/Node.js**: Aplicações performáticas com NestJS e Express
- **Bancos de Dados**: PostgreSQL, MongoDB, otimização de queries

Busco oportunidades onde possa aplicar **arquitetura limpa**, **design patterns** e **código tipado** para construir sistemas robustos e de fácil manutenção.

---

## 🛠 Stack Técnica

### **Backend Principal**

| Tecnologia | Nível | Aplicações |
|------------|-------|-------------|
| **Java 17+** | Avançado | APIs REST, microsserviços, sistemas corporativos |
| **Spring Boot** | Avançado | Spring Data, Security, MVC, Cloud |
| **TypeScript** | Avançado | Tipagem estática, código escalável |
| **Node.js** | Avançado | APIs performáticas, microsserviços |
| **NestJS** | Intermediário | Arquitetura modular, GraphQL, WebSockets |

### **Banco de Dados & ORM**

```yaml
SQL:
  - PostgreSQL (principal)
  - MySQL
  - Query optimization
  - Migrations (Flyway/Liquibase)

ORM/Frameworks:
  - Spring Data JPA / Hibernate
  - Prisma ORM
  - TypeORM

NoSQL:
  - MongoDB (básico)
```

Ferramentas & DevOps

· Controle de versão: Git, GitHub Flow
· Testes: JUnit, Mockito, Jest (aprendendo)
· Containers: Docker, Docker Compose (básico)
· Cloud: AWS (EC2, RDS), Railway, Render
· Monitoramento: Logging, Actuator (Spring)

---

📁 Projetos em Destaque

API Bancária - Java/Spring Boot

Java 17 • Spring Boot 3 • Spring Security • JWT • PostgreSQL

· Implementação de transferências, saques e extratos com controle transacional
· Autenticação com JWT e roles (USER/ADMIN)
· Documentação com SpringDoc OpenAPI (Swagger)
· Validações com Bean Validation e exception handlers
· 🔗 Ver repositório

E-commerce Platform - NestJS

NestJS • TypeScript • Prisma • PostgreSQL • Redis

· Arquitetura modular (Controllers, Services, Repositories)
· Cache de produtos com Redis (TTL estratégico)
· Sistema de pedidos com relacionamentos complexos
· Rate limiting e validação com class-validator
· 🔗 Ver repositório

TaskFlow - API de Gerenciamento

Node.js • Express • TypeScript • Prisma • JWT

· Sistema completo de tarefas com hierarquia (workspace → projects → tasks)
· Middlewares de autenticação e autorização
· Filtros avançados e paginação
· Testes de integração (Jest/Supertest)
· 🔗 Ver repositório

---

💻 Código com Qualidade

```typescript
// Exemplo prático do meu estilo de código (NestJS)

@Controller('users')
@UseGuards(JwtAuthGuard)
@ApiTags('users')
export class UsersController {
  constructor(
    @Inject(USER_SERVICE) private readonly userService: IUserService,
    private readonly logger: Logger,
  ) {}

  @Get(':id')
  @ApiOperation({ summary: 'Get user by ID' })
  async findById(@Param('id', ParseIntPipe) id: number): Promise<UserResponseDto> {
    this.logger.log(`Fetching user ${id}`);
    
    const user = await this.userService.findById(id);
    if (!user) {
      throw new NotFoundException(`User ${id} not found`);
    }
    
    return plainToInstance(UserResponseDto, user, {
      excludeExtraneousValues: true,
    });
  }
}
```

```java
// Java/Spring Boot - Mesmo padrão de qualidade

@RestController
@RequestMapping("/api/users")
@RequiredArgsConstructor
public class UserController {
    
    private final UserService userService;
    private final UserMapper mapper;
    
    @GetMapping("/{id}")
    @PreAuthorize("hasRole('USER')")
    public ResponseEntity<UserResponse> findById(@PathVariable Long id) {
        return userService.findById(id)
            .map(mapper::toResponse)
            .map(ResponseEntity::ok)
            .orElseThrow(() -> new ResponseStatusException(NOT_FOUND));
    }
}
```

---

📊 GitHub Analytics

<div align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Arch-Ghostman&show_icons=true&theme=dark&include_all_commits=true&count_private=true"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Arch-Ghostman&layout=compact&langs_count=7&theme=dark&hide=html,css"/>
</div>

---

📫 Vamos conversar?

Estou aberto a oportunidades como Desenvolvedor Backend Júnior/Pleno ou estágios avançados onde possa aplicar minha stack Java/Spring e TypeScript/Node em projetos reais.

<div align="center">

https://img.shields.io/badge/Email-robertosilva.rc42@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white
https://img.shields.io/badge/LinkedIn-Roberto_Silva-0077B5?style=for-the-badge&logo=linkedin&logoColor=white
https://img.shields.io/badge/GitHub-Arch--Ghostman-100000?style=for-the-badge&logo=github&logoColor=white

</div>

---

<div align="center">

"Código é a ponte entre problemas de negócio e soluções técnicas. Faço questão de construir pontes sólidas."

⭐ Total de repositórios públicos: 20+
🔥 Commits em 2024: 300+

</div>
