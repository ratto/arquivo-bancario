# Gerador de Arquivos Bancários

## Setup do projeto
```
npm install
```

### Compila com hot reload para desenvolvimento
```
npm run serve
```

### Compila e minifica para produção
```
npm run build
```

### Compila com electron com hot reload para desenvolvimento
```
npm run electron:serve
```

### Compila e minifica com Electron para produção
```
npm run electron:build
```

### Para rodar seus testes unitários
```
npm run test:unit
```

### Passa o Lint e repara arquivos
```
npm run lint
```

### Customizar a Configuração
Veja [Configuration Reference](https://cli.vuejs.org/config/).

### Nota
Você precisa ter o Node versão 16.16.0 instalado, para que possa ser *buildado* com o Electron 22x.
Pode ser necessário fazer um *downgrade* da versão do seu Node caso você queira usar uma versão do Electron diferente da que foi usada neste projeto (consulte [Configuration Reference](https://www.electronjs.org/pt/blog/electron-22-0) para mais informações).
