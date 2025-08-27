## Gestão de branch

1. Branch principal protegida

- __main__ (ou master) deve sempre conter a versão estável.

- Ative branch protection rules no GitHub (exigir pull request + revisão antes de merge).

2. Criação de branch a partir de main

Cada colaborador deve criar sua própria branch a partir da main:

```
git checkout main
git pull origin main
git checkout -b feature/teste-cenario-login
```

3. Nomeação de branch (padrão recomendado)

Use um padrão que identifique tipo de tarefa + contexto:

- __feature/teste-cenario-login__ → novos testes de login

- __feature/teste-cenario-reserva__ → novos testes de reserva

- __bugfix/corrigir-cenario-falha-login__ → correção de teste

- __chore/atualizar-dependencias-bdd__ → mudanças técnicas sem impacto funcional