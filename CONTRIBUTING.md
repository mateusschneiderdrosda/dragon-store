# Contribuindo para Dragon Store

Obrigado por se interessar em contribuir! Este documento fornece diretrizes e instruções.

## 📋 Diretrizes Gerais

1. **Clean Architecture**: Mantenha o código modular e bem organizado
2. **SOLID Principles**: Siga os princípios SOLID em todo o código
3. **Type Safety**: Use type hints no Python e TypeScript
4. **Testing**: Toda nova funcionalidade deve ter testes
5. **Documentation**: Documente APIs e funcionalidades complexas
6. **Commits**: Use commits atômicos com mensagens descritivas

## 🔄 Fluxo de Desenvolvimento

1. **Fork** o repositório
2. **Crie uma branch** para sua feature: `git checkout -b feature/nome-feature`
3. **Commit** suas mudanças: `git commit -am 'Add: descrição da feature'`
4. **Push** para a branch: `git push origin feature/nome-feature`
5. **Abra um Pull Request**

## 📝 Padrões de Commit

```
<tipo>(<escopo>): <descrição>

<corpo>

<rodapé>
```

### Tipos
- `feat`: Nova funcionalidade
- `fix`: Correção de bug
- `docs`: Alterações na documentação
- `style`: Formatação, falta de ponto e vírgula, etc
- `refactor`: Código que não muda funcionalidade
- `test`: Adição ou atualização de testes
- `chore`: Atualizações de dependências, etc

## 💻 Backend Development

### Setup
```bash
cd backend
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### Rodar servidor
```bash
uvicorn app.main:app --reload
```

### Testes
```bash
pytest
pytest --cov=app tests/
```

## 🎨 Frontend Development

### Setup
```bash
cd frontend
npm install
```

### Rodar servidor
```bash
npm run dev
```

## 🤖 Bot Development

### Setup
```bash
cd discord-bot
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## ✅ Checklist antes de PR

- [ ] Código segue Clean Architecture e SOLID
- [ ] Type hints/TypeScript completo
- [ ] Testes escritos e passando
- [ ] Documentação atualizada
- [ ] Commits atômicos com boas mensagens
- [ ] Nenhum código incompleto ou TODO