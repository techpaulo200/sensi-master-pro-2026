# 🔥 Sensi Master 2026
> O ecossistema definitivo para calibração de sensibilidade e DPI mobile.

O **Sensi Master 2026** é um projeto de engenharia focado em performance gamer. Evoluiu de um simples controlador de sliders para uma plataforma robusta com suporte a múltiplos perfis, feedback tátil (Haptics) e algoritmos de hardware.

---

## 🏗️ Registro de Engenharia e Dev Logs (#1 ao #60)

Este log documenta a jornada técnica, detalhando o que foi **adicionado, removido, refito e atualizado** em cada etapa.

### 🟢 Fase 1: Fundação e Kernel (#1 - #10)

* **#1 O Nascimento do Kernel**
    * **Adicionado:** Estrutura base HTML5 e inputs de range.
    * **Desenvolvedor:** *"No início, foquei no essencial: Geral, ADS e Sniper. Minha prioridade era a funcionalidade bruta antes da estética."*
* **#2 Identidade Cyber-Dark**
    * **Atualizado:** Paleta de cores para o tema gamer escuro.
    * **Desenvolvedor:** *"Refiz o CSS para sair do branco padrão. O app precisava 'falar' a língua dos jogadores logo de cara."*
* **#3 Lógica de Persistência**
    * **Adicionado:** Integração com `localStorage`.
    * **Desenvolvedor:** *"Implementei o salvamento automático. Nada pior que configurar a sensi e perder tudo ao fechar a aba."*
* **#4 Reatividade Visual**
    * **Alterado:** Gatilho de evento de `onchange` para `oninput`.
    * **Desenvolvedor:** *"Mudei como o número aparece; agora ele corre junto com o slider em tempo real, sem atraso."*
* **#5 Refatoração Clean Code**
    * **Refito:** Lógica das funções de atualização (Padrão DRY).
    * **Desenvolvedor:** *"Deletei funções repetidas e criei um loop que gerencia todos os sliders. O código ficou 40% menor."*
* **#6 Interface Glassmorphism**
    * **Adicionado:** Efeito de transparência e desfoque nos cards.
    * **Desenvolvedor:** *"Atualizei o design para o estilo vidro fosco, usando `backdrop-filter` para um ar de tecnologia moderna."*
* **#7 Escalabilidade Mobile**
    * **Alterado:** Unidades de `px` para `rem` e `vh`.
    * **Desenvolvedor:** *"Removi medidas fixas que quebravam em telas pequenas. Agora o layout se adapta a qualquer celular."*
* **#8 Blindagem de Dados**
    * **Adicionado:** Blocos `try...catch` para leitura de JSON.
    * **Desenvolvedor:** *"Protegi o carregamento. Se o cache estiver corrompido, o app reseta para o padrão em vez de travar."*
* **#9 Feedback Tátil**
    * **Adicionado:** Versão inicial da **Vibration API**.
    * **Desenvolvedor:** *"Adicionei uma vibração curta ao salvar. Queria uma confirmação física da ação concluída."*
* **#10 Milestone v1.0**
    * **Atualizado:** Padronização completa para ES6+.
    * **Desenvolvedor:** *"Limpei comentários de teste e preparei o terreno para as funções de hardware que viriam."*

---

### 🟡 Fase 2: Otimização e Hardware (#11 - #30)

* **#11 Modernização de Variáveis**
    * **Alterado:** Troca de `var` por `const` e `let`.
    * **Desenvolvedor:** *"Removi o uso de `var` para evitar bugs de escopo e deixar o sistema mais seguro."*
* **#12 Integridade de Cache**
    * **Adicionado:** Verificação de chaves vazias no armazenamento.
    * **Desenvolvedor:** *"Refiz a lógica de inicialização para evitar o erro de 'undefined' na tela inicial."*
* **#13 Performance de Carregamento**
    * **Atualizado:** Scripts movidos para o rodapé com atributo `defer`.
    * **Desenvolvedor:** *"Mudei a ordem de leitura do navegador: o design carrega primeiro e o código depois."*
* **#14 Estilização de Controles**
    * **Alterado:** Estética dos sliders via CSS customizado.
    * **Desenvolvedor:** *"Retirei o visual padrão do Android/Windows e criei sliders neon exclusivos do projeto."*
