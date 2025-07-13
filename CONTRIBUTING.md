# Guia de boas práticas de contribuição na comunidade da Associação Python Brasil (APyB)

Este documento estabelece diretrizes de como contribuir com discussões nesse repositório, prezando manter o ambiente saudável, seguro, livre de preconceitos, em conformidade com a Lei Geral de Proteção de Dados (LGPD - Lei nº 13.709/2018) e boas práticas de segurança da informação.

## 🛡️ Princípios Fundamentais da LGPD

### 1. Finalidade
- Compartilhe dados pessoais apenas quando necessário para a finalidade específica da discussão
- Evite divulgar informações pessoais desnecessárias para o contexto

### 2. Adequação e Necessidade
- Questione-se: "Esta informação pessoal é realmente necessária para minha contribuição?"
- Priorize dados anonimizados ou pseudonimizados quando possível

### 3. Transparência
- Seja claro sobre por que está compartilhando determinada informação
- Informe se a informação compartilhada pode ser sensível

## 🚫 Dados que NÃO devem ser compartilhados

### Dados Pessoais Sensíveis (Art. 5º, II da LGPD)
- **Origem racial ou étnica** - Evite referências desnecessárias
- **Convicção religiosa** - Compartilhe apenas se essencial ao contexto
- **Opinião política** - Mantenha discussões técnicas
- **Filiação sindical** - Informação desnecessária para discussões técnicas
- **Dados de saúde** - Nunca compartilhe condições médicas específicas
- **Vida sexual** - Informação irrelevante para o contexto comunitário
- **Dados genéticos ou biométricos** - Nunca compartilhe

### Dados Pessoais Comuns (que requerem cuidado)
- **CPF, RG, ou outros documentos** - Nunca compartilhe números completos
- **Endereço residencial completo** - Use apenas cidade/região quando necessário
- **Telefone pessoal** - Prefira meios de contato profissionais
- **E-mail pessoal** - Use e-mail profissional quando apropriado
- **Dados bancários** - Nunca compartilhe
- **Senhas ou chaves de API** - Use variáveis de ambiente e exemplos genéricos

## ✅ Boas Práticas para Proteção de Dados

### 1. Anonimização e Pseudonimização
```
❌ Evite: "João Silva (CPF: 123.456.789-00) da empresa XYZ reportou este problema"
✅ Prefira: "Um desenvolvedor da comunidade reportou este problema"
✅ Ou: "João da empresa XYZ reportou este problema" (apenas nome)
```

### 2. Compartilhamento de Código e Exemplos
```
❌ Evite dados reais:
API_KEY = "sk-1234567890abcdef"
USER_EMAIL = "joao.silva@email.com"
DATABASE_URL = "postgresql://user:pass@real-server.com/db"

✅ Use dados fictícios:
API_KEY = "sk-your-api-key-here"
USER_EMAIL = "usuario@exemplo.com"
DATABASE_URL = "postgresql://usuario:senha@localhost/nome_db"
```

### 3. Relatórios de Problemas (Issues/Discussions)
- Use dados fictícios ou anonimizados em exemplos
- Remova logs que contenham informações pessoais
- Substitua informações sensíveis por placeholders

### 4. Screenshots e Imagens
- Borre ou edite informações pessoais visíveis
- Use dados de teste em demonstrações
- Evite capturar informações da barra de endereços que possam conter dados sensíveis

## 🔒 Segurança em Repositórios

### 1. Secrets e Variáveis de Ambiente
- Nunca faça commit de arquivos `.env` com dados reais
- Use `.env.example` com valores de exemplo
- Configure adequadamente o `.gitignore`

### 2. Historico do Git
- Verifique commits antes de enviar
- Use `git log --oneline` para revisar histórico
- Se dados sensíveis foram commitados acidentalmente, remova do histórico

### 3. Configurações e Logs
- Sanitize logs antes de compartilhar
- Remova tokens de autenticação de configurações de exemplo
- Use ferramentas como `git-secrets` para prevenção

## 🚨 Em Caso de Vazamento Acidental

### Ações Imediatas:
1. **Delete ou edite** o conteúdo imediatamente
2. **Notifique** os moderadores se não conseguir remover
3. **Documente** o incidente para análise
4. **Comunique** às pessoas afetadas, se aplicável


## 📞 Contato para Questões de Privacidade

Se você identificar vazamentos de dados ou tiver dúvidas sobre privacidade:
- Abra uma issue privada ou contate os moderadores
- Para questões urgentes, entre em contato diretamente com a APyB

## 📚 Recursos Adicionais

### Legislação
- [Lei Geral de Proteção de Dados - LGPD](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm)
- [Guia ANPD para Desenvolvedores](https://www.gov.br/anpd/pt-br)

### Ferramentas Úteis
- [git-secrets](https://github.com/awslabs/git-secrets) - Previne commits com dados sensíveis
- [detect-secrets](https://github.com/Yelp/detect-secrets) - Scanner de secrets
- [GitGuardian](https://gitguardian.com/) - Monitoramento de secrets

### Geradores de Dados Fictícios
- [Faker (Python)](https://faker.readthedocs.io/) - Geração de dados fictícios
- [JSONPlaceholder](https://jsonplaceholder.typicode.com/) - API com dados de exemplo
- [Lorem Ipsum](https://www.lipsum.com/) - Texto de exemplo

---

**Lembre-se**: A proteção de dados é responsabilidade de todos. Quando em dúvida, prefira não compartilhar a informação ou busque orientação dos moderadores.

**Este documento está em conformidade com a LGPD (Lei nº 13.709/2018) e será atualizado conforme necessário para manter a conformidade com mudanças na legislação.**
