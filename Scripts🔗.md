# 🔗 Scripts e atalhos

Pequenos exemplos de JavaScript que podem ser executados como bookmarklets no navegador.

## 🎨 Personalização visual de uma página

O exemplo abaixo altera o título da aba e o ícone exibido pelo navegador. A mudança é local e temporária: recarregar a página restaura os valores originais.

```javascript
javascript:(function() {
  var link = document.querySelector("link[rel*='icon']") || document.createElement('link');
  link.type = 'image/x-icon';
  link.rel = 'shortcut icon';
  link.href = 'https://edusp-static.ip.tv/sala-do-futuro/conteudo_logo.png';
  document.head.appendChild(link);
  document.title = 'Sala do Futuro Aluno';
})();
```

## 📌 Observações

- Bookmarklets executam código na página atual.
- Confira o código antes de executar qualquer script.
- Use apenas em páginas e situações em que você tenha autorização para fazer alterações.