* **#15 Cálculo de DPI Base**
    * **Adicionado:** Algoritmo inicial de sugestão de DPI.
    * **Desenvolvedor:** *"Criei uma lógica matemática que sugere DPIs fixas baseadas na sensibilidade escolhida."*
* **#16 Limpeza de Arquivos**
    * **Removido:** Assets e bibliotecas não utilizadas.
    * **Desenvolvedor:** *"Fiz um 'faxinão'. O app agora carrega quase instantaneamente mesmo em redes lentas."*
* **#17 Precisão Cirúrgica**
    * **Atualizado:** Tratamento de casas decimais.
    * **Desenvolvedor:** *"Refiz o arredondamento: display mostra inteiros, mas o cálculo mantém a precisão decimal interna."*
* **#18 Otimização Touch**
    * **Adicionado:** Suporte a eventos `touchstart`.
    * **Desenvolvedor:** *"Removi o atraso de toque de alguns celulares. A resposta agora é imediata e sem lag."*
* **#19 Alerta de Estado**
    * **Adicionado:** Indicador de 'não salvo' nos cards.
    * **Desenvolvedor:** *"Criei um aviso visual para o usuário não esquecer de gravar as alterações feitas."*
* **#20 Milestone v2.1.5**
    * **Refito:** Estrutura do CSS para evitar conflitos de cache.
    * **Desenvolvedor:** *"Ajustei o versionamento interno para o navegador baixar a versão nova sem precisar limpar cache."*
* **#21 Haptic Patterns**
    * **Atualizado:** Padrões de vibração diferenciados para ações.
    * **Desenvolvedor:** *"Refiz o sistema: o celular vibra diferente ao salvar e ao resetar. Ficou muito mais intuitivo."*
* **#22 DPI Dinâmica v2**
    * **Adicionado:** Algoritmo que cruza dados de ADS e Sniper.
    * **Desenvolvedor:** *"Atualizei a inteligência: o app agora entende a relação entre as sensis para dar uma DPI precisa."*
* **#23 PWA Ready**
    * **Adicionado:** Arquivo `manifest.json`.
    * **Desenvolvedor:** *"Preparei o app para ser instalado na tela inicial do celular como um aplicativo nativo."*
* **#24 Legibilidade Extrema**
    * **Alterado:** Contraste de cores e fontes.
    * **Desenvolvedor:** *"Refiz a tipografia para garantir leitura clara mesmo sob luz solar intensa."*
* **#25 Fallback de Segurança**
    * **Adicionado:** Sistema de salvamento temporário (`SessionStorage`).
    * **Desenvolvedor:** *"Criei um plano B para navegadores que bloqueiam o armazenamento permanente."*
* **#26 Refatoração CSS Profunda**
    * **Removido:** Estilos inline e seletores lentos.
    * **Desenvolvedor:** *"Limpei o HTML novamente. O design agora é 100% separado do conteúdo técnico."*
* **#27 Splash Animation**
    * **Adicionado:** Efeito de fade-in suave.
    * **Desenvolvedor:** *"Adicionei uma animação de entrada para dar uma sensação de software robusto e bem acabado."*
* **#28 Otimização de RAM**
    * **Alterado:** Gerenciamento de variáveis globais.
    * **Desenvolvedor:** *"Refiz a estrutura de objetos internos para manter o consumo de memória sempre baixo."*
* **#29 Cloud Prep**
    * **Adicionado:** Estrutura de exportação para objetos JSON.
    * **Desenvolvedor:** *"Preparei o terreno para a nuvem, organizando a sensi para fácil integração com bancos de dados."*
* **#30 Estado Atual v2.2.5**
    * **Atualizado:** Revisão final de toda a lógica do Log #1 ao #30.
    * **Desenvolvedor:** *"Chegamos à maturidade técnica. O projeto evoluiu de uma ideia simples para um ecossistema sólido."*

---

### 🔵 Fase 3: Inteligência e Automação (#31 - #50)

