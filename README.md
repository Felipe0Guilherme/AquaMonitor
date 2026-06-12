# AquaMonitor 🐠

> Aplicativo mobile para **monitoramento de parâmetros de aquário**, desenvolvido com React Native e Expo. Permite que aquaristas acompanhem em tempo real os valores essenciais da água — pH, temperatura, amônia, oxigênio dissolvido, TDS e mais — tudo em uma interface otimizada para mobile.

---

## 📱 Sobre o Projeto

O AquaMonitor nasceu da necessidade de ter um controle centralizado e visual dos parâmetros de um aquário. O app oferece uma experiência fluida com navegação entre telas, listagem de parâmetros via `FlatList`, componentes customizados e suporte a atualizações Over-the-Air (OTA) sem necessidade de nova publicação nas lojas.

É o projeto de destaque do portfólio, demonstrando domínio do ecossistema React Native / Expo de ponta a ponta.

---

## 🗂️ Estrutura do Projeto

```
AquaMonitor/
├── App.js              # Ponto de entrada — navegação e estrutura raiz
├── app.json            # Configurações do Expo (nome, slug, versão, ícone)
├── eas.json            # Configurações de build e perfis do EAS CLI
├── babel.config.js     # Configuração do Babel para Expo
├── assets/             # Ícones, splash screen e imagens
└── .expo/              # Cache e metadados locais do Expo (não versionar)
```

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| **React Native** | Framework principal para UI mobile nativa |
| **Expo** | Plataforma de desenvolvimento e gerenciamento do app |
| **EAS CLI** | Build, submit e publicação nas stores (Android/iOS) |
| **OTA Updates** | Atualizações Over-the-Air via Expo Updates |
| **FlatList** | Listagem performática dos parâmetros |
| **React Navigation** | Navegação entre telas (Stack / Tab) |
| **JavaScript (ES6+)** | 100% da base de código |

---

## ✨ Funcionalidades

- 📊 **Monitoramento de parâmetros** — pH, temperatura, NH₃ (amônia), O₂, TDS e outros
- 📋 **Listagem com FlatList** — scroll performático mesmo com muitos registros
- 🧭 **Navegação entre telas** — fluxo intuitivo entre dashboards e detalhes
- 🔄 **OTA Updates** — recebe atualizações sem passar por review das stores
- 📱 **Interface otimizada para mobile** — componentes customizados, layout responsivo
- ⚙️ **Build com EAS CLI** — pronto para geração de APK/IPA e publicação

---

## 🚀 Como Rodar Localmente

### Pré-requisitos

- Node.js 18+
- Expo CLI instalado globalmente:
  ```bash
  npm install -g expo-cli
  ```
- App **Expo Go** instalado no celular (Android ou iOS)

### Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/Felipe0Guilherme/AquaMonitor.git
   cd AquaMonitor
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. Inicie o servidor de desenvolvimento:
   ```bash
   npx expo start
   ```

4. Escaneie o QR Code com o **Expo Go** no celular.

---

## 📦 Build com EAS CLI

Para gerar um build de produção (APK ou IPA):

```bash
# Instalar EAS CLI
npm install -g eas-cli

# Login na conta Expo
eas login

# Build Android (APK)
eas build --platform android --profile preview

# Build iOS
eas build --platform ios --profile production
```

Os perfis de build estão configurados em `eas.json`.

---

## 🔄 OTA Updates

Para publicar uma atualização sem novo build:

```bash
eas update --branch production --message "Descrição da atualização"
```

O app receberá a atualização automaticamente na próxima abertura.

---

## 📌 Próximos Passos

- [ ] Persistência local de dados com AsyncStorage ou SQLite
- [ ] Gráficos históricos de parâmetros ao longo do tempo
- [ ] Alertas e notificações push quando parâmetros saem da faixa ideal
- [ ] Suporte a múltiplos aquários
- [ ] Publicação na Google Play Store

---

## 👨‍💻 Autor

**Felipe Guilherme**
Desenvolvedor Front-End & Mobile — São Paulo, SP
[GitHub](https://github.com/Felipe0Guilherme) · [Portfólio](https://website-portfolio-theta-ashen.vercel.app)

---

## 📄 Licença

Este projeto é open source e está disponível sob a licença [MIT](LICENSE).
