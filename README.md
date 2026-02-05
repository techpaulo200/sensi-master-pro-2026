# 🎮 Sensi Master Pro 2026

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-1.0.0-green.svg)](https://github.com/techpaulo200/sensi-master-pro-2026)

Calibrador de sensibilidade profissional para dispositivos móveis. Otimize suas configurações de sensibilidade para jogos mobile com base no seu dispositivo específico.

## 🌟 Características

- 🎯 **Calibração Precisa**: Valores otimizados para mais de 50 dispositivos
- 📱 **Multi-Marca**: Suporte para Samsung, Motorola, Xiaomi, iPhone e mais
- ⚡ **Interface Moderna**: Design responsivo e animações fluidas
- 🎨 **Tema Escuro**: Interface otimizada para longas sessões
- 💾 **Configurações DPI**: Recomendações personalizadas por dispositivo
- 🔄 **Atualizado 2026**: Base de dados atualizada com modelos recentes

## 🚀 Demo

[Ver Demo ao Vivo](https://techpaulo200.github.io/sensi-master-pro-2026)

## 📸 Screenshots

![Screenshot Principal](assets/screenshot.png)

## 🛠️ Tecnologias Utilizadas

- HTML5
- CSS3 (Variáveis CSS, Flexbox, Animações)
- JavaScript ES6+ (Classes, Arrow Functions, Promises)
- Design Responsivo

## 📦 Instalação

### Uso Direto

1. Clone o repositório:
```bash
git clone https://github.com/techpaulo200/sensi-master-pro-2026.git
```

2. Abra o arquivo `index.html` no seu navegador

### Hospedagem no GitHub Pages

1. Faça fork deste repositório
2. Vá em Settings > Pages
3. Selecione a branch `main` como source
4. Seu site estará disponível em: `https://seu-usuario.github.io/sensi-master-pro-2026`

## 💻 Estrutura do Projeto

```
sensi-master-pro-2026/
├── index.html              # Página principal
├── assets/
│   ├── css/
│   │   └── styles.css      # Estilos globais
│   └── js/
│       ├── database.js     # Base de dados de dispositivos
│       ├── calculator.js   # Lógica de cálculo
│       └── app.js          # Aplicação principal
├── README.md               # Documentação
└── LICENSE                 # Licença MIT
```

## 🎯 Como Usar

1. **Selecione a Marca** do seu dispositivo
2. **Escolha o Modelo** específico
3. **Clique em "CALIBRAR AGORA"**
4. Aguarde o processo de calibração
5. **Copie os valores** para o seu jogo

### Valores de Sensibilidade

- **GERAL**: Sensibilidade geral de mira
- **RED DOT**: Mira com Red Dot
- **2X**: Mira com scope 2x
- **4X**: Mira com scope 4x
- **AWM**: Sensibilidade para sniper AWM
- **DPI**: Configuração DPI recomendada

## 🔧 Personalização

### Adicionar Novos Dispositivos

Edite o arquivo `assets/js/database.js`:

```javascript
export const DEVICE_DATABASE = {
    "SUA_MARCA": [
        "Modelo 1",
        "Modelo 2",
        // ...
    ]
};
```

### Customizar Valores de Sensibilidade

Modifique a função `calcularSensi()` em `assets/js/calculator.js`:

```javascript
calcularSensi(marca, modelo) {
    return {
        geral: 200,
        redDot: 200,
        // Customize aqui
    };
}
```

## 🤝 Contribuindo

Contribuições são bem-vindas! Siga estes passos:

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/NovaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/NovaFeature`)
5. Abra um Pull Request

### Diretrizes de Contribuição

- Siga os padrões de código existentes
- Adicione comentários quando necessário
- Teste suas alterações em múltiplos dispositivos
- Atualize a documentação se necessário

## 📝 Roadmap

- [ ] Modo de comparação entre dispositivos
- [ ] Exportar configurações em JSON
- [ ] PWA (Progressive Web App)
- [ ] Suporte a mais jogos
- [ ] Sistema de favoritos
- [ ] Histórico de calibrações

## 🐛 Reportar Bugs

Encontrou um bug? [Abra uma issue](https://github.com/techpaulo200/sensi-master-pro-2026/issues) com:

- Descrição do problema
- Passos para reproduzir
- Comportamento esperado vs atual
- Screenshots (se aplicável)
- Informações do dispositivo/navegador

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 Autor

**Paulo Tech** ([@techpaulo200](https://github.com/techpaulo200))

## 🙏 Agradecimentos

- Comunidade de jogadores mobile
- Contribuidores do projeto
- Testadores e usuários

## 📞 Contato

- GitHub: [@techpaulo200](https://github.com/techpaulo200)
- Issues: [GitHub Issues](https://github.com/techpaulo200/sensi-master-pro-2026/issues)

---

⭐ **Se este projeto foi útil, considere dar uma estrela!** ⭐
