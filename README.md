<div align="center">

<img src="https://edicarlosmv.github.io/fintrack-site/icon.png" width="100" height="100" style="border-radius:22px" alt="FinTrack Logo"/>

# FinTrack

### Controle financeiro inteligente · Smart financial control

[![Google Play](https://img.shields.io/badge/Google_Play-Em_breve-1D9E75?style=for-the-badge&logo=google-play&logoColor=white)](https://play.google.com/store/apps/details?id=com.yourname.fintrack)
[![Licença](https://img.shields.io/badge/Licença-MIT-534AB7?style=for-the-badge)](LICENSE)
[![Plataforma](https://img.shields.io/badge/Plataforma-Android-E24B4A?style=for-the-badge&logo=android&logoColor=white)](https://play.google.com/store)
[![Versão](https://img.shields.io/badge/Versão-1.0.0-BA7517?style=for-the-badge)](https://github.com/edicarlosmv/fintrack-site/releases)

**🌐 [fintrackapp.com.br](https://edicarlosmv.github.io/fintrack-site) · PT 🇧🇷 · EN 🇺🇸**

</div>

---

## 📱 Sobre o app

O **FinTrack** é um aplicativo mobile de controle financeiro pessoal desenvolvido em React Native com Expo. Vai além do básico — mostra o **futuro do seu bolso** antes que ele chegue.

> *"O único app que mostra quanto da sua renda futura já está comprometida com parcelas."*

---

## ✨ Funcionalidades

| Recurso | Descrição | Plano |
|---|---|---|
| 💰 Lançamentos | Receitas e despesas ilimitadas | Gratuito (50/mês) / PRO |
| 💳 Parcelamentos | Controle de compras parceladas com lembretes de vencimento | Todos |
| 🔔 Lembretes | Alertas de parcelas a vencer e em atraso | Todos |
| 📊 Gráficos | Evolução mensal dos últimos 6 meses por categoria | PRO |
| 🔭 Previsão | Projeção financeira dos próximos 3 meses | PRO |
| 🎯 Metas | Metas financeiras com prazo e progresso visual | PRO |
| 📐 50/30/20 | Regra financeira calculada automaticamente | PRO |
| ❤️ Score | Score de saúde financeira de 0 a 100 | PRO |
| 🌐 Bilíngue | Português e inglês com detecção automática | Todos |
| 🌙 Dark mode | Suporte automático ao modo escuro do sistema | Todos |

---

## 💎 Planos

| | Gratuito | PRO Mensal | PRO Anual |
|---|:---:|:---:|:---:|
| **Preço** | R$ 0 | R$ 19,90/mês | R$ 12,90/mês |
| **Lançamentos** | 50/mês | Ilimitado | Ilimitado |
| **Parcelas + lembretes** | ✅ | ✅ | ✅ |
| **Gráficos de desempenho** | ❌ | ✅ | ✅ |
| **Previsão 3 meses** | ❌ | ✅ | ✅ |
| **Score de saúde** | ❌ | ✅ | ✅ |
| **Trial gratuito** | — | 7 dias | 7 dias |
| **Economia** | — | — | 35% |

---

## 🛠️ Tecnologias

```
React Native · Expo ~51     → Framework mobile
TypeScript                  → Linguagem tipada
React Navigation            → Navegação por abas
Expo SecureStore            → Armazenamento criptografado
Expo Localization           → Detecção de idioma
react-i18next               → Internacionalização PT/EN
react-native-chart-kit      → Gráficos de desempenho
react-native-svg            → Score ring animado
@expo/vector-icons          → Ícones Ionicons
EAS Build                   → Build e deploy nas lojas
RevenueCat (planejado)      → Gestão de assinaturas
```

---

## 🚀 Rodando localmente

### Pré-requisitos
- Node.js 18+
- npm ou yarn
- Expo Go (celular) ou emulador Android/iOS

### Instalação

```bash
# Clone o repositório do app
git clone https://github.com/edicarlosmv/fintrack-app.git
cd fintrack-app

# Instale as dependências
npm install

# Inicie o servidor de desenvolvimento
npm start
```

Escaneie o QR code com o **Expo Go** no celular.

---

## 📦 Build de produção

```bash
# Instalar EAS CLI
npm install -g eas-cli
eas login

# Build Android (Google Play)
eas build --platform android --profile production

# Publicar na Play Store
eas submit --platform android

# Build iOS (App Store)
eas build --platform ios --profile production
eas submit --platform ios
```

---

## 📁 Estrutura do projeto

```
fintrack/
├── App.tsx                        # Entrada, navegação, header bilíngue
├── app.json                       # Config Expo
├── eas.json                       # Config de build EAS
├── assets/                        # Ícones e splash screen
└── src/
    ├── i18n/index.ts              # Traduções PT + EN
    ├── contexts/AppContext.tsx    # Estado global
    ├── utils/
    │   ├── storage.ts             # Tipos e helpers financeiros
    │   ├── theme.ts               # Cores light/dark
    │   └── subscription.ts        # Planos e RevenueCat
    ├── components/index.tsx       # Componentes reutilizáveis
    └── screens/
        ├── HomeScreen.tsx         # Saldo, métricas, alertas
        ├── EntriesScreen.tsx      # Lançamentos (editar/excluir)
        ├── RemindersScreen.tsx    # Lembretes de vencimento
        ├── PerformanceScreen.tsx  # Gráficos 6 meses
        ├── ForecastScreen.tsx     # Previsão 3 meses
        ├── PlanScreen.tsx         # Metas + 50/30/20
        ├── SubscriptionScreen.tsx # Planos PRO + trial
        ├── HealthScreen.tsx       # Score + indicadores
        └── AddEntryModal.tsx      # Modal de lançamento
```

---

## 🔐 Privacidade

Todos os dados ficam armazenados **exclusivamente no dispositivo do usuário** (Expo SecureStore — criptografado). Nenhum dado é enviado para servidores externos.

📄 [Política de Privacidade](https://edicarlosmv.github.io/fintrack-site#privacidade)

---

## 📊 Roadmap

- [x] Lançamentos de receitas, despesas e parcelas
- [x] Lembretes de vencimento com status
- [x] Gráficos de desempenho 6 meses
- [x] Previsão financeira 3 meses
- [x] Score de saúde financeira
- [x] Metas com regra 50/30/20
- [x] Bilíngue PT/EN
- [x] Dark mode
- [x] Publicação Google Play
- [ ] Assinaturas via RevenueCat
- [ ] Backend Supabase (sync entre dispositivos)
- [ ] Importação de extrato bancário (OFX/CSV)
- [ ] Notificações push de vencimento
- [ ] Widget para tela inicial Android/iOS
- [ ] Exportar relatório PDF mensal
- [ ] Open Finance Brasil
- [ ] Publicação App Store iOS

---

## 📬 Contato

**Edicarlos Mangabeira**
- 📧 suporte@fintrack.app
- 🌐 [edicarlosmv.github.io/fintrack-site](https://edicarlosmv.github.io/fintrack-site)
- 🐙 [github.com/edicarlosmv](https://github.com/edicarlosmv)

---

## 📄 Licença

MIT © 2026 Edicarlos Mangabeira — livre para uso comercial.

---

<div align="center">

**Feito com 💚 e muita organização financeira**

⭐ Se o projeto te ajudou, deixe uma estrela!

</div>
