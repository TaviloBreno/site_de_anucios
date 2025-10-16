# 📢 Sistema de Anúncios

[![PHP Version](https://img.shields.io/badge/PHP-%3E%3D5.6-blue.svg)](https://www.php.net/)
[![CodeIgniter](https://img.shields.io/badge/CodeIgniter-3.x-orange.svg)](https://codeigniter.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Sistema web completo para gerenciamento e publicação de anúncios, desenvolvido com CodeIgniter 3 e painel administrativo moderno.

## 🚀 Sobre o Projeto

Sistema robusto de anúncios com área administrativa completa, desenvolvido seguindo as melhores práticas de desenvolvimento PHP e padrão MVC. Ideal para classificados online, marketplace ou plataformas de anúncios.

### ✨ Principais Funcionalidades

- 📊 **Painel Administrativo Moderno** - Interface responsiva com template Otika
- 🔐 **Área Restrita** - Sistema de autenticação e controle de acesso
- 📱 **Design Responsivo** - Compatível com todos os dispositivos
- ⚡ **Performance Otimizada** - Estrutura MVC para código limpo e manutenível
- 🎨 **UI/UX Profissional** - Interface intuitiva e moderna

## 🛠️ Tecnologias Utilizadas

### Backend
- **PHP** 5.6+ / 7.x / 8.x
- **CodeIgniter 3.x** - Framework MVC
- **Composer** - Gerenciador de dependências

### Frontend
- **HTML5** & **CSS3**
- **JavaScript** (ES6+)
- **Bootstrap** - Framework CSS
- **Feather Icons** - Biblioteca de ícones
- **jQuery** - Manipulação DOM

### Template Admin
- **Otika** - Dashboard Template Premium
- Componentes responsivos e modernos
- Múltiplos layouts e temas

## 📋 Pré-requisitos

- PHP >= 5.6 (recomendado 7.4+)
- MySQL 5.7+ / MariaDB 10.2+
- Apache/Nginx com mod_rewrite habilitado
- Composer
- XAMPP/WAMP/LAMP (para ambiente local)

## 🔧 Instalação

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/anuncios.git
cd anuncios
```

### 2. Instale as dependências

```bash
composer install
```

### 3. Configure o banco de dados

Edite o arquivo `application/config/database.php`:

```php
$db['default'] = array(
    'hostname' => 'localhost',
    'username' => 'seu_usuario',
    'password' => 'sua_senha',
    'database' => 'anuncios_db',
    'dbdriver' => 'mysqli',
);
```

### 4. Configure a URL base

Edite o arquivo `application/config/config.php`:

```php
$config['base_url'] = 'http://localhost:8080/';
```

### 5. Importe o banco de dados

```bash
mysql -u seu_usuario -p anuncios_db < database/schema.sql
```

### 6. Configure permissões (Linux/Mac)

```bash
chmod -R 755 application/cache
chmod -R 755 application/logs
```

## 🎯 Como Usar

### Ambiente Local (XAMPP)

1. Copie o projeto para `C:\xampp\htdocs\anuncios`
2. Inicie Apache e MySQL no painel do XAMPP
3. Acesse: `http://localhost:8080/`

### Área Administrativa

- URL: `http://localhost:8080/restrita/home`
- Credenciais padrão (alterar após primeiro acesso):
  - Usuário: `admin`
  - Senha: `admin123`

## 📁 Estrutura do Projeto

```
anuncios/
├── application/           # Código da aplicação
│   ├── controllers/       # Controladores MVC
│   │   └── restrita/      # Controllers da área admin
│   ├── models/           # Modelos de dados
│   ├── views/            # Views (templates)
│   │   └── restrita/     # Views da área admin
│   ├── config/           # Arquivos de configuração
│   └── libraries/        # Bibliotecas customizadas
├── public/               # Arquivos públicos
│   └── restrita/         # Assets do painel admin
│       └── assets/       # CSS, JS, imagens
├── system/               # Core do CodeIgniter
├── vendor/               # Dependências do Composer
├── .htaccess            # Configuração Apache
├── composer.json        # Dependências PHP
└── index.php           # Ponto de entrada

```

## 🎨 Screenshots

### Painel Administrativo
Dashboard moderno e intuitivo com métricas em tempo real, gráficos interativos e navegação simplificada.

### Área de Anúncios
Interface responsiva para listagem, criação e gerenciamento de anúncios.

## 🔐 Segurança

- ✅ Proteção contra SQL Injection
- ✅ Proteção XSS (Cross-Site Scripting)
- ✅ Proteção CSRF (Cross-Site Request Forgery)
- ✅ Validação de dados do lado do servidor
- ✅ Senhas criptografadas
- ✅ Controle de acesso baseado em sessões

## 📈 Melhorias Futuras

- [ ] Sistema de busca avançada com filtros
- [ ] Upload de múltiplas imagens para anúncios
- [ ] Sistema de categorias e subcategorias
- [ ] Integração com gateway de pagamento
- [ ] API RESTful para integração mobile
- [ ] Sistema de notificações em tempo real
- [ ] Chat entre anunciantes e interessados
- [ ] Dashboard com analytics avançado
- [ ] Sistema de avaliações e comentários
- [ ] Exportação de relatórios (PDF/Excel)

## 🧪 Testes

```bash
# Executar testes unitários
composer test

# Cobertura de código
composer test:coverage
```

## 📚 Documentação

- [CodeIgniter 3 Documentation](https://codeigniter.com/userguide3/)
- [Otika Template Documentation](docs/otika-template.md)
- [API Documentation](docs/api.md)

## 🤝 Contribuindo

Contribuições são sempre bem-vindas! Para contribuir:

1. Faça um Fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona MinhaFeature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

## 📝 Convenções de Código

- PSR-12 para PHP
- Nomes de variáveis em camelCase
- Nomes de classes em PascalCase
- Comentários em português
- Commits semânticos

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 Autor

**Seu Nome**

- GitHub: [@seu-usuario](https://github.com/seu-usuario)
- LinkedIn: [Seu Perfil](https://linkedin.com/in/seu-perfil)
- Email: seu.email@example.com

## 🙏 Agradecimentos

- CodeIgniter Team pelo excelente framework
- Otika Template pela interface administrativa
- Comunidade open source

---

⭐ **Se este projeto foi útil, considere dar uma estrela!**

Desenvolvido com ❤️ e ☕

