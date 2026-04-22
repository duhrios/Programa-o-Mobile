# Settings — Tela de Configurações em Jetpack Compose

Projeto Android Studio que implementa a atividade de tela de Configurações utilizando Jetpack Compose.

## Como abrir

1. Abra o **Android Studio** (Hedgehog ou superior).
2. Selecione **File → Open** e aponte para a pasta `android-settings/`.
3. Aguarde o Gradle sincronizar (ele vai baixar as dependências automaticamente).
4. Execute em um emulador ou dispositivo Android (API 24+).

## Componentes implementados

- `SettingsHeader` — Cabeçalho com nome do app e ícone de configurações
- `SettingsImage` — Imagem de perfil clicável
- `SettingsCheckbox` — Aceitar cookies não essenciais
- `SettingsSwitch` — Permitir download usando dados móveis
- `SettingsSlider` — Configurar tamanho do texto
- `SettingsRadioButtons` — Forma de pagamento preferida (PayPal, Credit Card, Bank Transfer)
- `SettingsAlertDialog` — Botão Sign out com confirmação

Todos os textos estão em `app/src/main/res/values/strings.xml` e o estilo do cabeçalho em `ui/theme/Type.kt` (`HeaderTextStyle`).

## Estrutura

```
android-settings/
├── app/
│   ├── build.gradle.kts
│   └── src/main/
│       ├── AndroidManifest.xml
│       ├── java/com/example/settings/
│       │   ├── MainActivity.kt
│       │   └── ui/theme/
│       │       ├── Color.kt
│       │       ├── Theme.kt
│       │       └── Type.kt
│       └── res/
│           ├── drawable/sunflower.xml
│           └── values/{strings,colors,themes}.xml
├── build.gradle.kts
├── settings.gradle.kts
└── gradle.properties
```
<img width="630" height="828" alt="image" src="https://github.com/user-attachments/assets/6762f0b4-f888-4799-936c-e2bc2d558c7d" />