* **#31 Sugestão por Arquétipo:** Calibração baseada no estilo de jogo (Rush vs Sniper).
* **#32 Garbage Collection:** Limpeza ativa de listeners órfãos.
* **#33 Protótipo OCR:** Estrutura para leitura de prints de tela.
* **#34 Temas Dinâmicos:** Adaptação de cores baseada no sistema operacional.
* **#35 IndexedDB Migration:** Suporte para armazenamento de imagens pesadas.
* **#36 Share Sensi:** Gerador de códigos curtos (Hash) para compartilhamento.
* **#37 Anti-Jitter:** Sincronização com `requestAnimationFrame`.
* **#38 Service Workers:** Funcionamento 100% offline.
* **#39 Battery Drain Opt:** Ajuste fino na vibração para economia de energia.
* **#40 Dev Mode:** Interface oculta para monitoramento de cálculos matemáticos.
* **#41 IA de Tela:** Correção baseada na resolução e polegadas do aparelho.
* **#42 Zero External Deps:** Migração de ícones para SVGs inline.
* **#43 Safe Zones:** Ajuste de layout para celulares com notch/câmera na tela.
* **#44 Recoil Simulator:** Preview visual da movimentação de mira.
* **#45 Passive Events:** Otimização de performance de scroll mobile.
* **#46 Exportação JSON:** Backup físico da configuração.
* **#47 CSS Variables v2:** Centralização do design system em variáveis `:root`.
* **#48 Input Híbrido:** Suporte para digitação manual de valores.
* **#49 Filtro de Luz Azul:** Automação de cores para uso noturno.
* **#50 Milestone v2.5.0:** Finalização do ecossistema inteligente.

---

### 🎮 Fase 4: Expansão de Perfis (#51 - #60)

* **#51 Sistema Multi-Perfis (v2.6.0)**
    * **Adicionado:** Banco de dados para salvar perfis distintos (FF, COD, PUBG).
    * **Desenvolvedor:** *"O usuário não precisa mais sobrescrever dados. Agora ele tem uma aba para cada jogo separadamente."*
* **#52 Refatoração de UI (Tab System)**
    * **Alterado:** Menu lateral por barra de navegação inferior estilo nativo.
    * **Desenvolvedor:** *"Facilitei o alcance do polegar. O app agora tem a ergonomia de um app da App Store."*
* **#53 Integração com Giroscópio**
    * **Adicionado:** Sensor de inclinação para medir estabilidade da mão.
    * **Desenvolvedor:** *"Usei sensores do celular para sugerir se o usuário deve usar sensi alta ou baixa baseado no seu tremor."*
* **#54 Purge de CSS Legado**
    * **Retirado:** Antigas classes de cores fixas obsoletas.
    * **Desenvolvedor:** *"Deletei quase 200 linhas de estilos repetidos. O código está mais limpo do que nunca."*
* **#55 Segurança de Dados**
    * **Atualizado:** Sistema de sanitização contra injeção de scripts.
    * **Desenvolvedor:** *"Bloqueei qualquer tentativa de inserir códigos maliciosos nos nomes dos perfis."*
* **#56 Suavização de DPI (v2.7.0)**
    * **Adicionado:** Cálculo de 'Pixel Skipping' para resoluções altas.
    * **Desenvolvedor:** *"O app agora avisa se a combinação de DPI vai causar pulos de pixel na mira."*
* **#57 Bulk Export**
    * **Adicionado:** Função para exportar todos os perfis em um único arquivo `.sensi`.
    * **Desenvolvedor:** *"Criei um jeito do usuário baixar um backup definitivo de todas as suas configurações de uma vez."*
* **#58 Aceleração por Hardware**
    * **Alterado:** Uso de `will-change: transform` nas animações.
    * **Desenvolvedor:** *"Forcei o uso da GPU para as transições, economizando bateria e mantendo o celular frio."*
* **#59 Sensi da Comunidade**
    * **Adicionado:** Área para importação de códigos de influenciadores.
    * **Desenvolvedor:** *"Criei uma ponte para buscar recomendações externas e manter o app sempre atualizado."*
* **#60 Milestone v2.8.0**
    * **Atualizado:** Documentação técnica e comentários finais do código.
    * **Desenvolvedor:** *"Chegamos ao Log #60. O projeto agora é um gerenciador completo de performance gamer. Estamos prontos para o próximo nível!"*

---

## 🛠️ Tecnologias Utilizadas
* **JS:** ES6+, Vibration API, Device Orientation API.
* **Storage:** LocalStorage, IndexedDB.
* **CSS:** Glassmorphism, CSS Variables, Flexbox/Grid.
* **Mobile:** PWA (Progressive Web App).
