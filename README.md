# Prática Notificações LDDM

# 🧩 Guia Rápido – Configuração do Android Studio + Flutter

---

## ⚙️ Instalação do Android Studio
- [ ] Baixar em [developer.android.com/studio](https://developer.android.com/studio)
- [ ] Instalar e abrir o Android Studio
- [ ] Escolher **Standard setup**
- [ ] Aceitar todas as **licenças SDK**
- [ ] Finalizar e abrir a tela inicial

---

## 🐦 Instalar o Flutter SDK
- [ ] Criar uma pasta para SDKs  
  ```bash
  mkdir -p ~/SDKs
  cd ~/SDKs
  git clone https://github.com/flutter/flutter.git -b stable
  ```
- [ ] Adicionar o Flutter ao PATH  
  ```bash
  export PATH="$PATH:$HOME/SDKs/flutter/bin"
  ```
- [ ] Testar a instalação  
  ```bash
  flutter --version
  ```

---

## 💡 Instalar o Dart SDK (caso não venha com o Flutter)
### Opção 1 – via Homebrew (macOS/Linux)
```bash
brew tap dart-lang/dart
brew install dart
```
### Opção 2 – manual
- [ ] Baixar em [dart.dev/get-dart](https://dart.dev/get-dart)
- [ ] Extrair e configurar o caminho:
  ```bash
  export PATH="$PATH:/caminho/para/dart/bin"
  ```

---

## 🧰 Configurar no Android Studio
- [ ] Abrir **File ▸ Settings ▸ Languages & Frameworks ▸ Flutter**
  - [ ] Definir o caminho do Flutter SDK
- [ ] Abrir **Languages & Frameworks ▸ Dart**
  - [ ] Definir o caminho do Dart SDK (caso necessário)
- [ ] Clicar em **Apply → OK**
- [ ] Reiniciar o Android Studio

---

## 📱 Configurar o Android SDK
- [ ] Abrir **Preferences ▸ Appearance & Behavior ▸ System Settings ▸ Android SDK**
- [ ] Na aba **SDK Tools**, marcar:
  - [ ] Android SDK Command-line Tools (latest)
  - [ ] Android SDK Platform-Tools
  - [ ] Android Emulator
  - [ ] Android SDK Build-Tools
- [ ] Aplicar e aguardar o download

---

## 🚀 Finalização
- [ ] Aceitar as licenças do Android SDK  
  ```bash
  flutter doctor --android-licenses
  ```
- [ ] Verificar se tudo está ok  
  ```bash
  flutter doctor
  ```
- [ ] Criar e iniciar um emulador Android pelo **Device Manager**
- [ ] Executar o primeiro app:  
  ```bash
  flutter run
  ```

---

🟢 **Pronto!** Seu ambiente Flutter + Android Studio está configurado e pronto para desenvolvimento.
